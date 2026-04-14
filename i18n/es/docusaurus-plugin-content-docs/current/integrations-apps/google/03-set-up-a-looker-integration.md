---
title: "Configura una integraci\xF3n de Looker"
article_id: 25112862440978
translation_id: 25112862440978
locale: es
sidebar_position: 4
created_at: '2025-03-05T14:00:46Z'
updated_at: '2025-06-04T08:30:26Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: looker
---

:::note
Para obtener documentos de administración completos con detalles y más información sobre la integración de Miro y Looker, consulta la [documentación de administración de Looker](https://docs.google.com/document/d/1AUCQWRwDICLygwVmwSxXpz7RmRivPit0EIKgBMIkT6A/edit?usp=sharing).
:::

Para configurar la integración de **Looker** con Miro, debes registrar la aplicación OAuth en Looker.

## Requisitos previos

- Asegúrate de que un **administrador de empresa** haya aprobado Looker para tu organización en Miro.

## Registrar la aplicación OAuth en Looker

1. En el **Looker Marketplace**, encuentra y selecciona la **extensión API Explorer**.
2. Seleccionar **Instalar**.
3. Ve a **Inicio** > **Aplicaciones** > **Extensión de API**.
4. Buscar y seleccionar **Registrar aplicación OAuth**.
5. Seleccionar **Ejecutar**.
6. Se abre un menú donde puedes agregar datos de solicitudes.
   Añade los siguientes valores:
   - **client_guid**: `15609152-a12a-4fa1-b364-337e7896d25d`
   - **cuerpo**:

   ```
     "redirect_uri": "https://integrations.miro.com/api/contenthub/public/oauth/callback"
     nombre_para_mostrar Miro
     Descripción Integración de Miro y Looker
     "habilitado": verdadero,
     "group_id": ""
   }
   ```
7. Selecciona **Entiendo que este endpoint de la API cambiará datos**.
8. Selecciona **Ejecutar**.
9. Una ejecución exitosa devuelve el cuerpo con un código de respuesta **HTTP 200**.
   - 💡 Si el cuerpo devuelto incluye `"enabled":false`, entonces ejecuta la API Update OAuth App con los mismos valores que en el paso 6.

Has configurado correctamente una integración de Looker con Miro.

## Más información

- Consulta la [Referencia de la API de Looker](https://developers.looker.com/api/explorer/4.0/methods/Auth/register_oauth_client_app) (externa).
