---
title: Descripción general de la gestión de usuarios en el plan Enterprise
article_id: 360017571474
translation_id: 360017571474
locale: es
sidebar_position: 12
created_at: '2019-02-11T10:09:06Z'
updated_at: '2026-02-26T14:12:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-management
availability:
  notes: 'Disponible para: [plan Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)
    Configurado por: admins de empresa'
---

Puedes administrar fácilmente los permisos de decenas, cientos o miles de usuarios de Miro en tu plan. Los admins pueden hacer un seguimiento de las listas de usuarios y filtrarlas, y ver los roles de los usuarios, su tasa de actividad y el consumo de las licencias. Usa acciones masivas como invitar, agregar y eliminar usuarios, asignar roles y licencias, y mover usuarios entre equipos. Ahorra tiempo y entiende mejor cómo funciona tu plan de Miro al dominar las operaciones administrativas rápidas en Miro.

Todos los usuarios corporativos que pertenecen a dominios que se han reclamado y verificado mediante el Control de dominio son [usuarios administrados dentro de tu organización Enterprise](06-managed-users-on-enterprise-plan.md).

## Sección de usuarios activos

Para abrir la configuración del equipo, haz clic en el nombre del equipo en la esquina superior izquierda de tu panel y luego haz clic en el icono de **Miembros del equipo**.

Se abrirán las configuraciones de la empresa con una lista de usuarios en el equipo elegido. En esta sección, los admins de empresa y de equipo pueden agregar o eliminar usuarios del equipo, y promover o revocar el rol de admin de equipo.

Los admins de empresa también pueden convertir a un invitado en un miembro con una licencia Estándar o Completa (legado). Para revocar o bajar de categoría una licencia avanzada, estándar o completa (legado), los admins de empresa pueden en su lugar asignar al miembro una licencia [Free restricted](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).

:::note
Los empleados que comparten un dominio verificado son miembros con una licencia Avanzada, Estándar, Completa (legado), Free, Free Restricted. Para los planes Enterprise, solo los usuarios de un dominio externo pueden añadirse como invitados.
:::

:::note
Los admins de equipo pueden invitar a nuevos miembros del equipo si está permitido en la [configuración de invitación](05-manage-user-invitations-on-enterprise-plan.md).
:::

Para ver la lista completa de los usuarios en tu suscripción Enterprise, ve a **Configuración de empresa**. En el lado izquierdo, debajo de **Usuarios**, selecciona **Todos los usuarios** para abrir la lista de usuarios activos (también puedes cambiar a las pestañas **Usuarios desactivados** e **Invitaciones** desde esta pantalla). Verás la lista de todos los usuarios añadidos o invitados a equipos o tableros dentro de esa suscripción en particular, así como su fecha de **Última actividad**.

:::note
Para llegar a la Configuración de empresa desde la Configuración del equipo, haz clic en **Empresa** en la esquina superior izquierda.
:::

Como admin de empresa, puedes descargar una lista completa de usuarios en tu organización junto con su último inicio de sesión. Encuentra el **botón Descargar CSV** arriba de la lista de usuarios activos.

En la **sección de usuarios activos** verás la lista completa de usuarios junto con su Rol, Licencia, Equipos y Actividad.

El **Rol** define los niveles de acceso dentro del plan. Mientras que admin de empresa es el rol más poderoso con la capacidad de administrar el plan, un invitado solo puede acceder a los tableros a los que se les invita. Aprende más en [el artículo sobre niveles de acceso.](11-user-access-levels-on-enterprise-plan.md)

El **tipo de Licencia** muestra si un usuario está consumiendo una licencia Avanzada, Estándar, Completa (legado) o Gratuita.

El **Equipos** es la cantidad de equipos dentro del plan a la que un usuario está añadido.

**Última** **actividad** muestra cuándo un usuario ha abierto algún tablero dentro de la suscripción. Para filtrar por usuarios activos/inactivos, selecciona las fechas del calendario o usa una de las opciones preestablecidas: 30, 60, 90 o 180 días. Definimos un usuario activo como alguien que ha usado Miro en los últimos 90 días

### Cambiar el estado de un solo usuario

Como admin de empresa, puedes cambiar el rol, la licencia y la cantidad de equipos para cualquier usuario o grupo de usuarios. También puedes [desactivar a un usuario](01-deactivated-users.md) y luego [eliminarlo](10-remove-users-on-enterprise-plan.md). Para acceder a estas opciones, haz clic en el ícono de **tres puntos** (**...**) junto a la fila de cualquier miembro del equipo.

:::tip
El sistema avanzado de gestión de usuarios te ayuda a administrar los recursos que has comprado de manera más eficaz. Si tienes activado el  [Programa de Licencias Flexibles](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md), puedes liberar licencias de usuarios inactivos convirtiéndolas en Free Restricted.
:::

### Filtros

Si tienes docenas, cientos o miles de usuarios de Miro **busca** por correo electrónico y nombre o **filtra la lista** por un criterio específico para encontrar a alguien más rápido. También puedes ocultar usuarios invitados para ver solo a los usuarios de Miro registrados en tu plan.

Una vez aplicados los filtros, puedes seleccionar masivamente hasta 50 usuarios en la lista y usar acciones masivas.

### Acciones masivas

El **botón de acciones masivas** te ayuda a administrar los grupos de usuarios más rápidamente. Selecciona varios usuarios para aplicar los cambios necesarios de forma masiva.

Puedes seleccionar a los usuarios de a uno marcando las casillas a la izquierda o aplicar filtros y seleccionar hasta 50 usuarios a la vez.

#### Gestiona usuarios activos de manera masiva

En la lista **Usuarios activos**, selecciona la lista de usuarios para aplicar una de las siguientes acciones.

1. Gestionar la membresía del equipo de manera masiva.
   1. Agregar o mover usuarios a un equipo.
   2. [Crear un nuevo equipo](../managing-enterprise-teams-and-content/09-create-a-new-team-on-enterprise-plan.md) y agregar usuarios.
2. Gestionar licencias y roles de manera masiva.
   1. Cambiar a miembro avanzado. Las licencias avanzadas no son compatibles con el Programa de Licencias Flexibles (PLF) y siempre operan bajo un modelo de límite fijo (no PLF). Solo puedes asignar hasta la cantidad de licencias avanzadas que tu organización haya adquirido. Las organizaciones que usan PLF para Standard pueden continuar haciéndolo manteniendo las licencias avanzadas bajo un límite fijo, permitiendo un modelo de licenciamiento mixto: Standard puede seguir en PLF (licencias gratuitas ilimitadas con baja automática a Free Restricted), mientras que las licencias avanzadas permanecen fijas a la cantidad de licencias compradas. Los usuarios que necesiten funciones avanzadas deben tener explícitamente asignada una licencia avanzada o seguir el proceso de mejora de plan de tu organización o el flujo de solicitud.
   2. Cambiar a miembro Standard o miembro con acceso completo (legado).
   3. Cambiar a miembro básico.
   4. Cambiar a invitado o invitado de equipo.
   5. Cambiar a Free Restricted (disponible para [suscripciones Enterprise FLP](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)).
3. Cambiar el grupo de facturación o crear uno nuevo.
4. Revocar Restringido.
5. Desactivar usuarios de manera masiva [.](01-deactivated-users.md)

#### Gestionar invitaciones de manera masiva

Cambia a la pestaña de Invitaciones para ver usuarios invitados (usuarios no registrados a quienes se les enviaron invitaciones para unirse a tu suscripción hace menos de 30 días y que aún no se han registrado en Miro). Selecciona la lista de invitados para realizar una de las siguientes acciones.

1. Gestionar la membresía del equipo de manera masiva.
   1. Agregar usuarios a varios equipos con o sin eliminar de los actuales.
   2. Agregar usuarios a un nuevo equipo ([crear uno nuevo](../managing-enterprise-teams-and-content/09-create-a-new-team-on-enterprise-plan.md)).
2. [Desactivar](01-deactivated-users.md) usuarios de manera masiva.
3. Cambiar las licencias de usuario de manera masiva.

#### Eliminar de un equipo de manera masiva

En la lista **Equipos** selecciona el equipo en el cual quieres eliminar usuarios. Una vez seleccionados los usuarios, puedes eliminarlos del equipo.

### Información del usuario

La información del usuario es una tarjeta de estado individual y editable para cada usuario dentro de tu plan. Al contrario que en la gestión masiva, puedes ver el estado y administrar a una persona de manera individual. Cada usuario tiene un **perfil de usuario** con una fotografía, nombre, correo electrónico, número de tableros, número de proyectos, número de plantillas, equipos actuales y licencia. Para abrir una tarjeta de usuario, haz clic en el ícono de **tres puntos** (**...**) en su fila y selecciona **Información del usuario**.

:::note
Los detalles del usuario incluyen una clasificación **interna** o **externa**. Los usuarios internos inician sesión con una dirección de correo electrónico de un dominio verificado. Los usuarios externos no lo hacen. Para más información, consulta [Control de dominio: usuarios internos y externos](../canvas-25-admin-features/domain-control/01-domain-control.md).
:::

Los admins de empresa pueden cambiar la membresía del equipo y otorgar derechos de admin a un usuario directamente desde la tarjeta. Ten en cuenta que los Admins no pueden cambiar la información del usuario como el nombre, la imagen de perfil o el correo electrónico; en cambio, los usuarios pueden hacer eso en su configuración de perfil. Si usas [SSO](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), los datos son atribuidos automáticamente por tu proveedor de identidad al iniciar sesión correctamente.

### Preguntas frecuentes

1. *Recibo muchas solicitudes de usuarios para agregarlos a diferentes equipos. Quiero dejar de recibir estas notificaciones.*
   - Es probable que tu [privacidad del equipo](../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md) esté deshabilitada, lo que significa que los usuarios de Enterprise pueden descubrir nuevos equipos a los que unirse dentro de la organización. Si quieres dejar de recibir estas solicitudes, puedes:
   - Habilitar la privacidad, de manera que los usuarios no puedan descubrir nuevos equipos en la organización o
   - Hacer que los equipos sean completamente abiertos, de manera que los usuarios no necesiten tu aprobación para unirse al equipo
2. *Muchos usuarios están recibiendo una licencia Estándar o Completa (heredada), pero yo no asigné ninguna. ¿Por qué?*
   - Para cada equipo, puedes definir quién debería poder invitar usuarios a un equipo específico. Asegúrate de configurar tu [configuración de invitación](03-invitation-settings-on-enterprise-plan.md). También puedes activar el [Programa de licencias flexibles](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) y establecer la licencia predeterminada (gratuita o gratuita limitada) que los usuarios recibirán al unirse a tu plan.
