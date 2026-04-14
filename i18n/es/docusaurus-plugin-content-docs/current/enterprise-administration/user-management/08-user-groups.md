---
title: Grupos de usuarios
article_id: 30658859384594
translation_id: 30658859384594
locale: es
sidebar_position: 8
created_at: '2025-10-30T13:00:25Z'
updated_at: '2026-01-20T13:17:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: groups
availability:
  notes: 'Quién puede hacerlo: (Configuración) Admins de empresa, Miembros del equipo
    Qué planes: Enterprise Qué plataformas: Navegador, Escritorio, Móvil'
---

Como admin de empresa, los Grupos de Usuarios te permiten gestionar el acceso al contenido para grupos de usuarios, en lugar de compartir con cada miembro individualmente. Todos los miembros de tu organización pueden ver y compartir su contenido con los Grupos de Usuarios que crees.

Este artículo explica cómo crear, gestionar y compartir contenido con los Grupos de Usuarios. Para obtener información más general sobre la funcionalidad, consulta la [visión general de Grupos de Usuarios](07-user-groups-overview.md).

:::note
Para aprender sobre cómo gestionar Grupos de Usuarios a través de SCIM, contacta a tu gerente de Customer Success de Miro o Asistencia.
:::

## Guía para el admin de empresa

### Crear un grupo de usuarios

1. Como admin de empresa, ve a la Consola de administración.
2. Ve a **Usuarios** > **Grupos**.
3. En la parte superior derecha, haz clic en **+ Crear grupo**.
   Se abre el modal **Crear nuevo grupo**.
4. Nombra tu grupo.
5. (Opcional) Añade una descripción para tu nuevo grupo. Puedes añadir o editar la descripción más tarde.
6. Haz clic en **Crear grupo**.
   Tu nuevo grupo se añade a la vista de **Grupos**.

### Agregar usuarios a un Grupo de Usuarios

1. En la Consola de Administración, ve a **Usuarios** > **Grupos**.
2. Para el Grupo de Usuarios que quieres gestionar, selecciona los tres puntos (**...**) al final de la fila.
3. Haz clic en **Agregar usuarios**.
   Se abre el modal **Agregar usuarios**.
4. Para localizar a tus usuarios, busca por nombre o correo.
5. Marca cada usuario que quieras añadir.
6. Haz clic en **Agregar usuarios seleccionados**.
   Cada usuario seleccionado es añadido a tu Grupo de Usuarios.

### Agregar Grupo de Usuarios a equipos

1. En la consola de administración, ve a **Usuarios** > **Grupos**.
2. Para el Grupo de Usuarios que deseas gestionar, selecciona los tres puntos (**...**) al final de la fila.
3. Haz clic en **Agregar a equipos**.
   Se abre el modal **Agregar grupo a equipos**.
4. Para localizar tus equipos, busca por nombre.
5. Marca cada equipo al que deseas que se una tu Grupo de Usuarios.
6. Haz clic en **Agregar**.
   Tu Grupo de Usuarios se ha unido a cada equipo que seleccionaste.

   > ✏️ Los miembros del Grupo de Usuarios tienen acceso para editar todo el contenido en cada equipo que seleccionaste.

### Editar un Grupo de Usuarios

1. En la Consola de Admin, ve a **Usuarios** > **Grupos**.
2. Para el Grupo de Usuarios que deseas gestionar, selecciona los tres puntos (**...**) al final de la fila.
3. Haz clic en **Editar grupo**.
   Se abre el modal de **Editar grupo**.
4. (Opcional) Renombra tu grupo.
5. (Opcional) Añade una descripción para tu nuevo grupo.
6. Haz clic en **Guardar**.

### Eliminar un Grupo de Usuarios

:::warning
La eliminación de un grupo de usuarios no se puede deshacer. Al eliminar un grupo de usuarios, algunos usuarios pueden ser removidos de algunos equipos.
:::

1. En la Consola de Administrador, ve a **Usuarios** > **Grupos**.
2. Para el grupo de usuarios que deseas gestionar, selecciona los tres puntos (**...**) al final de la fila.
3. Haz clic en **Eliminar grupo**.
   Se abre el modal **Eliminar \{nombre del grupo de usuarios\}**.
4. Haz clic en **Eliminar**.
   El grupo de usuarios se elimina de forma permanente.

## Guía del usuario

### Compartir un tablero con un grupo de usuarios

Los miembros del equipo pueden compartir un tablero con cualquier Grupo de Usuarios en su organización. El tablero se comparte con todos los miembros de ese Grupo de Usuarios.

Sigue estos pasos:

1. En un tablero de Miro, en la esquina superior derecha, haz clic en **Compartir**.
   Se abrirá un modal.
2. Introduce el nombre de tu Grupo de Usuarios objetivo.
3. De las opciones autocompletadas, selecciona el Grupo de Usuarios.
4. (Opcional) Actualiza los permisos. Predeterminado: **Puede editar**.
5. (Opcional) Añade un mensaje personalizado.
6. Haz clic en **Enviar invitaciones**.
   Cada usuario del Grupo de Usuarios recibirá una invitación por correo electrónico para acceder a tu tablero.

### Compartir un Espacio con un Grupo de Usuarios

Los miembros del equipo pueden compartir un Espacio con cualquier Grupo de Usuarios en su organización y especificar permisos. El Espacio se comparte con todos los miembros de ese Grupo de Usuarios.

Sigue estos pasos:

1. Desde el panel de Miro, en el Espacio que deseas compartir, haz clic en los tres puntos verticales para abrir el menú de **Opciones**.

   > 💡 Alternativamente, en la barra lateral de Espacios, en la parte superior haz clic en los tres puntos verticales para abrir el menú de **Opciones**.
2. Haz clic en **Compartir**.
   Se abre el modal de **Compartir Espacio '\{Space Name\}'**.
3. Introduce el nombre del Grupo de Usuarios.
4. (Opcional) Actualiza los permisos. Predeterminado: **Puede editar**.
5. (Opcional) Agrega un mensaje personalizado.
6. Haz clic en **Enviar invitaciones**.
   Cada miembro del Grupo de Usuarios recibe una invitación por correo electrónico para acceder a tu Espacio.

:::note
Los miembros añadidos al Grupo de Usuarios tienen acceso a los Espacios compartidos automáticamente. Para los miembros eliminados del Grupo de Usuarios, su acceso se revoca automáticamente.
:::
