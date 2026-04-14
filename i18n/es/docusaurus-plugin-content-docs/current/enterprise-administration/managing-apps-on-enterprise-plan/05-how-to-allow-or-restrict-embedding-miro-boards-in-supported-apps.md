---
title: "C\xF3mo permitir o restringir la inserci\xF3n de los tableros de Miro en las\
  \ aplicaciones compatibles"
article_id: 4405088016274
translation_id: 4405088016274
locale: es
sidebar_position: 5
created_at: '2021-08-13T05:51:25Z'
updated_at: '2025-11-25T16:06:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: live-embed
---

Miro tiene varias integraciones que permiten a los usuarios compartir fácilmente un tablero en todas las aplicaciones externas como [Zoom](../../integrations-apps/zoom/02-miro-app-for-zoom-user-guide.md), [Microsoft Teams](../../integrations-apps/microsoft/microsoft-teams/05-embed-miro-boards-in-microsoft-teams.md), [Jira](../../integrations-apps/atlassian/02-miro-for-jira-cloud.md), [Confluence](../../integrations-apps/atlassian/01-miro-for-confluence.md) y [otras](https://miro.com/marketplace/category/embed-miro/).  Los administradores de Enterprise pueden permitir o restringir la inserción de tableros en las aplicaciones compatibles.

> **Relevante para: plan Enterprise**

### Insertar tableros de Miro en las aplicaciones compatibles

Cuando insertas un tablero de Miro en una aplicación compatible, puedes otorgar acceso al tablero a los usuarios de la aplicación, incluso si no tienen perfiles de Miro.

Compartir un tablero dentro de una aplicación compatible no afecta tus ajustes de uso compartido en Miro.  Obtén más información sobre el acceso a los tableros insertados en las aplicaciones compatibles/span>[.](../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md)

![allow_restrict_embed_personalizar_embed.gif](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/21019705471122_allow_restrict_embed_customize_embed.gif)*Insertar un tablero de Miro con acceso restringido*

### Cómo restringir o permitir la inserción de tableros en las aplicaciones compatibles

> **Quién puede hacerlo:** admins de empresa

Los admins de empresa en el plan Enterprise pueden configurar la capacidad de insertar tableros de Miro en aplicaciones compatibles**.**  Con esta configuración activada, los usuarios pueden insertar sus tableros de Miro, incluso si el uso compartido público está restringido en tu organización o equipos/strong>.

Para permitir o restringir el uso compartido con usuarios que no hayan iniciado sesión en aplicaciones compatibles:

1. Ve a **Configuración de** **la organización**.
2. En **Seguridad**, haz clic en **Compartir**.
3. Desplázate hasta la sección Contenido y activa/desactiva **Permitir compartir mediante insertar**.

:::note
Obtén más información sobre [el acceso a tableros insertados para usuarios con licencias gratuitas limitadas](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).
:::

![allow-embedding.pngPermitir](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803639826_allow-embedding.png)
*compartir mediante insertar en el plan Enterprise*

Si desactivas la configuración, los tableros previamente insertados dejarán de estar disponibles. Sigue siendo posible insertar tableros nuevos, pero precisará que cada visitante tenga acceso.

Los usuarios tienen una vista completa de todas las aplicaciones donde un tablero específico se ha insertado con la capacidad de revocar el acceso en cualquier momento, todos desde los ajustes de uso compartido del tablero. Obtén más información sobre cómo administrar y revocar el acceso a los tableros insertados/span>[.](../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md)

### ¿Los tableros insertados en aplicaciones compatibles pueden estar protegidos por una contraseña?

En la configuración de la empresa, los admins tienen la opción de exigir contraseñas para los tableros de Miro que se comparten mediante un enlace público.

Cuando [compartes un tablero mediante un enlace público con una contraseña en Miro](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), estos ajustes no se reflejan en los tableros insertados en las aplicaciones compatibles.  La protección con contraseña no es obligatoria cuando insertas un tablero en Microsoft Teams, Zoom/span> [u otras aplicaciones.](../../integrations-apps/microsoft/microsoft-teams/05-embed-miro-boards-in-microsoft-teams.md)

En lugar de eso, garantizamos que el acceso a un tablero insertado solo está disponible en la aplicación compatible y no se proporciona fuera de la aplicación (por ejemplo, en un navegador web), a menos que el tablero se [comparta desde Miro](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).
