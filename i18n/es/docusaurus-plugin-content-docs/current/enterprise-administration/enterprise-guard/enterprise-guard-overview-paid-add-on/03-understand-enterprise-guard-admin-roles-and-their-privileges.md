---
title: Comprender los roles de admin de Enterprise Guard y sus privilegios
article_id: 15695755655954
translation_id: 15695755655954
locale: es
sidebar_position: 1
created_at: '2023-12-11T18:33:53Z'
updated_at: '2026-03-12T22:21:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Las funcionalidades de Enterprise Guard se controlan a través de privilegios de admin. Estos privilegios pueden ser otorgados mediante roles de admin predefinidos o a través de roles de admin personalizados configurados con los privilegios necesarios.

La siguiente tabla lista los privilegios disponibles para cada función y muestra qué roles de admin predefinidos los incluyen por defecto. Al crear roles de admin personalizados, los admins de empresa pueden asignar estos privilegios para otorgar acceso a funcionalidades específicas de Enterprise Guard.

La siguiente tabla lista los privilegios detallados y el matriz de roles de admin para cada función.

|  |  |  |  |
| --- | --- | --- | --- |
| **Gestión del ciclo de vida del contenido** | | | |
| **Privilegio** | **Admin de gobernanza de datos** | **Admin de contenido sensible** | **Admin de eDiscovery** |
| Ver configuración de la papelera | ✅ | ❌ | ❌ |
| Editar configuración de la papelera | ✅ | ❌ | ❌ |
| Añadir política de retención | ✅ | ❌ | ❌ |
| Editar política de retención | ✅ | ❌ | ❌ |
| Eliminar política de retención | ✅ | ❌ | ❌ |
| Agregar política de eliminación | ✅ | ❌ | ❌ |
| Editar política de eliminación | ✅ | ❌ | ❌ |
| Eliminar política de eliminación | ✅ | ❌ | ❌ |
| **Clasificación de datos** | | | |
| **Privilegio** | **Admin de Gobernanza de Datos** | **Admin de Contenido Sensible** | **Admin de eDiscovery** |
| Ver la configuración de clasificación de datos | ❌ | ✅ | ❌ |
| Editar niveles de clasificación | ❌ | ✅ | ❌ |
| Editar configuración de clasificación automática | ❌ | ✅ | ❌ |
| Editar configuración de barreras de protección de clasificación | ❌ | ✅ | ❌ |
| Editar nivel de clasificación predeterminado | ❌ | ✅ | ❌ |
| **Descubrimiento de datos** | | | |
| **Privilegio** | **Admin de Gobernanza de Datos** | **Admin de Contenido Sensible** | **Admin de eDiscovery** |
| Ver etiquetas de privacidad | ❌ | ✅ | ❌ |
| Activar/desactivar la detección de privacidad de datos | ❌ | ✅ | ❌ |
| Ver recuento de coincidencias: etiquetas de privacidad | ❌ | ✅ | ❌ |
| Ver coincidencias ocultas: etiquetas de privacidad | ❌ | ✅ | ❌ |
| Ver coincidencias completas: etiquetas de privacidad | ❌ | ✅ | ❌ |
| **eDiscovery** | | | |
| **Privilegio** | **Admin de Gobernanza de Datos** | **Admin de Contenido Sensible** | **Admin de eDiscovery** |
| Gestionar la configuración de retenciones legales | ❌ | ❌ | ✅ |
| Ver la configuración de retenciones legales | ❌ | ❌ | ✅ |

*Matriz de privilegios detallados y roles de administrador predefinidos para cada función*

> **NOTA:** Las funcionalidades de Enterprise Guard se pueden otorgar a través de roles de administrador predefinidos o mediante roles de administrador personalizados configurados con los privilegios requeridos.

## Asignar un rol de administrador de Enterprise Guard

:::note
Para asignar un rol de administrador de Enterprise Guard a un usuario, debes ser un **admin de empresa**.
:::

1. Ve a tu **configuración de perfil**:

   - Desde un tablero: **Menú principal > Preferencias > Configuración de perfil**.
   - Desde el panel: Haz clic en tu **avatar** en la esquina superior derecha y haz clic en **Configuración**.
   - Desde la URL: Ve a `https://miro.com/app/settings`, y elige tu **Empresa** de la lista en la esquina superior izquierda.
2. En **Gestión de usuarios**, haz clic en **Roles de admin**.
3. En el panel derecho, encuentra el rol de admin que quieres asignar (por ejemplo, **Gobernanza de Datos**, **Admin de Contenido Sensible** o **eDiscovery Admin**).
4. Haz clic en el **icono de elipsis (…)** junto al rol y selecciona **Asignar rol**.
5. Elige al usuario al que quieres asignar el rol.
6. Desplázate hasta el final de la ventana y haz clic en **Asignar**.

## Roles de admin personalizados para Enterprise Guard

Los roles de admin personalizados permiten a los admins de empresa otorgar acceso a funcionalidades individuales de Enterprise Guard sin asignar roles administrativos más amplios. Esto permite a las organizaciones personalizar el acceso en función de las responsabilidades internas de gobernanza, seguridad o cumplimiento.

Al crear o editar un rol de admin personalizado, los admins de empresa pueden seleccionar las funcionalidades que determinan a qué capacidades de Enterprise Guard puede acceder y gestionar el rol. Estas funcionalidades abarcan varios dominios de Enterprise Guard, como clasificación de datos, descubrimiento de datos, gestión del ciclo de vida del contenido y eDiscovery.

Al asignar solo las funcionalidades requeridas, las organizaciones pueden delegar tareas administrativas, como revisar hallazgos de contenido sensible, gestionar configuraciones de clasificación, configurar políticas de ciclo de vida o acceder a herramientas de eDiscovery, a los equipos correspondientes. La tabla a continuación lista las funcionalidades que se pueden asignar al configurar roles de admin personalizados.

|  |  |  |
| --- | --- | --- |
| **Capacidad** | **Privilegio** | **Descripción** |
| **Clasificación de datos** | Ver la configuración de clasificación de datos | El admin puede ver la configuración de la clasificación de la organización. |
| Editar la configuración de clasificación automática | El admin puede editar la configuración de clasificación automática de la organización. |
| **Descubrimiento de datos** | Ver configuración de descubrimiento de datos | El admin puede ver la configuración de descubrimiento de datos de la organización. |
| Gestionar la configuración de descubrimiento de datos | El admin puede gestionar la configuración de descubrimiento de datos de la organización. |
| Ver resultados de descubrimiento de datos | El admin puede ver resultados relacionados con el descubrimiento de datos. |
| Gestionar resultados de descubrimiento de datos | El admin puede gestionar los resultados relacionados con el descubrimiento de datos. |
| **eDiscovery** | Ver configuración de retenciones legales | El admin puede ver las retenciones legales en la página de configuración de los casos de eDiscovery. |
| Gestionar configuración de retenciones legales | El admin puede administrar las retenciones legales en la página de configuración de los casos de eDiscovery. |
| Ver exportaciones de tableros | El admin puede ver exportaciones de tableros de eDiscovery. |
| Gestionar exportaciones de tableros | El admin puede gestionar exportaciones de tableros de eDiscovery. |
| **Gestión del ciclo de vida del contenido** | Ver configuración de la papelera | El admin puede ver la configuración de la papelera de tableros de la organización. |
| Gestionar configuración de la papelera | El admin puede gestionar el tiempo de vida útil y los permisos de la papelera de tableros de la organización. |
| Ver configuración de retención del ciclo de vida del contenido | El admin puede ver la página de configuración de retención del ciclo de vida del contenido. |
| Gestionar parámetros de configuración de retención del ciclo de vida del contenido | El admin puede gestionar la página de configuración de retención del ciclo de vida del contenido. |
| Ver parámetros de configuración de eliminación del ciclo de vida del contenido | El admin puede ver la página de configuración de eliminación del ciclo de vida del contenido. |
| Gestionar parámetros de configuración de eliminación del ciclo de vida del contenido | El admin puede gestionar la página de configuración de eliminación del ciclo de vida del contenido. |
| Ver contenido bajo retención o eliminación | Permite al usuario ver el contenido afectado por políticas de retención o eliminación. |
