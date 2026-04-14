---
title: Configurar conectores de Miro para Okta Workflows
article_id: 8166481458706
translation_id: 8166481458706
locale: es
sidebar_position: 2
created_at: '2022-10-19T06:52:05Z'
updated_at: '2025-02-26T11:59:06Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: okta-workflows
---

Los conectores de Miro para Okta Workflows te permiten automatizar fácilmente tareas de admin repetitivas y de varios pasos en Miro. Aprende cómo configurar la automatización de flujos de trabajo y simplificar la gestión de usuarios y equipos.

> Relevante para: plan Enterprise

## Conector de gestión de usuarios de Miro

El conector de gestión de usuarios de Miro permite a los clientes empresariales de Miro con SCIM habilitado agregar usuarios a su organización y gestionar las licencias y los estados de los usuarios.

**Autorización del conector de gestión de usuarios de Miro:**

Cuando añadas una tarjeta de gestión de usuarios de Miro a un flujo por primera vez, te pediremos que configures una conexión para tu organización.  Consulta Autorización/span>.

**Tarjetas de acción del conector de gestión de usuarios de Miro:**

|  |  |
| --- | --- |
| **Acción** | **Descripción** |
| Crear usuario | Crea un nuevo usuario. |
| Leer usuario | Busca un usuario existente en una organización mediante email. |
| Actualizar el tipo de licencia de usuario a completa | Actualiza un recurso de usuario existente y cambia su tipo de licencia de usuario a **completa.** |
| Actualizar estado de usuario | Actualiza un recurso de usuario existente, cambiando su estado activo a un valor de verdadero o falso.El conector de Gestión de Usuarios de Miro funciona utilizando tu token SCIM. La gestión de usuarios de Miro solo está disponible para empresas con SSO y SCIM habilitados. |

## Autorización

Puedes crear y gestionar varias conexiones desde **Conexiones** página Conexiones.
Esto es útil si planeas operar con varias organizaciones. Cada conexión del conector de gestión de usuarios /span>de Miro puede vincularse a una sola organización de Miro.

Para habilitar SCIM y obtener un nuevo token, o para copiar un token existente, sigue las instrucciones de [Cómo habilitar SCIM](https://developers.miro.com/docs/how-to-enable-scim).
Para crear una nueva conexión de una tarjeta de acción, haz lo siguiente:

1. Haz clic en **New Connection (nueva conexión)**.
2. Ingresa un **Connection Nickname (apodo de conexión)**.  Recomendamos usar un nombre que represente a la organización.
3. Habilita el aprovisionamiento SCIM desde [la página de integración de Enterprise de Miro siguiendo las](https://developers.miro.com/docs/how-to-enable-scim) instrucciones.
   1. Copia la **URL de base** desde Miro y pégala en el campo **URL de base** en la conexión
   2. Copia el **token de API** desde Miro y pégalo en el campo **Access Token** (Token de acceso) en la conexión.
4. Haz clic en **Create (crear)**.  Esto te ahorra la conexión y te lleva de nuevo a tu flujo.

### Crear usuario

Crea un usuario dentro de la organización.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| **Detalles de usuario** |  |  |  |
| Correo electrónico | El email del usuario. | String | VERDADERO |
| Activo | El estado del usuario.   - **Verdadero**: el usuario está activo. - **Falso**: el usuario está inactivo.    Cuando no se especifica, el valor predeterminado es **false**. | Dropdown | FALSO |
| Tipo de licencia de usario | El tipo de licencia del usuario.   - **Con acceso completo** - **Gratuita**    Cuando no se especifica, la licencia de usuario se establece de acuerdo con la lógica interna de Miro, que depende del plan de la organización. | Dropdown | FALSO |
| Rol | La función del usuario en la organización.   - **Miembro de la organización**: miembro regular sin privilegios de admin. - **Admin de organización**: usuario con privilegios de admin en toda la empresa.    Cuando no se especifica, el valor predeterminado es **miembro de la organización**. | Dropdown | FALSO |
| **Nombre** |  |  |  |
| Nombre de familia | El nombre de familia o apellido del usuario. | String | FALSO |
| Nombre | El nombre del usuario. | String | FALSO |
| Nombre a visualizar | El nombre que se mostrará en Miro. | String | FALSO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| **Usuario** |  |  |
| ID de usuario | El ID del nuevo usuario. | String |

### Leer usuario

Buscar un usuario existente en una organización mediante correo electrónico

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| **Consulta** |  |  |  |
| Correo electrónico | La dirección de correo electrónico del usuario a buscar | String | VERDADERO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| **Usuario** |  |  |
| ID de usuario | El ID del usuario. | Número |
| Tipo de licencia de usario | El tipo de licencia del usuario. | Número |
| Activo | El estado del usuario.  - **Verdadero**: el usuario está activo. - **Falso**: el usuario está inactivo. | Número |
| **Nombre** |  |  |
| Nombre de usuario | El correo electrónico del usuario. | Número |
| Nombre de familia | El apellido del usuario. | Número |
| Nombre | El nombre del usuario. | Número |
| Nombre a visualizar | El nombre que se muestra en Miro. | Número |

### Actualizar el tipo de licencia de usuario a completa

Actualiza un recurso de usuario existente, ya que se cambia su tipo de usuario (licencia) a **completa**.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| usuario |  |  |  |
| ID de usuario | El ID del usuario. | String | VERDADERO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| **Respuesta** |  |  |
| Código de estado | Estado HTTP de la solicitud.  Códigos que indican una actualización de licencia exitosa:   - 200. OK    Códigos que indican una actualización de licencia incorrecta:   - 400. 400: solicitud con formato incorrecto - 401. 401: sin autorización - 403. 403: prohibido - 404. No encontrado - 409. 409: conflicto - 429. 429: demasiadas solicitudes | Número |

### Actualizar estado de usuario

Actualiza un recurso de usuario existente, ya que cambia su **estado activo** a un valor verdadero o falso.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| usuario |  |  |  |
| ID de usuario | El ID del usuario. | String | VERDADERO |
| Activo | El nuevo estado del usuario.  - **Verdadero**: el usuario está activo. - **Falso**: el usuario está inactivo. | Dropdown | VERDADERO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| **Respuesta** |  |  |
| Código de estado | Estado HTTP de la solicitud.  Códigos que indican una actualización de estado activo exitosa:   - 200. OK    Códigos que indican una actualización de estado activo incorrecta:   - 400. 400: solicitud con formato incorrecto - 401. 401: sin autorización - 403. 403: prohibido - 404. No encontrado - 409. 409: conflicto - 429. 429: demasiadas solicitudes | Número |

## Conector de administración de Miro

El conector de administración de Miro permite a los clientes empresariales crear equipos y gestionar los ajustes y los miembros de los equipos.

**Autorizar tu conector de administración de Miro**:

Cuando añadas una tarjeta Miro a un flujo por primera vez, te pediremos que configures una conexión para tu organización.  Consulta Autorización/span>.

**Tarjetas de acción** **de conector de administación de Miro**:

|  |  |
| --- | --- |
| **Acción** | **Descripción** |
| Crear equipo | Crea un equipo nuevo en una organización existente. |
| Buscar equipos | Busca equipos existentes en una organización.  Los primeros 10 registros coincidentes se seleccionan desde el conjunto de resultados. |
| Añadir un miembro al equipo | Añade un nuevo miembro a un equipo existente. |
| Actualizar función de un miembro del equipo | Actualiza el rol de un miembro del equipo en un equipo existente. |
| Obtener ajustes de equipo | Recupera los ajustes del equipo de un equipo existente. |
| Actualizar los ajustes de las políticas de uso compartido del equipo | Actualiza los ajustes para la política de uso compartido de un equipo existente. |
| Actualizar los ajustes de invitación del equipo | Actualiza los ajustes de la política de invitación de un equipo existente. |
| Actualizar los ajustes de colaboración del equipo | Actualiza los ajustes de la política de colaboración de un equipo existente. |
| Actualizar los ajustes de descubrimiento del equipo | Actualiza los ajustes de la política de descubrimiento de un equipo existente. |
| Actualizar los ajustes de acceso de copia del equipo | Actualiza los ajustes de la política de acceso de copia de un equipo existente. |
| Borrado de sesión de usuario (BETA) | Borra todas las sesiones de usuario de una dirección de correo electrónico determinada. |

## Autorización

El conector de administración de Miro funciona con el token de la API de OAuth.  El conector de administración de Miro solo está disponible para los clientes del plan Enterprise. Para crear una conexión nueva, los usuarios deben tener los permisos necesarios para instalar aplicaciones con los alcances compatibles a continuación.

Puedes crear y gestionar varias conexiones desde **Conexiones** página Conexiones.
Esto es útil si planeas operar con varias organizaciones. Cada conexión del conector de administración de Miro puede vincularse a una sola organización de Miro.

Para crear una nueva conexión de una tarjeta de acción, haz lo siguiente:

1. Haz clic en **New Connection (nueva conexión)**.
2. Ingresa un **Connection Nickname (apodo de conexión)**.  Recomendamos usar un nombre que represente a la organización.
3. Obtén **el ID de la organización** y **el token de acceso** de la página de integración de Enterprise mediante las [instrucciones](02-miro-connector-for-okta-workflows.md).
4. Haz clic en **Create (crear)**.  Esto te ahorra la conexión y te lleva de nuevo a tu flujo.

Alcances admitidos:

- organizations:teams:write
- organizations:teams:read

### Crear equipo

Crea un equipo en una organización existente.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| Equipo: |  |  |  |
| Nombre de equipo | El nombre del equipo. | string | VERDADERO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| **Respuesta** |  |  |
| ID de equipo | El ID del nuevo equipo. | String |

### Buscar equipos

Busca equipos existentes en una organización.  Los primeros 10 registros coincidentes se seleccionan desde el conjunto de resultados.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| **Consulta** |  |  |  |
| Nombre del equipo. | Palabras que deben coincidir con el nombre del equipo.  Cualquier equipo cuyo nombre contenga esas palabras exactas se mostrará como conjunto de resultados. Los equipos con nombres que coinciden completamente con la consulta estarán entre los primeros resultados. | String | FALSO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| **Respuesta** |  |  |
| **Equipos** | Lista con los primeros diez equipos encontrados. Cada equipo tiene los campos que se muestran a continuación. | Lista |
| ID de equipo | El ID del equipo | String |
| Nombre | Nombre del equipo | String |

### Añadir un miembro al equipo

Añade un nuevo miembro a un equipo existente.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| **Team** |  |  |  |
| ID de equipo | El ID del equipo. | String | VERDADERO |
| Miembro |  |  |  |
| Email del usuario | El correo electrónico del usuario que quieres agregar al equipo. | String | VERDADERO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| **Respuesta** |  |  |
| ID de miembro | El ID del nuevo miembro del equipo. | Cadena |

### Actualizar función del miembro del equipo

Actualiza el rol de un miembro del equipo en un equipo existente.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| **Team** |  |  |  |
| ID de equipo | El ID del equipo. | String | VERDADERO |
| Miembro |  |  |  |
| ID de miembro | El ID del miembro del equipo. | String | VERDADERO |
| Rol | La nueva función del miembro en el equipo.  - **Miembro**: miembro regular. - **Admin**: miembro con privilegios de admin en el equipo. - **Invitado al equipo**: invitado con privilegios limitados. | Dropdown | VERDADERO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| **Respuesta** |  |  |
| ID de miembro | El ID del miembro del equipo. | String |
| Rol | La nueva función asignada al miembro del equipo.  - **miembro**: miembro regular. - **admin**: miembro con privilegios de admin dentro del equipo. - **team_guest**: invitado con privilegios limitados. | String |

### Obtener ajustes de equipo

Recupera los ajustes del equipo de un equipo existente.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| Equipo: |  |  |  |
| ID de equipo | El ID del equipo. | String | VERDADERO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| Ajustes de las invitaciones al equipo |  |  |
| Quién puede invitar | - **only_org_admins**: solo los admins de empresa pueden invitar colaboradores. - **admins**: los admins de empresa y los admins de equipo pueden invitar colaboradores. - **all_members**: todos los miembros del equipo pueden invitar colaboradores. | String |
| Invitar usuarios externos | - **allowed**: se admiten colaboradores que no sean miembros del equipo. - **Not_allowed**: no se admiten colaboradores que no sean miembros del equipo. | String |
| Ajustes de colaboración del equipo |  |  |
| Rol de copropietario | - **enabled**: se habilita el rol de copropietario en tableros y proyectos. - **disabled**: se deshabilita el rol de copropietario en tableros y proyectos. | String |
| **Ajustes a nivel de acceso de copia de equipo** |  |  |
| Nivel de acceso de copia | - **anyone**: cualquier persona con acceso al tablero puede copiar el contenido existente en este en tableros recién creados. ATENCIÓN: esta opción sólo está disponible si **Limitación del nivel de acceso para copiar** está establecida en **cualquiera**. - **team_members**: los miembros del equipo pueden copiar contenido del tablero existente en los tableros recién creados. - **team_editors**: los miembros del equipo con derechos de edición pueden copiar el contenido del tablero existente en tableros recién creados. - **board_owner**: solo los propietarios pueden copiar el contenido del tablero existente en tableros recién creados. | String |
| Limitación a nivel de acceso de copia | - **anyone**: los miembros del equipo y los usuarios externos al equipo pueden obtener permiso para copiar el contenido del tablero. - **team_members**: solo los miembros del equipo pueden recibir permiso para copiar el contenido del tablero. | String |
| Ajustes de descubrimiento del equipo |  |  |
| Descubrimiento | - **hidden**: solo los usuarios invitados pueden ver el equipo y acceder a él. - **request**: los miembros de la organización pueden encontrar al equipo y solicitar unirse al equipo con la aprobación del admin. - **join**: los miembros de la organización pueden encontrar y unirse al equipo. | String |
| **Ajustes de política para compartir en equipo** |  |  |
| Acceso predeterminado al tablero | - **Privado**: solo los propietarios pueden acceder a los tableros. - **view**: cualquier persona en el equipo puede ver los tableros. - **comment**: cualquier persona en el equipo puede añadir comentarios a los tableros. - **edit**: cualquier persona en el equipo puede editar tableros. | String |
| Acceso predeterminado a la organización | - **Privado**: solo los propietarios pueden acceder a los tableros. - **view**: cualquier persona en la organización puede ver los tableros. - **Comentar**: cualquier persona en la organización puede añadir comentarios a los tableros. - **edit**: cualquier persona en la organización puede editar tableros. | String |
| Compartir en la organización | - - **allowed**: permite el uso compartido a nivel de la organización. - **allowed_with_editing**: se permite el uso compartido con derechos de edición a nivel de la organización. - **not_allowed**: no se permite el uso compartido a nivel de la organización. | String |
| Compartir en el equipo | - - **Permitido**: se permite el uso compartido a nivel del equipo. - **allowed_with_editing**: se permite el uso compartido con derechos de edición a nivel del equipo. - **No** permitido: no se permite compartir a nivel del equipo. | String |
| Compartir mediante enlace público | - **Permitido**: **se permite el uso compartido mediante enlace público.** - **allowed_with_editing**:se permite compartir con derechos de edición mediante enlace público. - **not_allowed**:no se permite compartir mediante enlace público. | String |
| Mover tablero al equipo | - **allowed**: se permite mover los tableros a un equipo diferente. - **not_allowed**: no se permite mover los tableros a un equipo diferente. | String |

### Actualizar los ajustes de la política de uso compartido del equipo

Actualiza los ajustes para la política de uso compartido de un equipo existente.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| **Team** |  |  |  |
| ID de equipo | El ID del equipo. | String | VERDADERO |
| Acceso predeterminado al tablero | - **Privado**: solo los propietarios del tablero pueden acceder a los tableros. - **Ver**: cualquier persona en el equipo puede ver los tableros - **Comentar**: cualquier persona en el equipo puede añadir comentarios a los tableros. - **Editar**: cualquier persona en el equipo puede editar tableros. | Dropdown | FALSO |
| Acceso predeterminado a la organización | - **Privado**: cualquier propietario puede acceder a los tableros. - **Ver**: cualquier persona en el equipo puede ver los tableros - **Comentar**: cualquier persona en el equipo puede añadir comentarios a los tableros. - **Editar**: cualquier persona en el equipo puede editar tableros. | Dropdown | FALSO |
| Compartir mediante enlace público | - **Permitido**: se permite el uso compartido mediante enlace público. - **allowed_with_editing**:se permite compartir con derechos de edición mediante enlace público. - **No permitido**: no se permite compartir mediante enlace público. | Dropdown | FALSO |
| Compartir en el equipo | - **Permitido**: se permite el uso compartido a nivel del equipo. - **allowed_with_editing**: se permite el uso compartido con derechos de edición a nivel del equipo. - **No** permitido: no se permite compartir a nivel del equipo. | Dropdown | FALSO |
| Compartir en la organización | - **allowed**: permite el uso compartido a nivel de la organización. - **allowed_with_editing**: se permite el uso compartido con derechos de edición a nivel de la organización. - **not_allowed**: no se permite el uso compartido a nivel de la organización. | Dropdown | FALSO |
| Mover tablero al equipo | - **Permitido:** se permite mover tableros a un equipo diferente. - **No permitido** no se permite mover tableros a un equipo diferente. | Dropdown | FALSO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| **Ajustes de política de uso compartido del equipo** |  |  |
| Acceso predeterminado al tablero | - **Privado**: solo los propietarios pueden acceder a los tableros. - **view**: cualquier persona en el equipo puede ver los tableros. - **comment**: cualquier persona en el equipo puede añadir comentarios a los tableros. - **edit**: cualquier persona en el equipo puede editar tableros. | String |
| Acceso predeterminado a la organización | - **Privado**: solo los propietarios pueden acceder a los tableros. - **view**: cualquier persona en la organización puede ver los tableros. - **comment**: cualquier persona en la organización puede añadir comentarios a los tableros. - **edit**: cualquier persona en la organización puede editar tableros. | String |
| Compartir en la organización | - - **allowed**: permite el uso compartido a nivel de la organización. - **allowed_with_editing**: se permite el uso compartido con derechos de edición a nivel de la organización. - **not_allowed**: no se permite el uso compartido a nivel de la organización. | String |
| Compartir en el equipo | - - **Permitido**: se permite el uso compartido a nivel del equipo. - **allowed_with_editing**: se permite el uso compartido con derechos de edición a nivel del equipo. - **No** permitido: no se permite compartir a nivel del equipo. | String |
| Compartir mediante enlace público | - - **Permitido**: se permite el uso compartido mediante enlace público. - **allowed_with_editing**:se permite compartir con derechos de edición mediante enlace público. - **not_allowed**:no se permite compartir mediante enlace público. | String |
| Mover tablero al equipo | - **allowed**: se permite mover los tableros a un equipo diferente. - **not_allowed**: no se permite mover los tableros a un equipo diferente. | String |

### Actualizar los ajustes de invitación del equipo

Actualiza los ajustes de la política de invitación de un equipo existente.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| **Team** |  |  |  |
| ID de equipo | El ID del equipo. | String | VERDADERO |
| Invitar usuarios externos | - **Permitido**: se admiten colaboradores que no sean miembros del equipo. - **No permitido:** no se admiten colaboradores que no sean miembros del equipo. | Dropdown | FALSO |
| Quién puede invitar | - **Solo los admins de la organización**: solo los admins de la empresa pueden invitar colaboradores. - **Admins**: los admins de empresa y los admins de equipo pueden invitar colaboradores. - **Todos los miembros**: todos los miembros del equipo pueden invitar colaboradores. | Dropdown | FALSO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| **Ajustes de las invitaciones al equipo** |  |  |
| Invitar usuarios externos | - **allowed**: se admiten colaboradores que no sean miembros del equipo. - **Not_allowed**: no se admiten colaboradores que no sean miembros del equipo. | String |
| Quién puede invitar | - **only_org_admins**: solo los admins de empresa pueden invitar colaboradores. - **admins**: los admins de empresa y los admins de equipo pueden invitar colaboradores. - **all_members**: todos los miembros del equipo pueden invitar colaboradores. | String |

### Actualizar los ajustes de acceso de copia del equipo

Actualiza los ajustes de la política de acceso de copia de un equipo existente.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| **Team** |  |  |  |
| ID de equipo | El ID del equipo. | String | VERDADERO |
| Nivel de acceso de copia | - **anyone**: cualquier persona con acceso al tablero puede copiar el contenido existente en este en tableros recién creados. - **Miembros del equipo**: los miembros del equipo pueden copiar contenido del tablero existente a los tableros recién creados. - **Editores del equipo**: los miembros del equipo con derechos de edición pueden copiar el contenido del tablero existente a tableros recién creado. - **board_owner**: solo los propietarios pueden copiar el contenido del tablero existente en tableros recién creados. | Dropdown | FALSO |
| Limitación a nivel de acceso de copia | - **Cualquier persona**: los miembros del equipo y los usuarios externos al equipo pueden obtener permiso para copiar el contenido del tablero. - **Miembros del equipo**: solo los miembros del equipo pueden recibir permiso para copiar el contenido del tablero. | Dropdown | FALSO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| **Ajustes de acceso de copia del equipo** |  |  |
| Nivel de acceso de copia | - **anyone**: cualquier persona con acceso al tablero puede copiar el contenido existente en este en tableros recién creados. - **team_members**: los miembros del equipo pueden copiar contenido del tablero existente en los tableros recién creados. - **team_editors**: los miembros del equipo con derechos de edición pueden copiar el contenido del tablero existente en tableros recién creados. - **board_owner**: solo los propietarios del tablero pueden copiar el contenido existente en este en tableros recién creados. | String |
| Limitación a nivel de acceso de copia | - **anyone**: los miembros del equipo y los usuarios externos al equipo pueden obtener permiso para copiar el contenido del tablero. - **team_members**: solo los miembros del equipo pueden recibir permiso para copiar el contenido del tablero. | String |

### Actualizar los ajustes de colaboración del equipo

Actualiza los ajustes de la política de colaboración de un equipo existente.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| **Team** |  |  |  |
| ID de equipo | El ID del equipo. | String | VERDADERO |
| Rol de copropietario | - **Habilitado**: se habilita el rol de copropietario en tableros y proyectos. - **Deshabilitado**: se deshabilita el rol de copropietario en tableros y proyectos. | Dropdown | FALSO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| **Ajustes de colaboración del equipo** |  |  |
| Rol de copropietario | - **enabled**: se habilita el rol de copropietario en tableros y proyectos. - **disabled**: se deshabilita el rol de copropietario en tableros y proyectos. | String |

### Actualizar los ajustes de descubrimiento del equipo

Actualiza los ajustes de la política de descubrimiento de un equipo existente.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| **Team** |  |  |  |
| ID de equipo | El ID del equipo. | String | VERDADERO |
| Descubrimiento | - **Oculto**: solo los usuarios invitados pueden ver y acceder al equipo. - **Solicitud**: los miembros de la organización pueden encontrar al equipo y solicitar unirse al equipo con la aprobación del admin. - **Unirse**: los miembros de la organización pueden encontrar y unirse al equipo. | Dropdown | FALSO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| **Ajustes de descubrimiento del equipo** |  |  |
| Descubrimiento | - **hidden**: solo los usuarios invitados pueden ver el equipo y acceder a él. - **request**: los miembros de la organización pueden encontrar al equipo y solicitar unirse al equipo con la aprobación del admin. - **join**: los miembros de la organización pueden encontrar y unirse al equipo. | String |

### Borrado de sesión de usuario

Borra todas las sesiones de usuario de una dirección de correo electrónico determinada.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definición** | **Tipo** | **Requerido** |
| Detalles de usuario |  |  |  |
| Correo electrónico | La dirección de correo electrónico del usuario cuyas sesiones se van a borrar. | String | VERDADERO |

Salida

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definición** | **Tipo** |
| **Respuesta** |  |  |
| Código de estado | Estado HTTP de la solicitud.   Códigos que indican que se ha actualizado correctamente la sesión de usuario:   - 200. Sesión de usuario eliminada    Códigos que indican una actualización fallida del borrado de sesión de usuario:   - 400. 400: solicitud con formato incorrecto - 401. 401: sin autorización - 403. 403: prohibido - 404. No encontrado - 409. 409: conflicto - 429. 429: demasiadas solicitudes | Número |
