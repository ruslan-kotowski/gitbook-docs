---
title: Inserta tableros de Miro en Microsoft Teams
article_id: 360017572514
translation_id: 360017572514
locale: es
sidebar_position: 5
created_at: '2019-02-11T10:13:30Z'
updated_at: '2025-04-24T13:52:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ms-teams
---

Integra tableros de Miro en los canales de Microsoft Teams y compártelos sin dificultades con los miembros del equipo. Mantén tus tableros de Miro a mano y ten la seguridad de que todo tu equipo está en sintonía.

:::note
Comprueba cómo puedes insertar tableros de Miro en las Reuniones de Microsoft Teams: [Miro](01-miro-for-microsoft-teams-admin-guide.md) [para Reuniones](02-miro-for-microsoft-teams-user-guide.md)[de Microsoft Teams (Guía del administrador)](01-miro-for-microsoft-teams-admin-guide.md), [Miro para Reuniones de Microsoft Teams (Guía del usuario)](02-miro-for-microsoft-teams-user-guide.md).
:::

> **Disponible para:** todos los planes de Miro

### Instalar el plugin

Primero, tienes que encontrar **Miro** en **Microsoft Teams Store** o, simplemente, utiliza el [enlace directo](https://teams.microsoft.com/l/app/8216e453-3db5-48ee-a3d6-5122f505c8a3).

:::warning
Ten presente que tu admin de usuarios del lado de Microsoft Teams debe habilitar la aplicación de Miro dentro de tu catálogo de aplicaciones de terceros para Teams.  A menos que Miro esté aprobado, no aparecerá entre las aplicaciones de Microsoft Teams Store listadas.
:::

Haz clic en **Add** (Agregar) para instalar el plugin.

instalación_plugin_Miro.jpg
Instalación del plugin de Miro

Una vez instalado el plugin de Miro, te redirigirán a un chat donde podrás configurar cómo recibir notificaciones de Miro. Para obtener más información, consulta [este artículo](10-miro-notifications-in-microsoft-teams.md).

Sin embargo, en ese momento, ya puedes comenzar a integrar tableros de Miro en un canal de Microsoft Teams sin ninguna configuración adicional.

### Integrar tableros en los canales de Microsoft Teams

> **Configurado por:** [propietarios de tableros](../../../using-miro/sharing-boards/01-board-access-rights.md) y [editores de tableros](../../../using-miro/sharing-boards/01-board-access-rights.md) que sean miembros del equipo donde se encuentra el tablero

Puedes insertar tus tableros en los canales de Microsoft Teams creando una nueva pestaña. Haz clic en el icono más Verás un selector con varias aplicaciones. Busca Miro en la lista de apps y selecciónala. Si no estás autorizado en Miro en el mismo navegador o dentro de la app de escritorio, tendrás que iniciar sesión. Haz clic en **Get Started** (Comenzar) e inicia sesión o [regístrate en Miro](../../../getting-started/start-here/02-how-to-register-with-miro.md).

integrar_en_Ms_teams.gif
El diálogo que te pide que autorices tu perfil de Miro

Una vez realizada la autorización, verás un selector con tableros de Miro (el selector mostrará los tableros a los que tienes acceso del lado de Miro). Ten en cuenta que puedes estar autorizado en Miro y en Microsoft Teams con diferentes emails.

Elige un tablero que quieras agregar a tu canal de Microsoft Teams.

selector_integración_MS_teams.jpg
El selector con tableros de Miro

Ten en cuenta que solo los propietarios de tableros y editores de tableros que sean miembros del equipo pueden insertar tableros de Miro. Si eliges un tablero para el cual no tengas el nivel de acceso necesario, verás un mensaje de advertencia.

no_puedes_integrar_tableros.jpg
El mensaje de advertencia de que tu nivel de acceso no te permite integrar un tablero

A continuación, puedes configurar permisos para el resto de los participantes de la reunión y dar o restringir el acceso al tablero. Puedes elegir entre estos tipos de permisos:

- **Cualquier persona puede editar** (no se requiere inicio de sesión)
- **Cualquier persona puede comentar** (no se requiere inicio de sesión)
- **Cualquier persona puede ver** (no se requiere inicio de sesión)
- **Privado**

nivel_compartir.jpg
Configuración de accesos para un tablero integrado

:::note
Ten presente que la configuración de accesos establecida para un tablero en Miro también puede definir el acceso al tablero dentro de Microsoft Teams. Si el tablero se comparte públicamente en Miro, estará disponible para cualquier persona en Microsoft Teams, incluso si has integrado el tablero como Privado/span>**.**  Sin embargo, si tu tablero es privado del lado de Miro y lo integras con un acceso de tipo Cualquier persona puede ver/comentar/editar, el acceso al tablero en Miro no se verá afectado./span> Más información:
:::

:::note
Para los usuarios del [plan Enterprise](../../../enterprise-administration/user-management/05-manage-user-invitations-on-enterprise-plan.md) de Miro, tu configuración de acceso respetará los controles de acceso de toda la organización, lo que podría implicar que algunas opciones para compartir estén restringidas.  Más información: [Cómo administrar la política de uso compartido de Enterprise respecto de las integraciones insertadas](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
:::

:::warning
La opción **Anyone can comment** [(Cualquier persona puede comentar) no es compatible si integras un tablero ubicado en un equipo Free](../../../plans-billing/miro-plans/09-free-plan.md).
:::

Una vez integrado el tablero, puedes comenzar a interactuar con él de inmediato.

inserción_Miro_en_MS_teams.jpg
Tablero integrado a un canal de Microsoft Teams

> *✏️* Los usuarios de Microsoft Teams que usan Miro en la aplicación móvil de Microsoft Teams pueden ver y comentar en los tableros en función de los permisos establecidos. Para editar tableros, recomendamos mucho a los usuarios que instalen nuestra [aplicación móvil](../../../getting-started/apps-for-devices/08-mobile-app.md) nativa, para la cual hemos optimizado la interfaz de usuario.

Miro_en_MS_Team_en_móvil.jpg
**Tablero de Miro en MS Teams en el móvil: presiona Open in the app (Abrir en la aplicación) para instalar la aplicación móvil nativa de Miro**

### Preguntas frecuentes

1. *¿Necesita cada miembro del equipo tener un perfil de Miro para ver los tableros de Miro insertados en Microsoft Teams?*
   - Si eliges **Cualquiera puede ver/comentar/editar** al insertar el tablero, incluso los usuarios no registrados podrán ver/comentar el tablero. Además, si el tablero se [comparte públicamente](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartir-tableros-a-traves-de-un-enlace-publico) del lado de Miro, estará disponible para cualquier persona en Microsoft Teams.
2. **Una vez insertado un tablero, ¿quién tiene la capacidad de cambiar el acceso al tablero en MS Teams (por ejemplo, de "Cualquiera puede ver" a "Privado")?**
   - Nadie puede cambiar el acceso al tablero adjunto, ni siquiera el que lo ha adjuntado. Sin embargo, cualquiera puede hacer clic en **Configuración** en el tablero y, a continuación, elegir otro (o el mismo) tablero para el mismo tablero y seleccionar otro nivel de acceso para el tablero elegido.
3. *Estoy registrado en Miro con dos direcciones de correo electrónico y me gustaría integrar un tablero de Miro desde mi segundo perfil de Miro.* ¿Cómo puedo cambiar el perfil de Miro?
   - El selector muestra los tableros del usuario con el que estás autorizado en Miro en el mismo navegador. Abre Miro en otra pestaña del navegador, cierra la sesión e inicia sesión en tu segundo perfil de Miro.
   Si utilizas la app de escritorio de Microsoft Teams, cierra sesión en la app - esto también te cerrará sesión en Miro dentro de la app. A continuación, conéctate a la app e intenta [insertar un tablero](#h_5af20ae6-78c0-4e6c-ab20-e4968c89c97f). Se te pedirá que inicies sesión en Miro y podrás iniciar sesión en otro perfil de Miro.
