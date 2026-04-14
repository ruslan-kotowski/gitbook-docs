---
title: "Gu\xEDa de despliegue de Enterprise Guard - Parte 1: Configurar roles de admins"
article_id: 17120595534994
translation_id: 17120595534994
locale: es
sidebar_position: 1
created_at: '2024-02-19T09:19:59Z'
updated_at: '2025-11-25T15:41:04Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Los admins de empresa pueden otorgarse a sí mismos y a otros roles de admins adicionales una vez habilitado Enterprise Guard. En consecuencia, el número de admins de empresa en tu organización debe mantenerse al mínimo. Considera detenidamente tu configuración actual de admins y traslada a los admins de empresa a otros roles (como admins de equipos o usuarios) cuando sea apropiado para equilibrar la seguridad, el cumplimiento y la eficacia operativa.

Aunque se recomienda, no es necesario realizar una reevaluación global de la configuración de admins para implantar Enterprise Guard. Pasa a [Parte 2: Despliega la Seguridad de Datos](03-enterprise-guard-deployment-guide-part-2-deploy-data-security.md) a tu discreción.

## Visión general de los roles de admins de Miro

Aquí tienes una lista de los roles de admins disponibles en Miro, incluyendo una descripción de responsabilidades y para quién son adecuados en una organización típica.

:::note
Notas :
- Se trata de una lista evolutiva de roles y privilegios. Consulta esta página periódicamente para ver las actualizaciones.
- Para asignar el rol admin de gobernanza de datos o admin de contenido sensible a un usuario, debes ser admins de empresa.
:::

|  |  |  |
| --- | --- | --- |
| **Rol de admins** | **Responsabilidades** | **Recomendado para** |
| **admins de empresa** | Responsable de la gestión general y de delegar responsabilidades específicas a otros roles de admins. Debe tener un amplio conocimiento de las necesidades operativas de la organización y de las obligaciones de cumplimiento. | - Administradores superiores de TI - Jefes de departamento - Gerentes de proyecto - Líderes de equipo - Directores de Operaciones - Directores de Tecnología de Empresa - Miro Propietario de Producto |
| **admins de equipo** | Gestiona los ajustes específicos de cada equipo y el acceso de los usuarios dentro de sus respectivos equipos. Garantiza la autonomía del equipo al tiempo que se alinea con políticas organizativas más amplias. | - Jefes de departamento - Gerentes de proyecto - Líderes de equipo - Directores de Operaciones |
| **Admins de usuario** | Gestión de usuarios y licencias. Ideal para gestionar el acceso y las cuentas de los empleados. Gestiona eficazmente a los usuarios sin sobrecargar a los admins de empresa o de equipo. | - Director de informática - Administradores informáticos - Servicio de asistencia informática |
| **admins de gobernanza de datos (Enterprise Guard)** | Responsable del cumplimiento y la gobernanza de datos. Debe comprender el panorama legal y normativo relevante para los datos de la organización, incluidas las políticas de retención y eliminación de la organización. | - Director de Cumplimiento (CCO) - Gestor de gobernanza de datos - Responsable de Cumplimiento - Responsable de Asuntos Reglamentarios - Administrador de riesgos - Gestor de Registros - Analista de eDiscovery - Analista forense |
| **Admins de eDiscovery (Enterprise Guard)** | Gestiona los ajustes de retención legal para conservar los tableros relevantes para las investigaciones en curso o los casos legales. Esto incluye crear, modificar y liberar retenciones o casos legales para evitar la eliminación permanente de contenido, garantizando el cumplimiento de las obligaciones legales y reglamentarias. Este rol es crucial para las organizaciones que requieren una conservación rigurosa de los datos para apoyar los procedimientos legales y los mandatos de cumplimiento. | - Asesoría Jurídica - Especialistas en eDiscovery - Responsables de cumplimiento - Gestores de riesgos - Analistas forenses - Director de Seguridad de la Información (CISO) - Responsable de Protección de Datos (RPD) - Responsable de Privacidad/Gerente de Privacidad |
| **Admins de contenido sensible (Enterprise Guard)** | Responsable de protección de datos y privacidad. Crucial para clasificar, gestionar y salvaguardar la información sensible en toda la organización. Importante para el manejo de PII, PHI, PCI o propiedad intelectual. | - Director de Seguridad de la Información (CISO) - Responsable de Protección de Datos (RPD) - Responsable de Privacidad/Gerente de Privacidad - Analista de Ciberseguridad - Consultor de seguridad informática |

:::tip
Más información sobre [los roles de admins y sus privilegios](../enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) en el plan Enterprise.
:::

## Matriz detallada de privilegios y roles admins de Enterprise Guard

La tabla siguiente enumera los privilegios detallados y la matriz de roles de admins para cada función.

|  |  |  |  |
| --- | --- | --- | --- |
| **Gestión del ciclo de vida del contenido** | | |  |
| **Privilegio** | **Admin de gobernanza de datos** | **Admin de contenido sensible** | **Admin de eDiscovery** |
| Ver la configuración de la papelera |  |  |  |
| Editar la configuración de la papelera |  |  |  |
| Agregar política de retención |  |  |  |
| Editar la política de retención |  |  |  |
| Eliminar la política de retención |  |  |  |
| Agregar política de eliminación |  |  |  |
| Editar la política de eliminación |  |  |  |
| Borrar la política de eliminación |  |  |  |
| **Clasificación de datos** | | |  |
| **Privilegio** | **Admin de gobernanza de datos** | Admin de contenido sensible | **Admin de eDiscovery** |
| Ver la configuración de clasificación de datos |  |  |  |
| Editar niveles de clasificación |  |  |  |
| Editar la configuración de la clasificación automática |  |  |  |
| Editar la configuración de las barreras de protección de clasificación |  |  |  |
| Editar el nivel de clasificación predeterminado |  |  |  |
| **Descubrimiento de datos** | | |  |
| **Privilegio** | **Admin de gobernanza de datos** | **Admin de contenido sensible** | **Admin de eDiscovery** |
| Ver las etiquetas de privacidad |  |  |  |
| Activar/desactivar la detección de datos de privacidad |  |  |  |
| Ver recuento de coincidencias: etiquetas de privacidad |  |  |  |
| Ver coincidencias ocultas: etiquetas de privacidad |  |  |  |
| Ver coincidencias completas: etiquetas de privacidad |  |  |  |
| **eDiscovery** | | |  |
| **Privilegio** | **Admin de gobernanza de datos** | **Admin de contenido sensible** | **Admin de eDiscovery** |
| Administrar la configuración de retenciones legales |  |  |  |
| Ver la configuración de retenciones legales |  |  |  |

tabla Matriz detallada de privilegios y roles admins para cada función

## Transición de la configuración de admins

### Audita tu configuración actual de admins

Revisa la lista de usuarios que tienen derechos de admin en Miro y sus responsabilidades. Utiliza la Herramienta de Evaluación de la Configuración Admin para generar un resumen del estado actual.

- Filtra la lista de usuarios de la sección **Usuarios activos** de la configuración de la empresa para ver los admins de empresa.
- Ver la lista de admins de usuario, admins de gobernanza de datos y admins de contenido sensible utilizando la sección del **rol Admin** de la configuración de la empresa.

### Mapea una nueva configuración de admins

Compara tu configuración actual de admins con la tabla anterior y con las políticas de tu empresa. Utiliza la Herramienta de Evaluación de la Configuración Admin para generar una nueva configuración.

Plantéate preguntas como

- ¿Quién necesita el rol de Gobernanza de datos?
- ¿Quién necesita el rol Contenido sensible?
- ¿Qué admins de empresa pueden convertirse en admins de usuarios?
- ¿Qué admins de empresa pueden pasar a admins de equipo?

### Reasignar roles e informar a los usuarios

Los siguientes artículos del Centro de Ayuda muestran cómo asignar los distintos roles. Para tu comodidad, personaliza las plantillas de correos electrónicos proporcionadas para informar a los usuarios de las transiciones.

- [Cómo asignar admins de empresa y admins de equipo](../../../administration/user-management/06-how-to-manage-admin-roles.md)
- [Cómo asignar admins de usuario, admins de gobernanza de datos y admins de contenido sensible](../enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md)

### Asigna la función admin de gobernanza de datos rol

:::note
Para asignar el rol admin de gobernanza de datos a un usuario, debes ser admin de empresa.
:::

1. Ve a la configuración de tu perfil.
   - Desde un tablero: **Menú principal > Preferencias > Configuración del perfil**.- Desde el panel: haz clic en tu avatar en la esquina superior derecha y haz clic en **Configuración**.
   - Desde la URL `https://miro.com/app/settings`: Elige tu Empresa en la lista de la esquina superior izquierda.
2. Bajo “Gestión de usuarios”, haz clic en Roles de admin.
3. En el panel derecho, haz clic en la **elipsis** **admin de gobernanza de datos** **(****...)**y selecciona **Asignar rol**.
4. Elige el usuario al que deseas asignar el rol admin de gobernanza de datos, desplázate hasta la parte inferior de la ventana y, a continuación, haz clic en **Asignar**.

### Asigna la función admin de contenido sensible rol

:::note
Para asignar el rol admin de contenido sensible a un usuario, debes ser admin de empresa.
:::

1. Ve a la configuración de tu perfil.
   - Desde un tablero: **Menú principal > Preferencias > Configuración del perfil**.- Desde el panel: haz clic en tu avatar en la esquina superior derecha y haz clic en **Configuración**.
   - Desde la URL `https://miro.com/app/settings`: Elige tu Empresa en la lista de la esquina superior izquierda.
2. Bajo “Gestión de usuarios”, haz clic en Roles de admin.
3. On el panel derecho, haz clic en la **elipsis** **admin de contenido sensible** **(****...)**y selecciona **Asignar rol**.
4. Elige al usuario al que quieras asignar el rol de admin de contenido sensible, desplázate hasta la parte inferior de la ventana y haz clic en **Asignar**.

### Asigna la función eDiscovery Admin rol

:::note
Para asignar el rol de admin de eDiscovery a un usuario, debes ser admin de empresa.
:::

1. Ve a la configuración de tu perfil.
   - Desde un tablero: **Menú principal > Preferencias > Configuración del perfil**.- Desde el panel: haz clic en tu avatar en la esquina superior derecha y haz clic en **Configuración**.
   - Desde la URL `https://miro.com/app/settings`: Elige tu Empresa en la lista de la esquina superior izquierda.
2. Bajo “Gestión de usuarios”, haz clic en Roles de admin.
3. On el panel derecho, haz clic en la **elipsis** **eDiscovery Admin** **(****...)**y selecciona **Asignar rol**.
4. Elige el usuario al que quieres asignar el rol de admins de eDiscovery, desplázate hasta la parte inferior de la ventana y haz clic en **Asignar**.

### Recursos

- [Herramienta de evaluación de la configuración admins](https://docs.google.com/spreadsheets/d/1a0WQc-fBpuVwfnoY8VCx66PjOXS76q7DJ__xDYcp8rk/edit?usp=sharing) (haz una copia)
- [Plantillas de correo electrónico | Comunicaciones de configuración de admins](https://docs.google.com/document/d/18Kw4GNPq7GnAx8R8co5PaZ04peVogfVDgsdKK2MuARM/edit?usp=sharing) (haz una copia)
