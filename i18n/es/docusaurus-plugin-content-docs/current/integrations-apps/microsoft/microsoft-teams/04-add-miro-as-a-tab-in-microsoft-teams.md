---
title: Añadir Miro como ficha en Microsoft Teams
article_id: 4411292563602
translation_id: 4411292563602
locale: es
sidebar_position: 4
created_at: '2021-12-01T04:50:21Z'
updated_at: '2025-11-25T16:07:47Z'
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

Los usuarios pueden añadir tableros de Miro a las reuniones, canales y eventos de calendario de Microsoft Teams para colaborar sin problemas y compartir el acceso con otros miembros del equipo.
En este artículo aprenderás a utilizar Miro dentro:

- Microsoft Teams Meetings
- Eventos del calendario de Microsoft Teams
- Canales y chats de Microsoft Teams

## Añadir Miro en las reuniones de Microsoft Teams

- Los usuarios que se unen a reuniones en MS Teams vía móvil o tableta solo pueden ver un tablero Miro adjunto y no pueden editarlo ni comentarlo
- Cualquier usuario de Microsoft Teams que haya autorizado la app Miro puede añadir Miro a la reunión. Cualquier usuario de Teams con un perfil de Miro puede compartir un tablero en el centro del escenario
- ⚠️ Microsoft no permite que los usuarios invitados usen aplicaciones en una reunión de Teams. Los usuarios deben iniciar sesión en Teams para usar una aplicación (incluida Miro).

1. Haz clic en el desplegable **Más acciones.**
2. Selecciona **+Añadir una app.**
3. Busca Miro y haz clic en el icono de Miro.
4. Aquí, se te pedirá que te registres o inicies sesión en tu perfil de Miro.
5. Selecciona qué tablero quieres compartir o elige crear un nuevo tablero de Miro en blanco.
6. Establece permisos para el resto de participantes en la reunión y concede o restringe el acceso al tablero. Puedes elegir entre estos tipos de permisos:

- **Cualquiera puede editar** (no es necesario iniciar sesión en Miro)
- **Cualquiera puede comentar** (no es necesario iniciar sesión, no es compatible con tableros ubicados en un equipo Free)
- Anyone can view (Cualquier persona puede comentar); no se requiere inicio de sesión.
- **Privado** (sólo pueden colaborar quienes hayan accedido previamente al tablero)

"**Cualquiera puede editar, comentar o ver**" permite a cualquier persona de tu inquilino de Microsoft Teams acceder al tablero. Esto incluye lo siguiente:

- Otros usuarios de Miro externos a tu organización
- Usuarios que no tienen un perfil de Miro
- Usuarios en tu organización que no han iniciado sesión en Miro

:::note
Los ajustes de uso compartido que se establecen para un tablero en Miro también pueden definir el acceso al tablero dentro de Microsoft Teams. Si el tablero se comparte públicamente en Miro, estará disponible para cualquiera en Microsoft Teams, incluso si has anclado el tablero como [Privado](../../../using-miro/sharing-boards/15-make-a-miro-board-private.md). Sin embargo, si tu tablero es privado en el lado de Miro y lo anclaste con Cualquiera puede ver/comentar/editar, el acceso al tablero en el lado de Miro no se verá afectado. [Obtén más información](../../integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).
:::

:::note
Para los usuarios del plan Enterprise de Miro, los ajustes de acceso seguirán los controles de acceso de toda la organización. Los admins deben habilitar la opción de compartir enlaces públicos para insertarlos en **Configuración de la empresa** > **Seguridad**. Más información en [Gestionar la política de uso compartido de la empresa para insertar integraciones](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
:::

Si necesitas cambiar los derechos de acceso en un tablero integrado, elimina la pestaña y vuelve a añadirla con un nivel de acceso diferente.

Ahora puedes acceder al tablero de Miro en cualquier momento durante la reunión en el tablero específico. Si creas varios tableros, habrá una única pestaña para cada tablero.

Si haces clic en Miro, verás la pestaña emergente de Miro en el lado derecho con el tablero que has adjuntado a esta reunión.

Puedes seleccionar el botón Share-to-Stage (Compartir a escenario) para enviar el tablero a todos los participantes y colaborar juntos al mismo tiempo. Puedes dejar de compartir el tablero en cualquier momento si haces clic en el botón Stop presentation (Detener presentación) en la parte superior.

## Anclar tableros a eventos del calendario de Microsoft Teams

:::note
El calendario de Outlook aún no está soportado.
:::

- ⚠️ Los eventos en el calendario de Teams deben estar guardados y tener al menos un asistente antes que se pueda adjuntar el tablero de Miro a la reunión.
- ⚠️ [No hay manera de eliminar un tablero de Miro desde una invitación a una reunión en Teams (](https://support.microsoft.com/en-gb/office/remove-a-tab-in-microsoft-teams-c18c875c-0738-40ec-a228-61d7eb27f745#:~:text=In%20one%2Don%2Done%20and,the%20tab%20and%20select%20Remove.)artículo de referencia de Microsoft). Los usuarios deben eliminar la invitación y crear una nueva sin el tablero.

1. Primero, programa una nueva reunión en el calendario de Microsoft Teams.  Asegúrate de añadir un nombre a la reunión e invita a los asistentes.
2. Haz clic en **Envía** para compartir la invitación.
3. **Una vez se guarde la reunión, vuelve a hacer clic en la reunión y selecciona** Editar para poder adjuntar un tablero de Miro.
4. Podrás anclar Miro como una pestaña utilizando el signo más en la parte superior de la pantalla**(+**).
5. En la siguiente pantalla, se te instruirá para que añadas la app Miro. Busca Miro en la barra de búsqueda o selecciona Miro si ya lo ves.
6. Selecciona **Añadir** para poder añadir a Miro.
7. Se te pedirá que inicies sesión en tu perfil de Miro dentro de Equipos.
8. Una vez que inicies sesión en Miro, te pediremos que selecciones el tablero al que deseas añadir a la reunión. Puedes buscar y seleccionar un tablero existente o crear uno nuevo en blanco.
9. Aquí, también puedes establecer permisos para el resto de los participantes de la reunión y dar o restringir el acceso al tablero. Luego s**elige Guardar para que puedas adjuntar el tablero de Miro seleccionado a la reunión de Equipos. Puedes elegir entre estos tipos de permisos:**

- **Anyone can edit** (Cualquier persona puede editar); no se requiere inicio de sesión
- **Anyone can comment** (Cualquier persona puede comentar); no se requiere inicio de sesión.
- **Anyone can view** (Cualquier persona puede comentar); no se requiere inicio de sesión.
- **Privado**

## Anclar tableros a canales y chats de Microsoft Teams

> **Rol requerido:** [Propietarios de tableros](../../../using-miro/sharing-boards/01-board-access-rights.md) y [editores de tableros](../../../using-miro/sharing-boards/01-board-access-rights.md) que son miembros del equipo donde está ubicado el tablero.

Puedes anclar tableros a los canales de Microsoft Teams creando una nueva pestaña.

1. Haz clic en el icono más
2. Se abrirá un selector con varias apps.
3. Busca Miro en la lista de apps y selecciónala.
4. Si no estás autorizado en Miro en el mismo navegador o dentro de la app de escritorio, tendrás que iniciar sesión. Haz clic en **Get Started** (Comenzar) e inicia sesión o [regístrate en Miro](../../../getting-started/start-here/02-how-to-register-with-miro.md).
5. Una vez realizada la autorización, verás un selector con tableros de Miro (el selector mostrará los tableros a los que tienes acceso del lado de Miro). Ten en cuenta que puedes estar autorizado en Miro y en Microsoft Teams con diferentes emails.
6. Elige un tablero que quieras agregar a tu canal de Microsoft Teams.  Si eliges un tablero para el cual no tengas el nivel de acceso necesario, verás un mensaje de advertencia.
7. Establece permisos para el resto de participantes en la reunión y concede o restringe el acceso al tablero. Puedes elegir entre estos tipos de permisos:

   - **Cualquier persona puede editar** (no se requiere inicio de sesión)
   - **Cualquier persona puede comentar** (no se requiere inicio de sesión)
   - **Cualquier persona puede ver** (no se requiere inicio de sesión)
   - **Privado**
   > ✏️ Los usuarios de Microsoft Teams que usan Miro en la aplicación móvil de Microsoft Teams pueden ver y comentar en los tableros en función de los permisos establecidos. Para editar tableros, recomendamos mucho a los usuarios que instalen nuestra [aplicación móvil](../../../getting-started/apps-for-devices/08-mobile-app.md) nativa, para la cual hemos optimizado la interfaz de usuario.

   ## Preguntas frecuentes

¿Necesita cada miembro del equipo tener un perfil de Miro para ver los tableros de Miro insertados en Microsoft Teams?

Si eliges **Cualquiera puede ver/comentar/editar** al insertar el tablero, incluso los usuarios no registrados podrán ver/comentar el tablero. Además, si el tablero se [comparte públicamente](../../../using-miro/sharing-boards/08-collaboration-with-visitors.md) del lado de Miro, estará disponible para cualquier persona en Microsoft Teams.

Una vez insertado un tablero, ¿quién tiene la capacidad de cambiar el acceso al tablero en MS Teams (por ejemplo, de "Cualquiera puede ver" a "Privado")?

Nadie puede cambiar el acceso al tablero adjunto, ni siquiera el que lo ha adjuntado. Sin embargo, cualquiera puede hacer clic en **Configuración** en el tablero y, a continuación, elegir otro (o el mismo) tablero para el mismo tablero y seleccionar otro nivel de acceso para el tablero elegido.

Estoy registrado en Miro con dos direcciones de correo electrónico y me gustaría integrar un tablero de Miro desde mi segundo perfil de Miro. ¿Cómo puedo cambiar el perfil de Miro?

El selector muestra los tableros del usuario con el que estás autorizado en Miro en el mismo navegador. Abre Miro en otra pestaña del navegador, cierra la sesión e inicia sesión en tu segundo perfil de Miro.

Si utilizas la app de escritorio de Microsoft Teams, cierra sesión en la app - esto también te cerrará sesión en Miro dentro de la app. A continuación, conéctate a la app e intenta [insertar un tablero](05-embed-miro-boards-in-microsoft-teams.md). Se te pedirá que inicies sesión en Miro y podrás iniciar sesión en otro perfil de Miro.
