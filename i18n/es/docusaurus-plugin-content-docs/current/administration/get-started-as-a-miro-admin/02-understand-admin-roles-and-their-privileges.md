---
title: Entender los roles de admin y sus privilegios
article_id: 14766440626834
translation_id: 14766440626834
locale: es
sidebar_position: 2
created_at: '2023-10-30T19:54:40Z'
updated_at: '2026-02-09T12:56:12Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Asignar roles de administrador predefinidos es una forma fácil de otorgar privilegios a otro usuario en tu organización. Cada rol de administrador concede uno o más privilegios que en conjunto te permiten realizar funciones específicas en Miro.

Actualmente, Miro proporciona cuatro roles de administrador predefinidos a nivel organizativo, a saber, el admin de empresa, admin de usuario, admin de contenido y admin de seguridad.

La siguiente tabla enumera los privilegios asociados a cada rol.

:::note
Esta es una lista en evolución de roles y privilegios. Revisa esta página periódicamente para actualizaciones.
:::

|  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- |
| **Cuenta** | | | | | |
| **Privilegio** | **Funciones** | **Admin de la empresa** | **Admin de usuario** | **Admin de contenido** | **Admin de seguridad** |
| Ver el perfil de la empresa | - Ver la página del perfil de la empresa  - Ver contactos principales  - Ver logotipo de la empresa | ✅ | ❌ | ❌ | ❌ |
| Editar el perfil de la empresa | - Editar el nombre de la empresa  - Editar el logotipo de la empresa  - Editar los contactos principales | ✅ | ❌ | ❌ | ❌ |
| Ver estadísticas | - Ver estadísticas de uso de Miro | ✅ | ❌ | ❌ | ❌ |
| **Gestión de usuarios y equipos** | | | | | |
| **Usuarios** | | | | | |
| **Privilegio** | **Función** | **Admin de Empresa** | **Admin de Usuarios** | **Admin de Contenido** | **Admin de Seguridad** |
| Ver usuarios | - Ver usuarios activos  - Aplicar filtros de usuario  - Ver perfiles de usuario  - Ver usuarios desactivados | ✅ | ✅ | ❌ | ❌ |
| Editar usuarios | - Editar equipos del usuario  - Editar roles, permisos del usuario  - Habilitar/deshabilitar usuarios  - Cambiar membresía (invitado, miembro) | ✅ | ✅ | ❌ | ❌ |
| Ver invitaciones | - Ver invitaciones activas | ✅ | ✅ | ❌ | ❌ |
| Añadir usuarios | - Añadir usuarios a equipos  - Añadir usuarios a la organización | ✅ | ✅ | ❌ | ❌ |
| Eliminar usuarios | - Eliminar usuarios de los equipos  - Eliminar usuarios de la organización | ✅ | ✅ | ❌ | ❌ |
| Ver solicitudes de licencias | - Ver solicitudes de licencias | ✅ | ✅ | ❌ | ❌ |
| Gestionar solicitudes de licencias | - Aprobar solicitudes de licencias  - Rechazar solicitudes de licencias | ✅ | ✅ | ❌ | ❌ |
| **Equipos** | | | | | |
| **Privilegio** | **Funciones** | **Admin de empresa** | **Admin de usuarios** | **Admin de contenido** | **Admin de seguridad** |
| Ver equipos | - Ver todos los equipos en la organización  - Ver a los miembros del equipo  - Ver a los admin de equipo  - Realizar tareas relacionadas con el equipo, como buscar equipos, aplicar filtros, entre otros | ✅ | ✅ | ❌ | ❌ |
| Editar equipos | - Actualizar el nombre del equipo  - Actualizar el logotipo del equipo  - Actualizar los admins de equipo | ✅ | ✅ | ❌ | ❌ |
| **Grupos de usuarios** | | | | | |
| **Privilegio** | **Funciones** | **Admin de empresa** | **Admin de usuarios** | **Admin de contenido** | **Admin de seguridad** |
| Ver grupos | - Ver todos los grupos en la organización | ✅ | ❌ | ❌ | ❌ |
| Editar grupos | - Editar grupos en la organización | ✅ | ❌ | ❌ | ❌ |
| Asignar grupo | - Asignar un usuario a un grupo | ✅ | ❌ | ❌ | ❌ |
| Eliminar grupo | - Eliminar un usuario de un grupo | ✅ | ❌ | ❌ | ❌ |
| **Grupos de facturación** | | | | | |
| **Privilegio** | **Funciones** | **Admin de la compañía** | **Admin de usuarios** | **Admin de contenido** | **Admin de seguridad** |
| Ver grupos de facturación | - Ver todos los grupos de facturación de la organización | ✅ | ❌ | ❌ | ❌ |
| Editar grupos de facturación | - Editar todos los grupos de facturación de la organización | ✅ | ❌ | ❌ | ❌ |
| Asignar al grupo de facturación | - Asignar un usuario a un grupo de facturación | ✅ | ❌ | ❌ | ❌ |
| Eliminar grupo de facturación | - Eliminar un usuario de un grupo de facturación | ✅ | ❌ | ❌ | ❌ |
| **Gestión de Contenidos** | | | | | |
| **Espacios** | | | | | |
| **Privilegio** | **Funciones** | **Admin de empresa** | **Admin de usuarios** | **Admin de contenido** | **Admin de seguridad** |
| Crear espacios | - Crear espacios en la organización | **❌** | **❌** | **✅** | ❌ |
| Editar acceso a espacios | - Editar qué usuarios pueden acceder a los espacios | **❌** | **❌** | **✅** | ❌ |
| Editar espacios | - Editar los nombres y la ubicación de los espacios de la organización | **❌** | **❌** | **✅** | ❌ |
| Eliminar espacios | - Eliminar espacios en la organización | **❌** | **❌** | **✅** | ❌ |
| Crear tableros | - Crear tableros en espacios privados | **❌** | **❌** | **✅** | ❌ |
| **Tableros** | | | | | |
| **Privilegio** | **Funciones** | **Admin de Empresa** | **Admin de Usuarios** | **Admin de Contenido** | **Admin de Seguridad** |
| Ver tableros | - Ver todos los tableros (nombre, descripción, imagen) dentro de la organización | **❌** | **❌** | **✅** | ❌ |
| Crear tableros | - Crear tableros | **❌** | **❌** | **✅** | ❌ |
| Editar acceso a tableros | - Editar qué usuarios pueden acceder a los tableros | **❌** | **❌** | **✅** | ❌ |
| Editar tableros | - Editar todos los tableros en la organización | **❌** | **❌** | **✅** | ❌ |
| Editar la configuración para compartir del tablero | - Actualizar la configuración de uso compartido del tablero | **❌** | **❌** | **✅** | ❌ |
| Ver tableros en la papelera | - Ver todos los tableros en la papelera | **✅** | **❌** | **✅** | ❌ |
| Eliminar tableros | - Eliminar tableros y enviar a la papelera | **✅** | **❌** | **✅** | ❌ |
| Eliminar tableros de la papelera | - Eliminar permanentemente los tableros en la papelera | **✅** | **❌** | **✅** | ç |
| Restaurar tableros de la papelera | - Restaurar tableros de la papelera | **✅** | **❌** | **✅** | ❌ |
| Forzar la eliminación de tableros bajo retención | - Eliminar tableros bajo retención de la papelera | **❌** | **❌** | **✅** | ❌ |
| **Plantillas** | | | | | |
| **Privilegio** | **Funciones** | **Admin de empresa** | **Admin de usuarios** | **Admin de contenido** | **Admin de seguridad** |
| Ver plantillas | - Ver todas las plantillas de la organización | ❌ | ❌ | ✅ | ❌ |
| Editar plantillas | - Eliminar y editar detalles de la plantilla (para editar el contenido de la plantilla, deben compartir el tablero con ellos mismos) | ❌ | ❌ | ✅ | ❌ |
| Editar configuración de uso compartido de plantillas | - Editar la configuración de uso compartido de plantillas de la organización | ❌ | ❌ | ✅ | ❌ |
| **Aplicaciones** | | | | | |
| **Privilegio** | **Funciones** | **Admin de empresa** | **Admin de usuarios** | **Admin de contenido** | **Admin de seguridad** |
| Gestionar aplicaciones permitidas | - Gestionar la lista de admitidos de aplicaciones de la organización | ✅ | ❌ | ❌ | ❌ |
| Gestionar solicitudes de aplicaciones | - Aprobar o rechazar solicitudes para permitir aplicaciones en la organización | ✅ | ❌ | ❌ | ❌ |
| Gestionar la configuración de la aplicación | - Ver y actualizar la configuración de la aplicación a nivel de organización y de equipo. | ✅ | ❌ | ❌ | ❌ |
| **Roles de Admin** | | | | | |
| **Privilegio** | **Funciones** | **Admin de empresa** | **Admin de usuario** | **Admin de contenido** | **Admin de seguridad** |
| Ver roles de admin | - Ver roles de admin  - Ver privilegios de *roles de admin*  - Ver una lista de usuarios que tienen roles de admin asignados | ✅ | ❌ | ❌ | ❌ |
| Asignar roles de admin | - Asignar roles de admin a usuarios | ✅ | ❌ | ❌ | ❌ |
| Eliminar roles de admin | - Eliminar roles de admin de usuarios | ✅ | ❌ | ❌ | ❌ |
| **Gestión de Seguridad** | | | | | |
| **Registros de auditoría** | | | | | |
| **Privilegio** | **Funciones** | **Admin de la empresa** | **Admin de usuarios** | **Admin de contenido** | **Admin de seguridad** |
| Configurar registros de auditoría | - Actualizar el período de retención para los registros de auditoría | ✅ | ❌ | ❌ | ✅ |
| Ver/exportar registros de auditoría | - Ver y exportar registros de auditoría | ✅ | ❌ | ❌ | ✅ |
| **Configuración de autenticación** | | | | | |
| **Privilegio** | **Funciones** | **Admin de empresa** | **Admin de usuarios** | **Admin de contenido** | **Admin de seguridad** |
| Ver la configuración de autenticación | - Ver la configuración y el ajuste de autenticación | ✅ | ❌ | ❌ | ✅ |
| Editar configuración de autenticación | - Editar la configuración y parámetros de autenticación, como añadir un nuevo proveedor de inicio de sesión único (SSO) | ✅ | ❌ | ❌ | ✅ |
| **Configuración de colaboración** | | | | | |
| **Privilegio** | **Funciones** | **Admin de la compañía** | **User Admin** | **Admin de contenido** | **Admin de seguridad** |
| Ver configuración de colaboración | - Ver *configuración de invitación* (lista de admitidos, quién puede invitar, desactivar automáticamente a los invitados) - Ver *configuración de compartir*  (configuración de uso compartido del tablero, insertar) - Ver *configuración de privacidad del equipo* - Ver *configuración de permitir copropietario* - Ver *configuración de restringir el uso compartido de plantillas* | ✅ | ❌ | ❌ | ✅ |
| Editar configuración de colaboración | - Editar *configuración de invitación* (lista de admitidos, quién puede invitar, configuración para desactivar automáticamente a los invitados) - Editar *configuración de uso compartido* (configuración de compartir tableros, insertar) - Editar *configuración de privacidad del equipo* - Editar *configuración de permitir copropietario* - Editar *configuración para restringir compartir plantillas* | ✅ | ❌ | ❌ | ✅ |
| **Dominios administrados** | | | | | |
| **Privilegio** | **Funciones** | **Admin de la empresa** | **Admin de usuarios** | **Admin de contenido** | **Admin de seguridad** |
| Ver dominios gestionados | - Ver todos los dominios reclamados, su estado y configuraciones - Ver la *configuración de usuarios desactivados* | ✅ | ❌ | ❌ | ✅ |
| Editar  dominios administrados | - Agregar dominios - Editar dominios - Eliminar dominios - Verificar dominios - Editar *configuración de usuarios desactivados* | ✅ | ❌ | ❌ | ✅ |
