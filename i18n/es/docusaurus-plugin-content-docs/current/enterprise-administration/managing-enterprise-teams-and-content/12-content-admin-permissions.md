---
title: Permisos de admin de contenido
article_id: 360012777280
translation_id: 360012777280
locale: es
sidebar_position: 13
created_at: '2020-03-26T12:31:39Z'
updated_at: '2025-12-10T12:23:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-admin-permissions
availability:
  notes: 'Disponible para: plan Enterprise'
---

Los permisos de admin de contenido te permiten supervisar todo el contenido dentro de tu suscripción Enterprise. Como admin de contenido, puedes gestionar sin problemas el acceso a los tableros, espacios, secciones y plantillas, y limpiar el panel eliminando tableros, espacios y secciones no utilizados.

### Cómo asignar un rol de admin de contenido

1. Ve a tus [configuración](https://miro.com/app/settings/user-profile/).
2. En **Usuarios**, haz clic en **Roles de admin**.
3. Junto al rol de **admin de contenido**, haz clic en los tres puntos (**…**) y selecciona **Asignar rol** en el menú desplegable.
4. Selecciona el usuario o usuarios a los que deseas conceder derechos de admin de contenido. Puedes seleccionar hasta 50 usuarios.
5. Haz clic en el botón **Asignar** para confirmar tu selección.
6. Para ver todos los usuarios a los que se ha asignado el rol de admin de contenido, haz clic de nuevo en los tres puntos (**…**) y selecciona **Ver usuarios**. Alternativamente, haz clic en cualquier parte de la **barra de Admin de contenido** para ver una lista de usuarios.

Para ver los permisos asignados a los admin de contenido, haz clic en la **barra de Admin de contenido**, cambia a la pestaña **Privilegios** y desplázate hacia abajo para ver todos los permisos de **contenido**.

## Administración de tableros y espacios

Para obtener información detallada sobre los permisos que los admin de contenido tienen en tableros y espacios, consulta la [sección de gestión de contenido en la documentación de roles de admin](../../administration/get-started-as-a-miro-admin/02-understand-admin-roles-and-their-privileges.md).

Adicionalmente, los admin de contenido pueden:

- abrir el diálogo de Compartir y gestionar la configuración para compartir el tablero ([eliminar y cambiar el acceso de los usuarios](../../using-miro/sharing-boards/01-board-access-rights.md), compartir el tablero [con un equipo](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)/un usuario/[empresa](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)/[públicamente](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartir-tableros-a-traves-de-un-enlace-publico))
- cambiar la información del tablero (nombre, descripción, portada)
- mover el tablero a un [espacio](../../using-miro/spaces/01-spaces.md)
- mover el tablero a una sección
- [eliminar el tablero](../../using-miro/managing-boards/07-how-to-delete-a-board.md)
- [descargar la copia de seguridad del tablero](../../using-miro/import-and-export/export/05-how-to-save-board-backup.md)
- configurar [la configuración del contenido del tablero](../../using-miro/sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md)
- configurar [permisos avanzados de compartir tableros](../../using-miro/sharing-boards/02-who-can-share-a-miro-board.md)
- consultar qué usuario creó la [contraseña de un tablero público](../../using-miro/sharing-boards/13-password-protection-for-public-boards.md), y crear, cambiar o eliminar contraseñas para tableros compartidos públicamente
- restaurar cualquier tablero de la [papelera](../../using-miro/managing-boards/08-how-to-restore-a-deleted-board.md).

Los admins de contenido y admins de contenido del equipo pueden mover un tablero a otro equipo donde el propietario del tablero sea miembro. Si el propietario del tablero no es miembro del equipo de destino, puedes [transferir la propiedad del tablero](../../using-miro/managing-boards/05-how-to-transfer-board-ownership.md) a un miembro.

Si no ves un tablero en el panel, esto significa que el tablero no se ha compartido contigo, pero aún puedes encontrarlo: [busca](../../getting-started/start-here/miro-dashboard/03-how-to-search-in-miro.md) en el panel por el nombre del tablero, el propietario del tablero, o la ubicación (equipo). Los tableros que no se hayan compartido contigo aparecerán con un icono de candado junto a su nombre. Para administrar un tablero, haz clic en los tres puntos de la esquina superior derecha.

Cuando intentes abrir un tablero mediante un enlace directo o desde un resultado de búsqueda, recibirás el mensaje **Sin acceso al tablero**. En la parte inferior, verás las opciones para **ver la información del tablero** y **administrar los permisos de acceso**.

:::note
No puedes cambiar la configuración de espacios **privados** de los que **no** eres miembro, ni los verás en la lista de espacios. Si necesitas cambiar la configuración de un espacio privado, pide acceso al propietario del espacio o utiliza [las APIs públicas de Miro](https://developers.miro.com/reference/enterprise-update-project-settings). Puedes cambiar la configuración de los espacios que *ves* en el panel de control*.*
:::

## Administrar plantillas

Puedes cambiar tu configuración de uso compartido de plantillas ([personal, de equipo o de empresa](../../getting-started/start-here/your-first-board/02-custom-templates.md)), editar los detalles de la plantilla (nombre, descripción e imagen de portada) o eliminar una plantilla por completo.

**Cómo administrar plantillas personalizadas**

1. Ve a tu panel y haz clic en **Explorar plantillas** en la esquina superior derecha.
2. Ve a **Plantillas personalizadas** en la navegación izquierda y haz clic en tus **plantillas [Nombre de la empresa]** o **Personal**.
3. Desplázate sobre la plantilla que te gustaría editar y haz clic en los tres puntos (...).
4. Para eliminar la plantilla, haz clic en **Eliminar**.
5. Para gestionar otros detalles de la plantilla, haz clic en **Editar**.
6. El tablero se abrirá. Haz clic en el nombre de la plantilla en el menú del tablero.
7. Añade o edita el **Nombre de la plantilla** y la **Descripción**, selecciona la **Área de vista previa** para la imagen de portada, y cambia la configuración de uso compartido a **Personal**, **Equipo** o **Empresa**.
8. Haz clic en **Guardar cambios**.
