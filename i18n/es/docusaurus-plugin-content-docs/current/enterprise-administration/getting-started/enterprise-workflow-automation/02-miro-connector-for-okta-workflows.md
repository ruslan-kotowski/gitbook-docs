---
title: Conector de Miro para Okta Workflows
article_id: 8264504421394
translation_id: 8264504421394
locale: es
sidebar_position: 1
created_at: '2022-10-25T14:04:07Z'
updated_at: '2025-02-26T12:20:37Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: okta-workflows
---

Configura el conector de Miro para Okta Workflows con el fin de usar el conector administrador de Miro desde tu panel de Okta Workflows.

[Obtén más información sobre el conector administrador y el conector de usuario en Cómo configurar la automatización de flujos de trabajo en Okta Workflows.](03-set-up-miro-connectors-for-okta-workflows.md)

> **Disponible para:** plan Enterprise
> **Quién puede hacerlo:** admins de empresa

## Configurar los ajustes en Miro

### Cómo generar un token de acceso

1. En tu página de configuración de Miro Empresa, ve a **Apps e integraciones** > **Integraciones empresariales** y, a continuación, desplázate hasta **Flujos de trabajo de Okta**.

2. 2. Para habilitar **Okta Workflows**, haz clic en la opción de alternar correspondiente.

![okta-workflows-turn-on.pngConfiguración](images/24938361124242_okta-workflows-turn-on.png)
*de los flujos de trabajo de en las integraciones de Miro Enterprise*

3. 3. Para copiar el token de acceso, haz clic en **Copy** (copiar).

4. 4. Para generar un nuevo token de acceso, haz clic en **Generate new token** (generar nuevo token).

![okta-workflows-enablement.pngToken](images/24938336624402_okta-workflows-enablement.png)
*de*

:::warning
Si otro admin de empresa ya habilitó el conmutador, no puedes copiar el token. Solo puedes deshabilitar la integración.
:::

:::warning
La integración está vinculada al equipo con el mayor número de usuarios. No es posible elegir un equipo diferente. Sin embargo, la integración funcionará para todos los equipos de tu plan Enterprise y los eventos importantes para la integración se mostrarán en los registros de auditoría de todo el plan.
:::

## Configurar los ajustes en Okta Workflows

### Cómo crear una nueva conexión

1. 1. En tu panel de Okta Workflows, ve a **Connections** (Conexiones).

2. 2. Haz clic en el botón **+ New Connection** (nueva conexión).

3. 3. En el diálogo **New Connection** (conexión nueva), selecciona **Miro Administrator** (administrador de Miro).

![Miro-Administrator-connection.pngConector](images/21019791302290_Miro-Administrator-connection.png)
*de administración de*

4. 4. Pega el **ID de tu organización** y tu **token de acceso** en los campos de entrada correspondientes en el cuadro de diálogo.

5. **Haz clic en** Create (crear).

![Pegar-org-ID-y-clave-de-acceso-clic-crear.pngCrear](images/21019791303698_Paste-org-ID-and-access-token-click-create.png)
*un nuevo conector*

6. Después de establecer la conexión recién creada, puedes comenzar a crear Okta Workflows.
