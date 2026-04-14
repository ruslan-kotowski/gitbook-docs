---
title: Permisos de equipo en el plan Enterprise
article_id: 4402822899986
translation_id: 4402822899986
locale: es
sidebar_position: 10
created_at: '2021-06-24T12:51:56Z'
updated_at: '2026-02-19T16:30:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: board-roles-and-permissions
---

El plan Enterprise ofrece ajustes de permisos avanzados y te permite configurar fácilmente el nivel de acceso y seguridad necesarios para tus equipos. Puedes seleccionar el descubrimiento de equipos, los ajustes de invitaciones, los ajustes para compartir y los ajustes de contenido del tablero para cumplir con las necesidades y políticas de tu empresa. Los ajustes están configurados para cada equipo bajo la suscripción a Enterprise.

> [✏️ Al crear un nuevo equipo dentro de una subscripción Enterprise, los admins de empresa pueden seleccionar los ajustes de permisos predeterminados o elegir un equipo para copiar sus permisos.](09-create-a-new-team-on-enterprise-plan.md)  Más información sobre los ajustes predeterminados a continuación.

> **Disponible para: plan Enterprise
> **Configurado por:** admins de empresa, admins de equipo**

## Cómo acceder a los permisos y ajustes del equipo

En el panel de Miro, en la parte superior izquierda, selecciona tu avatar. A continuación, selecciona **Configuración** para abrir la consola de admin.

En la consola de admin, selecciona **Equipos**. A continuación, selecciona el equipo que quieras configurar. Se abre la vista de equipo. A continuación, selecciona **Configuración**.

:::tip
Para encontrar a tu equipo, puedes utilizar la barra de búsqueda situada en la parte superior de la vista **Equipos**.
:::

La primera configuración es **Configuración de descubrimiento de equipos**.

![Configuración del descubrimiento de equipos en la consola de admins de empresas](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921781883666_image.png)

*Ajustes de descubrimiento de equipos en la consola de admin de empresas.*

Puedes hacer que tus equipos estén abiertos para que otros usuarios Enterprise puedan unirse a él o bien ocultarlo; obtén más información en el artículoGestiona la privacidad y el descubrimiento de equipos en el plan Enterprise. Los admins de empresa y los admins de equipo pueden cambiar los ajustes si se les permite invitar a nuevos miembros al equipo.

**La configuración de las invitaciones de equipo** habilita a los admins de empresa a determinar quién puede invitar usuarios al equipo y a elegir si necesitas [invitados](../../using-miro/sharing-boards/07-collaboration-with-guests.md) en el equipo.

![Ajustes de invitación de equipo en la consola de admins de empresas](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921781883666_image.png)

*Configuración de la invitación de equipo en la consola de admins de empresas*

**Para más información:** Consulta [Gestionar invitaciones de usuarios en el plan Enterprise](../user-management/05-manage-user-invitations-on-enterprise-plan.md).

Los admins de empresa también pueden configurar **los ajustes de Compartir**.

En primer lugar, puedes definir quién puede crear nuevos contenidos (tableros, Espacios y plantillas) en el equipo y mover tableros al equipo. Esto resulta muy útil si tienes que establecer un equipo especial para el [aprovisionamiento automático](../user-management/13-user-provisioning-on-enterprise-plan.md) o usar un equipo como almacenamiento para ciertos tableros. Puedes permitir esto para todos los miembros, solo para los administradores de la empresa o para los administradores de la empresa y los administradores del equipo.

![Compartir ajustes en la consola de admins de Enterprise](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921781883666_image.png)*Compartir ajustes en la consola de admins de Enterprise*

Puedes permitir o prohibir a los miembros del equipo que compartan tableros y Espacios con todo el equipo, con toda la empresa o a través de enlaces públicos. Si restringes estas formas de compartir, las opciones se eliminarán de los tableros del equipo.

![Compartir tableros en la consola de admins de empresas](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921781883666_image.png)
*Compartir tableros en la consola de admins de empresas*

También es posible configurar [**Compartir** para el equipo tableros y Espacios recién creados](../../using-miro/sharing-boards/11-default-sharing-settings.md). Tanto los admins de empresa como los admins de equipo tienen acceso a los ajustes.

> **⚠️ La opción [Anyone at company can find and view/comment](07-team-management-on-enterprise-plan.md) (Cualquier persona en la empresa puede encontrar y ver o comentar) no se muestra si Team privacy (Privacidad del equipo) está habilitada.**

**Para más información:** Consulta la [Política de compartir en el plan Enterprise](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

Los administradores de la empresa pueden establecer los dominios permitidos para un equipo.

Los admins de empresa pueden ver la configuración para [restringir o permitir el movimiento de tableros desde y hacia el equipo](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md). ![Dominios permitidos para el equipo en la consola de admins de la empresa](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921781883666_image.png)
*Dominios permitidos para el equipo en la consola de admins de la empresa*

Los admins de empresa y de equipo pueden configurar los ajustes de **seguridad del contenido** para un equipo: elige si los usuarios ajenos al equipo deben poder copiar el contenido de los tableros (así como duplicar los tableros del equipo y descargar el contenido de los tableros) y decide para quién debe estar disponible esta opción en los tableros de nueva creación (a menos que el propietario del tablero seleccione otra opción).

![Seguridad de contenidos en la consola de admins de las empresas](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921781883666_image.png)
*Seguridad de contenidos en la consola de admins de la empresa*

Como parte de la configuración de seguridad del contenido, los admins de empresa y de equipo también pueden configurar una etiqueta predeterminada para los tableros recién creados en el equipo, o **clasificación de tableros**. La etiqueta predeterminada del equipo anulará la etiqueta predeterminada de la empresa configurada en los ajustes de clasificación del tablero de la empresa.

Al final de la página, verás la sección deCollaboration settings (Ajustes de colaboración).  Aquí, los administradores de la empresa y del equipo pueden habilitar el rol de copropietario del tablero, que está deshabilitado de forma predeterminada. Ten en cuenta que la opción se verá de color gris si el rol no está habilitado a nivel de la empresa.  [Obtén más información](../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md).

![Clasificación de tableros y configuración de la colaboración en la consola de admins de la empresa](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921781883666_image.png)
*Clasificación de tableros y configuración de la colaboración en la consola de admins de la empresa*

### Ajustes predeterminados

Si eliges los ajustes de permisos **predeterminados** cuando creas [un nuevo equipo Enterprise](09-create-a-new-team-on-enterprise-plan.md), estarás eligiendo los siguientes ajustes:

- **Ajustes de descubrimiento del equipo**: los miembros pueden sumarse después de la aprobación
- **Ajustes de las invitaciones**: todos los miembros del equipo pueden invitar a usuarios nuevos y están permitidos los colaboradores invitados
- **Ajustes para compartir**:
  - Todos los miembros del equipo pueden crear **recursos en este equipo**
  - **Uso compartido del tablero**: los miembros del equipo pueden compartir su contenido con el equipo para ver, comentar, editar y compartir con toda la empresa para ver y comentar, y de forma pública para ver y comentar (si [la opción de compartir públicamente está habilitada a nivel de la](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md) empresa)
  - **Ajustes para el uso compartido del tablero**: solo pueden acceder los propietarios de tableros
  - **Ajustes para compartir Espacios**: sólo pueden acceder los propietarios de Espacios
  - **Dominios permitidos para el equipo**: la opción de alternar para restringir dominios permitidos está desactivada. [Se aplican los dominios permitidos configurados a nivel](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md) de la empresa
- **Mover tableros a otros equipos**: permitido
- **Ajustes de contenido del tablero**
  - **Copiar contenido del tablero**: permitido para los miembros del equipo y los usuarios externos al equipo
  - **Función predeterminada de copia de los tableros**: los miembros del equipo con derechos de edición pueden copiar el contenido del tablero en tableros recién creados
- **Clasificación de tableros; la opción de** anular la etiqueta está desactivada
- **Ajustes de colaboración: el rol del copropietario está desactivado**
