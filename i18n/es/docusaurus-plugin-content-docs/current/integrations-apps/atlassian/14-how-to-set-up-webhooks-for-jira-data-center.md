---
title: Cómo configurar webhooks para el Centro de datos de Jira
article_id: 360017731113
translation_id: 8533022542226
locale: es
sidebar_position: 15
created_at: '2022-11-11T19:41:52Z'
updated_at: '2026-01-14T09:25:29Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Personas: Administradores de sistema de Jira Planes: Todos los planes de
    Miro (para la integración con Jira Server/Data Center mediante OAuth 1.0) Plataformas:
    Navegador, aplicación de escritorio (para los procedimientos de configuración)'
---

Para asegurar que tus [tarjetas de Jira](https://help.miro.com/hc/articles/360017572434) en un tablero de Miro se mantengan actualizadas, Miro debe recibir mensajes de Jira cada vez que ocurran cambios de datos. Estos eventos de Jira se transmiten a Miro a través de un webhook.

Esta guía proporciona dos maneras de crear webhooks para Jira Server y Jira Data Center usando OAuth 1.0 y OAuth2.0.

## Crear un webhook automáticamente

Al [configurar tu integración de tarjetas de Jira](https://help.miro.com/hc/articles/360019501754), si te estás conectando al Jira Server o al Jira Data Center, puedes dejar la opción **Crear un webhook automáticamente** activada. Este es el método recomendado.

:::note
La creación automática del webhook requiere que inicies sesión en Jira como Administrador de Sistema de Jira.
:::

![jira-webhooks-server-config.png](../../../../../../docs/integrations-apps/atlassian/images/21304245707026_jira-webhooks-server-config.png)
*Configuración de tarjetas de Jira, Paso 2: "Crear un webhook automáticamente**"** está habilitada*

Después de que el webhook se haya creado automáticamente, es una buena práctica ir a tu página de WebHooks de Jira y editar el webhook para darle un nombre único. Esto es especialmente importante si planeas conectar varios equipos de Miro a tu instancia de Jira.

:::note
Para conexiones OAuth2.0, la conexión del lado de Miro se establece a nivel de empresa. Se crea un webhook para todos los equipos de Miro.
:::

:::note
Para conexiones OAuth 1.0 a nivel de equipo de Miro, se crea un webhook por equipo. A nivel de empresa de Miro, se crea un webhook para todos los equipos.
:::

## Crear un webhook manualmente

Si prefieres o necesitas crear el webhook manualmente, sigue estos pasos.

**Obtén la URL del webhook desde Miro**

1. En la configuración de tarjetas de Jira en Miro (Paso 2, al conectar al Jira Server/Data Center), desmarca la opción de **Crear un webhook automáticamente**.
2. Copia y pega la **URL de Jira** de tu organización y haz clic en **Conectar y guardar configuración**.
   ![jira-webhooks-configure-jira-url-cropped.png](../../../../../../docs/integrations-apps/atlassian/images/21304245708818_jira-webhooks-configure-jira-url-cropped.png)
   *Configuración de tarjetas de Jira, Paso 2: "Crear un webhook automáticamente" está deshabilitado*
3. Permite que la integración se conecte en Jira cuando se te indique.
4. Después de estos pasos, Miro te proporcionará la **URL del WebHook**:
   ![webhook_URL.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016928565010_webhook%20URL.jpg)*URL del WebHook proporcionada por Miro*

:::note
Si no eres un Administrador del Sistema de Jira, copia la **URL del WebHook** proporcionada por Miro y mándasela a tu Administrador del Sistema de Jira para que pueda crear el webhook en Jira utilizando las instrucciones que están a continuación.
:::

**Crear el webhook en Jira**

A continuación se presentan los pasos para crear un webhook en Jira usando la URL obtenida de Miro. También puedes consultar la documentación oficial de Atlassian para [Jira Server](https://developer.atlassian.com/server/jira/platform/webhooks/) y para [Jira Cloud](https://developer.atlassian.com/cloud/jira/platform/webhooks/) (aunque este artículo se centra en Server/Data Center).

1. Para navegar a la página de **WebHooks** en Jira, ve a **Administración de Jira** > **Sistema** > **Avanzado >** **WebHooks** (la ruta exacta puede variar ligeramente dependiendo de tu versión de Jira). Alternativamente, a menudo puedes usar un enlace directo agregando `/plugins/servlet/webhooks` a la URL de tu instancia de Jira (por ejemplo, `https://NombreDeTuInstanciaDeJira/plugins/servlet/webhooks`).
2. Haz clic en **Crear un WebHook** en la esquina superior derecha de la página de WebHooks.
3. Ingresa un **Nombre** descriptivo para el WebHook (por ejemplo, "Webhook de Integración con Miro").
4. Establece el estado del WebHook en **Habilitado**.
5. Pega el **URL del webhook** que copiaste de la configuración de Miro en el campo URL.
   ![system_webhooks.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016941532050_system%20webhooks.jpg)
   *Configuración del sistema de webhooks en Jira*
6. En la sección **Eventos**, bajo **Problema**, selecciona los eventos **actualizado** y **eliminado**.
7. Haz clic en **Crear** para guardar el webhook.
   ![Jira_Webhook_settings.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016941533074_Jira%20Webhook%20settings.jpg)
   *Configuración de eventos de WebHook en Jira*
8. Después de que se haya creado el webhook en Jira, vuelve al **Paso 2** en la configuración de tarjetas de Jira en Miro, asegúrate de que la **URL de Jira** esté correctamente completada y haz clic en **Conectar**.

Ahora el webhook está creado y configurado. Las tarjetas de Jira en tus tableros de Miro se actualizarán automáticamente cuando se realicen cambios en Jira.
