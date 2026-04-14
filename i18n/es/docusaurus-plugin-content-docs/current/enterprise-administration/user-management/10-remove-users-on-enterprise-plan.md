---
title: "Eliminaci\xF3n de usuarios de un plan Enterprise"
article_id: 360017730193
translation_id: 360017730193
locale: es
sidebar_position: 10
created_at: '2019-02-11T10:09:21Z'
updated_at: '2025-11-04T11:30:33Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-management
---

La gestión de usuarios avanzada en Miro permite a los admins filtrar y gestionar fácilmente a todos los usuarios en un solo lugar. Como admin, puedes eliminar usuarios adicionales en cualquier momento.

> **Disponible para: plan Enterprise**

### Cómo eliminar un usuario de un equipo

Para eliminar a un usuario de un equipo concreto de tu suscripción para empresas, abre la Configuración del equipo pasando el ratón por encima del nombre del equipo en el panel y haciendo clic en el icono **Miembros del equipo**.

Se abrirá la pestaña **Usuarios**. Busca al miembro del equipo que quieras eliminar y selecciona **Eliminar del equipo** en el menú de **tres puntos** (**...**).

![borrar-usuarios-del-equipo.png](../../../../../../docs/enterprise-administration/user-management/images/23921781390482_delete-users-from-team.png)

Eliminar a un usuario de un equipo

Ten en cuenta que eliminar a un usuario de un equipo no lo elimina completamente de la organización Enterprise y no libera una licencia. Para eliminar a un usuario de la organización (empresa), sigue estos pasos.

También puedes seleccionar a varios usuarios o hasta 50 usuarios de un equipo a la vez y eliminarlos de manera masiva.

### Cómo eliminar a un usuario de la empresa

:::warning
Antes de eliminar usuarios, comprueba si has habilitado la configuración [Bloquear usuarios desactivados](02-block-deactivated-users.md). Los usuarios eliminados reciben un trato distinto al de los usuarios desactivados.
:::

Para eliminar completamente a un usuario de tu cuenta Enterprise, primero tienes que [desactivarlo](01-deactivated-users.md) en **la sección** Active users (usuarios activos) de **los ajustes** de la empresa. Después abre la pestaña  **Usuarios desactivados** y elige **Eliminar** en el menú de **tres puntos** (**...**) de la fila del usuario.

También puedes seleccionar de manera masiva hasta 50 usuarios y eliminarlos todos a la vez.

Si el usuario es el propietario de algunas [plantillas](../../getting-started/start-here/your-first-board/04-templates.md) de tableros o [proyectos](../../using-miro/sharing-boards/16-projects.md) creados en el plan Enterprise, tendrás la posibilidad de elegir a quién se le reasignará el contenido (puedes seleccionar un admin o a un usuario que no sea admin). Si eliges **Delete user and content** (eliminar el usuario y el contenido), se eliminará el contenido del usuario. Los admins podrán [restaurar los tableros eliminados](../../using-miro/managing-boards/08-how-to-restore-a-deleted-board.md) en el transcurso de los 30 días posteriores a la eliminación.

El usuario eliminado perderá todo acceso a los recursos de tu plan de inmediato (sin recibir una notificación). Ten en cuenta que conservarán el acceso a los tableros que se compartieron [con un enlace público,](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartir-tableros-a-traves-de-un-enlace-publico) si el usuario guardó los enlaces a esos tableros específicos.

Si eliminas a un usuario gestionado de tu suscripción Enterprise, se contará como [no capturado](../canvas-25-admin-features/domain-control/01-domain-control.md) en la Configuración de Control de dominio.
