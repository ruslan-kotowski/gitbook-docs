---
title: Referencia de Jira in situ con autorización de terceros usando OAuth 2.0
article_id: 26726425696530
translation_id: 26751143866130
locale: es
sidebar_position: 11
created_at: '2025-05-16T09:09:48Z'
updated_at: '2025-11-25T15:51:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Quién puede hacerlo: Admins de empresa ¿Cuáles son los planes?: Enterprise'
---

Este artículo proporciona detalles técnicos para usar un servidor de autorización de terceros con OAuth 2.0 para integrar Jira con Miro.

Para aprender cómo establecer una conexión, consulta [Conectar a Jira on-premise con servidores de autorización de terceros usando OAuth 2.0](https://help.miro.com/hc/articles/25692796700306).

## Cómo funciona la integración de Jira con Miro utilizando autorización in situ y OAuth 2.0

El siguiente gráfico muestra el flujo de comunicación entre Miro y un servidor de autorización de Jira en las instalaciones.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*Integración de Miro y Jira usando un servidor de autorización local a través de una puerta de enlace API*

## Parámetros de configuración

Para configurar el flujo de autorización entre Miro y Jira usando un servidor de autorización de terceros con OAuth 2.0, debes especificar los siguientes parámetros:

- **Servidor de autorización**
  - URL de solicitud de autorización
  - URL de solicitud de token
  - Alcance
- **Configuración de la aplicación de autorización**
  - ID de cliente
  - Secreto de cliente
- **Instancia de Jira**
  - URL pública de Jira
  - URL de base de Jira; URL interna

:::note
Miro proporciona la URL de redirección que el servidor de autorización valida contra la aplicación registrada.
:::

**Más información:** Consulta [Conectar a Jira local con servidores de autorización de terceros utilizando OAuth 2.0](https://help.miro.com/hc/articles/25692796700306).

## Solicitudes de autorización de usuarios entre Miro y el servidor de autorización local

Para una integración entre Miro y Jira usando un servidor de autorización de terceros, el siguiente gráfico muestra el flujo de solicitud de autorización de usuario.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*Solicitud de autorización de usuario*

### Solicitud de autorización

```
https://{authorization_URL}?
    tipo_de_respuesta=código&
    client_id={CLIENT_ID}&
    redirect_uri={URI de redirección de Miro}&
    scope={scope}&
    estado={{state}}
```

El usuario puede agregar parámetros a la solicitud de autorización como pares clave-valor en la configuración.

### Solicitud de token

```
curl --request POST \
    --url '{token request URL}' \
    --header 'content-type: application/x-www-form-urlencoded' \

    --data grant_type=código_de_autorización \
    --data 'client_id={CLIENT_ID}' \
    --data 'client_secret={CLIENT_SECRET}' \
    --data 'code={Código de autorización obtenido}' \
    --data 'redirigir_uri={Miro Redirigir URI}' \
```

Después de que Miro reciba el código de autorización, Miro proporciona el estado y solicita un par de tokens.

### Intercambio de tokens de actualización

```
curl --request POST \
    --url '{URL de solicitud de token}' \
    --header 'content-type: application/x-www-form-urlencoded' \
    --data grant_type=refresh_token \
    --data 'client_id={CLIENT_ID}' \
    --data 'refresh_token={current valid refresh token}' \
```

Asegúrate de que la operación de token de actualización esté habilitada; habilita el acceso sin conexión a las APIs.

### Solicitudes de API de Jira

```
curl --request GET \
    --url {Jira Public URL}/rest/api/{apiversion}/... \
    --header 'autorización: Portador {accessToken}
    --header 'content-type: application/json'
```

Cada solicitud utiliza la URL pública de Jira proporcionada como URL base y el token de acceso del usuario como token del portador.
