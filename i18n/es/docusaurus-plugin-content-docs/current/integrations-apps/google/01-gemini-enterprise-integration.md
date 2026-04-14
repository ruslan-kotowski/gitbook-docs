---
title: Integración de Gemini Enterprise (Beta)
article_id: 32304596526482
translation_id: 32304596526482
locale: es
sidebar_position: 1
created_at: '2026-01-05T10:38:04Z'
updated_at: '2026-02-17T09:38:53Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: bring-your-own-ai
availability:
  notes: '¿Quién puede hacerlo?: Admins de empresa ¿Qué planes?: Business, Enterprise
    ¿Qué plataformas?: Navegador, Escritorio'
---

Como admin de empresa, puedes habilitar y configurar la integración de Gemini Enterprise para los equipos de tu organización en Miro.

La integración de Gemini Enterprise te permite conectar Gemini Enterprise como un recurso de [Conocimientos](../../using-miro/miro-ai/09-knowledge.md) en Miro. Por ejemplo, usa Gemini Enterprise para proporcionar inteligencia empresarial a compañeros de IA y flujos.

También puedes conectar Gemini Enterprise a la aplicación de [chat independiente](../../using-miro/miro-ai/09-knowledge.md) en Miro.

Para usar la integración de Gemini Enterprise, sigue estos pasos:

1. Habilitar la aplicación de Gemini Enterprise.
   1. Como admin de empresa, ve a **Consola de administración**.
   2. Ve a **Apps e integraciones** > **Apps** > **Añadir apps**.
   3. Busca y encuentra **Gemini Enterprise**.
      Si no puedes encontrar la aplicación por nombre, entonces busca por el siguiente ID de cliente: `2392210303456548729`.
   4. En el perfil de la aplicación, selecciona si deseas añadir la aplicación para **Todos los equipos en \{Team name\}**, o selecciona **En** **equipos específicos**.
   5. Haz clic en **Añadir**.
2. Configura la aplicación de Gemini Enterprise.
   1. En **Admin Console**, ve a **Apps & integrations** > **Apps**.
   2. Para Gemini Enterprise, asegúrate de que **Permitido** esté activado. Luego haz clic en **Configuración**.
   3. Agrega los detalles de configuración de Gemini Enterprise.
      Para aprender cómo encontrar el Project ID, consulta (Externo) [Localizar el ID del proyecto](https://support.google.com/googleapi/answer/7014113?hl=en).
      Para obtener el App ID, ve a Gemini Enterprise > Apps y utiliza el valor en la columna ID.
      ![](images/33222238720274_image (2).png)
      *Configura la aplicación Gemini Enterprise para su uso en Miro.*

      > ✏️ **Project ID** y **App ID** son necesarios. Los otros campos son opcionales.
   4. Haz clic en **Guardar**.

:::note
Cuando un miembro del equipo conecta Gemini Enterprise como un recurso de [Conocimientos](../../using-miro/miro-ai/09-knowledge.md) por primera vez, se le pedirá autenticarse. El miembro del equipo debe tener una licencia de Gemini Enterprise.
:::
