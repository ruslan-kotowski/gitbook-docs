---
title: Usuarios desactivados
article_id: 360025025894
translation_id: 360025025894
locale: es
sidebar_position: 1
created_at: '2019-06-19T22:16:18Z'
updated_at: '2026-02-19T10:44:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-deactivation
---

La gestión avanzada de usuarios en Miro permite a los admins de empresa desactivar usuarios en lugar de eliminarlos. Los usuarios desactivados quedan en el directorio del plan y se pueden reactivar en cualquier momento.

> **Disponible para**: [Enterprise plan](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Configurado por:** admins de empresa

## Reglas

- Los usuarios desactivados no podrán acceder a tu cuenta Enterprise o a sus funciones.
- Si has habilitado la configuración [Bloquear usuarios desactivados](02-block-deactivated-users.md), al desactivar a un usuario gestionado, se bloquea su inicio de sesión en Miro.
- Los usuarios desactivados ya no podrán usar la opción de inicio de sesión único (SSO) de tu empresa para iniciar sesión, volviendo a los métodos estándar de autenticación.
- Los tableros compartidos y los espacios creados por usuarios desactivados *no* se reasignan a nadie más y siguen estando disponibles para los colaboradores (a menos que durante la desactivación, también elimines al usuario de su equipo. En este caso, los tableros se reasignan a un admin de equipo. Esto generalmente es relevante para las [operaciones SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)).
- Todas las [notificaciones](../../using-miro/managing-your-profile/02-miro-notifications.md) a usuarios desactivados están bloqueadas.
- Otros usuarios no pueden compartir tableros y espacios con usuarios desactivados.
- Los usuarios desactivados no se pueden agregar a los equipos dentro de tu suscripción Enterprise. Los admin de empresa pueden reactivar a los usuarios desactivados al invitarlos como miembros, [obtén más información](05-manage-user-invitations-on-enterprise-plan.md).
- A los usuarios desactivados no se les cobra. Sus licencias se liberan y pueden aplicarse a otro usuario activo.
- Los siguientes atributos no se pueden actualizar para los usuarios desactivados:

|  |
| --- |
| `nombreDeUsuario` |
| `tipoDeUsuario` |
| `roles.valor` |

## Desactivar a un usuario

Puedes desactivar un usuario en cualquier momento. Cuando desactivas a un usuario, pasa de un estado **Activo** a uno **Desactivado** y deja de consumir una licencia. Este cambio también se refleja en las listas de usuarios activos y desactivados en la configuración de **Usuarios**.

Para desactivar a un usuario:

1. Abre la **Configuración** de tu **Compañía**.
2. Selecciona **Todos los usuarios** en el menú de **Usuarios**.
3. Haz clic en el icono de **tres puntos** (**...**) a la derecha de un usuario al que te gustaría desactivar.
4. Haz clic en **Desactivar**.
   ![deactivate-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921781594002_deactivate-users.png)
   *La opción de desactivar un usuario en el plan Enterprise*

   También puedes desactivar usuarios en masa. Selecciona varios usuarios marcando las casillas de la izquierda o aplica filtros y selecciona hasta 50 usuarios filtrados a la vez, luego elige **Desactivar** en **Acciones en masa.**
5. Marca la casilla **Reasignar contenido del usuario** si deseas transferir los tableros, [plantillas](../../getting-started/start-here/your-first-board/02-custom-templates.md) y [espacios](../../using-miro/spaces/01-spaces.md) del usuario. Se debe elegir un nuevo propietario para cada equipo en el que el usuario seleccionado tenía contenido. La reasignación del contenido de los usuarios no se puede deshacer.
   ![deactivate-reassign-content.png](../../../../../../docs/enterprise-administration/user-management/images/23921804187154_deactivate-reassign-content.png)
   *La opción para reasignar el contenido de un usuario al desactivarlo*
6. Selecciona **Desactivar.**

La desactivación de usuarios no elimina sus datos en Miro. Los permisos que tienen se mantendrán y se restaurarán una vez que se reactive a esos usuarios.

:::note
Nota: Para desactivar a un admin de empresa, debes revocar primero sus permisos de admin.
:::

:::note
Si ves una notificación **que diga "El equipo debe tener al menos un admin"** al intentar desactivar a un usuario, significa que el usuario es el *único* admin de uno o más equipos de un plan Enterprise. Para solucionarlo, [invítate a esos equipos](05-manage-user-invitations-on-enterprise-plan.md) y [confiérete derechos de admin de equipo](../../administration/user-management/06-how-to-manage-admin-roles.md). Haz clic en el número de equipos del usuario correspondiente para saber de qué equipos es miembro.
:::

:::note
Si tu empresa utiliza la solución [SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md), también puedes desactivar usuarios a través de tu proveedor de identidad. Cuando un usuario es desactivado vía SCIM, su contenido no se reasigna: la opción de reasignación solo se admite en la UI para esta situación.
:::

### Desactivación automática para invitados

Para los invitados (usuarios originalmente invitados a tus tableros vía un correo electrónico) puedes habilitar la [desactivación automática](03-invitation-settings-on-enterprise-plan.md).

## Reactivar a un usuario

Para reactivar a un usuario:

1. Abre las **configuraciones** de tu **Compañía**.
2. Selecciona **Todos los Usuarios** en el menú de Usuarios y luego la pestaña de **Usuarios desactivados**.
3. Haz clic en el icono de **tres puntos** (...) a la derecha del usuario que deseas reactivar.
4. Selecciona **Reactivar**.
5. Agrega al usuario a equipos si es necesario.
6. Confirma **Reactivar**.

![reactivate-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921804191762_reactivate-users.png)
*Reactivar a un usuario*

Cuando reactivas a un usuario:

- Los usuarios pueden iniciar sesión de inmediato.
- Tendrán acceso a tableros compartidos, tableros de equipo y tableros que hayan creado antes de la desactivación (a menos que los tableros hayan sido reasignados).

:::note
Nota: Solo los admins de empresa pueden reactivar a usuarios desactivados.
:::

### Eliminar permanentemente a un usuario

Para eliminar permanentemente a un usuario desactivado:

1. Abre la **configuración** de tu Compañía.
2. Haz clic en **Usuarios** > **Todos los usuarios** desde el menú.
3. Selecciona la pestaña de **Usuarios desactivados**.
4. Haz clic en el icono de **tres puntos** (**...**) a la derecha del usuario que deseas eliminar.
5. Selecciona **Eliminar**.
   ![delete-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921781612562_delete-users.png)
   *Eliminando un usuario desactivado*
6. Elige si quieres reasignar el contenido del usuario o eliminarlo: elige al nuevo propietario y haz clic en **Eliminar usuario** o selecciona **Eliminar usuario y contenido**.

También puedes eliminar usuarios de forma masiva:

1. Desde la pestaña de usuarios desactivados, haz clic en la casilla junto a los usuarios que deseas eliminar.
2. Haz clic en el botón **Eliminar de la Empresa** en la parte superior.

:::note
Nota: luego de la eliminación, los usuarios pueden ser invitados de nuevo a tu plan como miembros o a un tablero como invitados por cualquier persona que tenga permiso para [agregar nuevos usuarios](05-manage-user-invitations-on-enterprise-plan.md).
:::
