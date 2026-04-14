---
title: Ajustes de invitaciones
article_id: 360022258119
translation_id: 360022258119
locale: es
sidebar_position: 3
created_at: '2021-06-03T10:01:33Z'
updated_at: '2025-06-02T11:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: invitations
availability:
  notes: 'Quién puede hacerlo: (Free, Starter, Education) Administradores de equipos,
    (Business, Enterprise) Administradores de empresa, Administradores de equipos'
---

Los admins pueden configurar permisos de invitación para un equipo y restringir la capacidad de los usuarios que no son admins para [invitar a miembros nuevos](01-invite-users.md) y cambiar el tamaño de la suscripción.

Accede a la consola de administración haciendo clic en tu avatar de perfil en la esquina superior derecha y luego haciendo clic en **consola de administración**.

En la pestaña **Seguridad** > **Permisos**, desplázate hacia abajo hasta **ajustes de invitaciones**. Los ajustes se ven diferentes en los diversos planes de Miro.

En los planes Free, Starter y Education, también puedes habilitar o deshabilitar el enlace de invitación al equipo, que permite que los usuarios se unan a tu equipo mediante un enlace especial que se puede copiar en los modales de Compartir e Invitación de los tableros. [Obtén más información](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).

![invitation-settings.png](../../../../../../docs/administration/user-management/images/25007070132626_invitation-settings.png)
*Ajustes de invitación en el plan Starter*

En los planes Starter y Education, solo los miembros pueden editar los tableros. Por lo tanto, si un usuario que no está autorizado a invitar a miembros intenta compartir un tablero con un editor que no es miembro del equipo, verá el mensaje emergente.

## Configuración de invitaciones en el plan Business y Enterprise

En los planes Business y Enterprise, los admins de empresa además pueden permitir o prohibir a [invitados](../../using-miro/sharing-boards/07-collaboration-with-guests.md).

![inv-settings-invitation.png](../../../../../../docs/administration/user-management/images/21855329470994_inv-settings-invitation.png)
*Configuración de las invitaciones en el plan Enterprise*

[Los administradores de empresa](../get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md) en el plan Business y el plan Enterprise pueden configurar los ajustes de invitación para cada equipo dentro de la suscripción.

Sigue estos pasos:

1. Ve a la **Consola de Admin**.
   Desde el panel de Miro, haz clic en tu avatar en la esquina superior derecha y selecciona **Admin Console**.
2. Haz clic en **Teams**.
3. En **nombre del equipo**, selecciona un equipo.
   Se abre el panel de configuración del equipo.
4. Haz clic en **Configuración**.
5. En **Invitación**, selecciona quién puede invitar a usuarios a este equipo.
   > ⚠️ (Business) Tu cantidad de licencias aumentará automáticamente cuando se añada un nuevo usuario. Si permites que cualquiera invite a nuevos usuarios, entonces cualquiera puede incurrir en nuevas licencias añadidas a tu suscripción.
6. Selecciona **Permitir** o **No permitir** para invitados.
7. Haz clic en la **X** en la esquina superior derecha para cerrar el panel de configuración del equipo.
   Tu configuración está guardada.

Si los usuarios no están autorizados a invitar a miembros nuevos, no verán la opción en sus paneles. Se muestra un mensaje emergente para los usuarios del plan Business si los invitados no están permitidos.

Para obtener más información sobre cómo funcionan las configuraciones de invitación en el plan Enterprise, consulta [este artículo](../../enterprise-administration/user-management/03-invitation-settings-on-enterprise-plan.md).
