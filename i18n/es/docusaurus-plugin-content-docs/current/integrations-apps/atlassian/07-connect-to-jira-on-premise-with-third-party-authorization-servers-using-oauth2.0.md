---
title: Conecta con Jira in situ usando servidores de autorización de terceros mediante
  OAuth2.0
article_id: 25692796700306
translation_id: 26751298772498
locale: es
sidebar_position: 9
created_at: '2025-05-16T09:14:10Z'
updated_at: '2025-11-25T15:50:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Quién puede hacerlo: Admins de empresa Qué planes: Enterprise'
---

> *✏️* Conectar Jira mediante un servidor de autorización solo se habilita a nivel organizacional.

Este artículo proporciona los pasos para conectar Miro a Jira con un servidor de autorización interno de terceros, utilizando OAuth2.0.

Para conocer los detalles técnicos sobre esta configuración, consulta el artículo de referencia para [Jira on-premise con autorización de terceros usando OAuth 2.0](https://help.miro.com/hc/articles/26726425696530).

## Requisitos previos

- Asegúrate de tener los siguientes permisos:
  - Admin de empresa de Miro
  - (Opcional) Administrador del sistema Jira, si quieres usar webhooks automáticos.
- En tu servidor de autorización, crea una aplicación OAuth 2.0.
- Configura la URL de redirección en tu aplicación OAuth 2.0 a la siguiente URL:
  https://integrations.miro.com/api/external-auth/oauth2/callback
- Asegúrate de tener los siguientes detalles de tu aplicación OAuth 2.0 listos para configurar en Miro:
  - URL de autorización
  - URL de token
  - ID de cliente
  - Secreto de cliente
  - Alcance

## Conectar a Jira in situ con servidores de terceros usando OAuth 2.0

1. En tu panel de Miro, selecciona tu avatar en la esquina superior derecha y ve a **Consola de administración** | **Configuración**.
2. Ir a **Aplicaciones e integraciones ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)**> **Aplicaciones** >> **Pestaña de gestionar aplicaciones** .
3. Asegúrate de que **Permitir solo aplicaciones de la siguiente lista** esté habilitado.
4. En la columna **Aplicación**, para **Tarjetas Jira** selecciona **Configuración**.
5. Haz clic en **Agregar nueva conexión**.
6. En **configuración de Jira**, haz clic en **Centro de datos de Jira**.
7. En **Método de autenticación**, selecciona **OAuth2.0 a través de un servidor de autorización de terceros**.
8. Debajo de **Jira URL**, ingresa la URL de tu instancia de Jira.
   > *✏️* Puedes añadir tu URL base de Jira externa o tu URL interna de Jira. Si usas una URL interna de Jira, entonces debes especificar tu URL del gateway API externo en el paso 10.

   > *✏️* En general, usar una URL interna te permite ajustar la funcionalidad de navegación a la fuente.
9. (Opcional) Para establecer esta conexión como la conexión predeterminada para todos los equipos de tu organización, marca **Establecer como predeterminada**.
10. (Opcional) Si usas un gateway de API para hacer solicitudes a Jira, entonces para **URL de base de Jira API Gateway**, ingresa la URL de tu gateway de API externa.
11. Ingresa los siguientes detalles de tu aplicación OAuth 2.0:
    - URL de autorización
    - URL de token
    - ID de cliente
    - Secreto de cliente
    - Alcance
12. (Opcional) Para recibir actualizaciones en tiempo real de Jira en Miro, marca **Crear un webhook automáticamente**.
    > *✏️ Puedes agregar el webhook manualmente más tarde.*
13. Haz clic en **Conectar**.
14. Sigue el flujo de autenticación para tu servidor de autorización. Si se te pide, inicia sesión en tu entorno.
    Cuando tu conexión se complete, tu instancia de Jira se listará bajo **Instancias conectadas** con la siguiente etiqueta: **Servidor de autenticación**.

## Asegúrate de que tu equipo pueda autenticarse

Ahora que tienes conectada tu instancia de Jira a nivel organizativo, puedes empezar a usar Jira a nivel de equipo.

1. En tu panel de Miro, selecciona tu avatar en la esquina superior derecha y ve a **Admin console**.
2. Selecciona **Equipos** > **Tu equipo**.
   El control deslizante de **tu equipo** se abre.
3. Selecciona la pestaña **Aplicaciones**.
4. Desde la lista de aplicaciones, selecciona **tarjetas Jira**.
5. En **Configuración de administrador**, verifica si tu configuración de Jira muestra la etiqueta **CONEXIÓN GLOBAL** y la URL correcta de la instancia de Jira, luego haz una de las siguientes cosas:
   - Si es así, has completado este procedimiento. Puedes saltar a [¿Qué sigue?](https://help.miro.com/hc/articles/25699264170386)
   - Si no, selecciona **Cambiar configuración** > **Configuración global de la organización** > **tu instancia de Jira**.
6. Selecciona **Guardar configuración**.

## ¿Ahora qué?

Cada miembro del equipo debe autorizar su cuenta de usuario. Para garantizar que cada usuario obtenga los tokens de acceso y actualización, cuando un miembro del equipo intente realizar una acción relacionada con Jira en un tablero de Miro, se le pedirá que autorice su cuenta.

## Preguntas frecuentes

**¿Qué servidores de autorización puedo usar?**

Puedes usar cualquier servidor de autorización que soporte los protocolos estándar de OAuth 2.0 para entornos locales. Por ejemplo, Azure Active Directory (Entra ID) y Okta.

**¿Puedo usar el mismo servidor de autorización para varias organizaciones?**

Sí, pero debes agregar manualmente el servidor a cada organización.

**¿Puedo actualizar el secreto del cliente para un servidor de autorización?**

No. Si necesitas cambiar el secreto del cliente, entonces debes desconectar y reconectar tu instancia.

**¿Pueden los admins de organización y de equipo seguir usando la autorización nativa en Jira?**

Sí. Dependiendo de la configuración seleccionada, los administradores pueden seguir usando el flujo de autorización nativo en Jira.

**¿Qué pasa si un equipo ya está conectado a otra instancia de Jira?**

Puedes actualizar los equipos a la configuración predeterminada de Jira de tu organización [default Jira settings](https://help.miro.com/hc/articles/26438407676434).

**¿Miro controla el mapeo entre usuarios autorizados y usuarios de Jira?**

No. La vinculación entre los usuarios autorizados y los usuarios de Jira es responsabilidad del entorno del cliente a través de su puerta de enlace API. Miro no controla este portal.

**¿Cómo sé si OAuth 2.0 a través de un servidor de autorización de terceros es la solución adecuada para mi organización?**

Si todos los siguientes elementos son verdaderos, entonces OAuth 2.0 a través de un servidor de autorización de terceros es una buena opción:

- Tu instancia de Jira está alojada en las instalaciones.
- El acceso externo a Jira solo es posible con un gateway de API.
- La puerta de enlace de API aplica la autorización utilizando un servidor de autorización personalizado.
- Debes conectar Miro a Jira sin exponer la URL base pública de Jira.

**¿Qué problema resuelve esta solución?**

Esta solución está diseñada para organizaciones que alojan Jira en sus propias instalaciones y enrutan el tráfico externo de la API a través de una puerta de enlace de API. En esta configuración, Jira no es accesible públicamente y el acceso está controlado mediante un servidor de autorización personalizado. En lugar de tener una URL base pública para Jira, esta solución te permite conectar tus instancias de Jira locales configurando Miro para autenticar a través de tu propio servidor de autorización.
