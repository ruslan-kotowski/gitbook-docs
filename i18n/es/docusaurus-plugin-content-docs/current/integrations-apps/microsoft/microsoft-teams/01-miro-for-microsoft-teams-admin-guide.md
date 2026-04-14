---
title: Miro para Microsoft Teams (guía para admins)
article_id: 4406387610002
translation_id: 4406387610002
locale: es
sidebar_position: 1
created_at: '2021-09-09T10:28:14Z'
updated_at: '2025-11-25T16:07:14Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: slack-ms-teams
availability:
  notes: 'Disponible para: Planes gratuitos, Starter, Business, Education, Enterprise
    y todos los planes de Microsoft 365'
---

:::note
Los ajustes de permisos y acceso variarán en función del tipo de plan. Para obtener más información sobre los usuarios externos en Microsoft Teams, consulta [la política de apps de Microsoft](https://learn.microsoft.com/microsoftteams/apps-external-users).
:::

Habilita la integración de Miro en Microsoft Teams para acelerar la colaboración dentro de tu organización. Miro para Microsoft Teams ofrece una serie de experiencias que permiten a los usuarios recibir notificaciones en tiempo real, así como colaborar en tableros de Miro insertados en reuniones, canales, chats e invitaciones de calendario de Teams.

Miro también admite tarjetas adaptables mediante el despliegue de enlaces y extensiones de mensajes de búsqueda, lo que da a los usuarios más contexto en los tableros compartidos y permite una rápida gestión de acceso a los tableros, todo ello sin salir de su espacio de Microsoft Teams.

:::tip
Más información sobre [la integración](..) de Miro con [Microsoft Teams](..).
:::

<iframe allowfullscreen="" frameborder="0" height="315" src="//www.youtube-nocookie.com/embed/6xab9nSnmAA" width="560"> <br/></iframe> *Miro para equipos Microsoft Teams*

## Gestión de aplicaciones

:::warning
Los admins de Microsoft tendrán que habilitar la integración de Miro para Microsoft Teams desde el catálogo de gestión de apps de Microsoft. Los admins de Miro Empresas también tendrán que habilitar la integración desde el panel de gestión de apps de Miro.
:::

### Gestión de apps en Microsoft Teams

Los ajustes pueden variar según la cuenta. Más información sobre [cómo gestionar apps en Microsoft Teams](https://learn.microsoft.com/microsoftteams/manage-apps).

Para asegurarte de que tu organización saca el máximo partido de la integración, instala en bloque y fija la app Miro utilizando [la política de configuración de apps de Microsoft](https://learn.microsoft.com/microsoftteams/teams-app-setup-policies).

### Gestión de aplicaciones en Miro

En la configuración de tu empresa Miro > **Apps**, verás dos apps de Microsoft Teams:

- Miro para Microsoft Teams (integración de fichas): inserta Miro en el Calendario, las reuniones de Teams, los canales y los chats.
- Microsoft Teams (integración de bots) - notificaciones a usuarios

Si desactivas Microsoft Teams (integración de bots), los usuarios ya no recibirán notificaciones de Miro dentro de Microsoft Teams.

![Microsoft-Teams-Bot-Tab-Apps.png](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21017606037010_Microsoft-Teams-Bot-Tab-Apps.png)*apps de Microsoft Teams*

## Comprensión de los ajustes de acceso para compartir tableros

Al añadir un tablero como pestaña en reuniones, invitaciones de calendario, chats y canales, los usuarios pueden definir los permisos adecuados para compartir. Para añadir un tablero como pestaña en Microsoft Teams, visita Añadir Miro como pestaña en Microsoft Teams. Más información sobre la [configuración de acceso a un tablero insertado](../../integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).

### Configuración de ajustes de acceso de tu tablero

Las opciones de ajustes de acceso seguirán los controles de acceso para toda la organización.  Si tienes un uso compartido restringido de las inserciones de tableros en un plan Enterprise, esa opción no estará disponible para los usuarios. Más información en [Gestión de la política de uso compartido de la empresa para insertar integraciones.](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md)

![edición_pública_desactivada.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21017593055506_publi%D1%81%20editing%20is%20turned%20off.jpg)*Ejemplo de cuando el admin de empresa desactiva la edición pública*
