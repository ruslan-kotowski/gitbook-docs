---
title: Configuración de las invitaciones del equipo
article_id: 13205512707858
translation_id: 13205512707858
locale: es
sidebar_position: 3
created_at: '2023-08-21T13:54:06Z'
updated_at: '2025-06-23T13:54:36Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: invitations
availability:
  notes: 'Quién puede hacerlo: admins de equipo, admins de empresa ¿Qué planes?: Free,
    Starter, Education, Business, Enterprise ¿Qué plataformas: Navegador, Escritorio,
    Móvil'
---

Los admins pueden especificar qué miembros del equipo pueden invitar a nuevos miembros a su plan Free o de pago. Por ejemplo, los admins pueden habilitar que solo los admins inviten a nuevos miembros.

Opcionalmente, los admins también pueden permitir que todos los miembros del equipo inviten a nuevos miembros.

:::note
Para los planes de pago, cuando un invitado acepta una invitación de un miembro existente del equipo, incluidos los admins, se añade automáticamente una licencia a tu suscripción.
:::

Si habilitas solo a los admins para agregar nuevos miembros al equipo, entonces los miembros existentes que no son admins no tendrán la opción de invitar a nuevos miembros en Miro.

:::tip
Para los planes Business y Enterprise, los admins de empresa pueden [configurar la configuración de invitación](../get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md) para cada equipo individualmente dentro de su suscripción.
:::

## Gestionar la configuración de las invitaciones al equipo

Para administrar la configuración de invitaciones del equipo en un plan Free, Starter o Education, asegúrate de tener el rol de admin de equipo.

Para gestionar la configuración de invitaciones del equipo en un plan Business o Enterprise, asegúrate de tener el rol de admin de empresa.

### plan Free, Starter y Education

Como admin de equipo, sigue estos pasos:

1. Desde el panel de Miro, haz clic en tu avatar en la esquina superior derecha y selecciona **Admin Console**.
2. Ve a **Seguridad** > **Permisos**.
3. Debajo de **Invitación**, selecciona quién puede invitar a usuarios a tu equipo.
4. (Opcional) Para proporcionar un enlace de equipo que cualquiera pueda seguir para unirse, activa **Habilitar enlace de invitación al equipo**.

:::note
Para los planes Starter y Education, si los miembros del equipo no tienen permitido invitar a nuevos miembros, cualquier miembro que envíe una invitación para editar verá una ventana emergente con **Pedir al admin que dé acceso de edición** preseleccionado. El miembro del equipo puede enviar su invitación, pero el invitado será añadido como invitado o autor del comentario, pendiente de la aprobación del admin para acceso de edición. Solo los miembros del equipo pueden editar tableros.
:::

### Plan Business

Como admin de empresa, sigue estos pasos:

1. Desde tu panel de Miro, haz clic en tu avatar en la esquina superior derecha y selecciona **Consola de Admin**.
2. Haz clic en **Equipos**.
3. Debajo de **nombre del equipo**, selecciona un equipo.
   El panel de configuración del equipo se abre.
4. Haz clic en **Configuración**.
5. En **Invitación**, selecciona quién puede invitar a usuarios a este equipo.
   > ⚠️ Tus licencias se incrementan automáticamente cuando se añade un nuevo usuario. Si permites que cualquiera invite a nuevos usuarios, cualquiera puede incurrir en nuevas licencias añadidas a tu suscripción.
6. Selecciona **Permitir** o **No permitir** para los [invitados](../../using-miro/sharing-boards/07-collaboration-with-guests.md).
7. En la esquina superior derecha, haz clic en la **X** para cerrar el panel de configuración del equipo.
   Tus configuraciones han sido guardadas.

> Si los invitados no están permitidos, un miembro del equipo que intente invitar a un invitado verá un mensaje emergente informándoles que los invitados no están permitidos.

### plan Enterprise

Para conocer la configuración de invitación de equipo en el plan Enterprise, consulta [Permisos de equipo en el plan Enterprise](../../enterprise-administration/managing-enterprise-teams-and-content/10-team-permissions-on-enterprise-plan.md).
