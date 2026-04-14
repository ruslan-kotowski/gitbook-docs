---
title: Eliminar usuarios
article_id: 360017571234
translation_id: 360017571234
locale: es
sidebar_position: 8
created_at: '2019-02-11T10:08:26Z'
updated_at: '2025-11-25T15:58:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-management
---

Al eliminar un usuario, los administradores limitan su acceso al contenido del equipo y pueden asumir la propiedad del contenido del usuario o eliminarlo.

> **Disponible para:** Free, Starter, Business, Education
> **Configurado por:** admins de equipo, admins de empresa

### Cómo eliminar usuarios

Para eliminar miembros o [invitados](../../using-miro/sharing-boards/07-collaboration-with-guests.md) de tu equipo, ve a **la consola Admin.** Para acceder a la consola desde tu panel de control, haz clic en el avatar de tu perfil en la parte superior derecha y luego en el botón **Consola admin**.

En la pestaña **Usuarios** > **Todos los usuarios**, haz clic en el icono de **tres puntos** (**...**) situado junto a un usuario y selecciona **Eliminar del equipo**.

> ✏️ Si no ves la opción para eliminar a un usuario, verifica los pasos a continuación.

![eliminar-del-equipo.png](../../../../../../docs/administration/user-management/images/25008730223122_delete-from-team.png)*Eliminar a un miembro del equipo*

Si el usuario es el propietario de algunos tableros, [proyectos](../../using-miro/spaces/01-spaces.md) o [plantillas](../../getting-started/start-here/your-first-board/04-templates.md) que se crearon en este equipo (compartidos o privados), tendrás la opción de transferir la propiedad a otro de los miembros del equipo (en los planes Free o Education, a uno de los administradores) o eliminarlos. Haz clic en el icono de cruz si quieres cambiar la propiedad. Si eliges eliminar el usuario y el contenido, un admin podrá [restaurar los tableros](../../using-miro/managing-boards/08-how-to-restore-a-deleted-board.md) durante un plazo de 90 días.

:::note
En el plan Business, si eliges transferir la propiedad a los admins de equipo, el contenido se reasigna automáticamente a uno de los admins.
:::

![eliminar_usuario_modal.jpg](../../../../../../docs/administration/user-management/images/21017515322002_delete%20user%20modal.jpg)*Cambiar la propiedad de los tableros, mientras se elimina a un usuario*

En los planes de pago, también puedes eliminar usuarios en masa: selecciona varios usuarios y elige **Eliminar del equipo** en **Acciones masivas**.

![borrar-usuarios-masivo.png](../../../../../../docs/administration/user-management/images/25008759156370_bulk-delete-users.png)*Borrar varios usuarios en bloque*

El usuario eliminado perderá de inmediato todo acceso a los Espacios de tu equipo (sin que se le notifique). Ten en cuenta que conservará el acceso a los tableros del equipo que se compartieron con un enlace público, si el usuario guardó los enlaces a esos tableros específicos.

Una vez que hayas eliminado correctamente a los miembros del equipo, verás una notificación en la parte superior con el número de licencias ahora disponibles. Puedes invitar a nuevos miembros del equipo o ir a la configuración de facturación para reducir el número de licencias de tu equipo.

Si reduces el tamaño del equipo, la cantidad de tiempo no utilizado se reflejará como un crédito en el saldo de la subscripción. Para obtener más información sobre el sistema de cargos prorrateados, revisa el artículoFacturación y pagos.

### Cómo eliminar usuarios en un plan Business

Para eliminar un usuario y liberar una licencia vacante, abre **la consola Admin** > **Usuarios** > sección **Todos los usuarios** y elige **Eliminar** en el menú del usuario. Define si quieres transferir la propiedad del contenido del usuario o eliminar todos los recursos del usuario y haz clic en Confirm (Confirmar). Si eliges transferir el contenido del usuario, se reasignará a los admins del equipo donde se encuentra el contenido.

Si has eliminado usuarios con una [licencia con acceso completo](../../enterprise-administration/user-management/11-user-access-levels-on-enterprise-plan.md)verás una notificación en la parte superior con el número de licencias ahora disponibles. Si no planeas invitar a miembros Completos a ocupar las licencias vacantes, puedes reducir el tamaño de tu equipo en tu Configuración de **facturación** > **Cambiar tamaño del equipo**.

:::note
Si ves una notificación que diga **"El equipo debe tener al menos un administrador"** al intentar eliminar a un usuario, significa que el usuario es el único administrador de uno o más equipos dentro de la suscripción. Para solucionarlo, podrías [invitarte a estos equipos](01-invite-users.md) y otorgarte [derechos del rol de administrador de equipo](06-how-to-manage-admin-roles.md). Haz clic en el número de equipos del usuario correspondiente para saber de qué equipos es miembro.
:::

### Preguntas frecuentes

1. *No tengo la opción de eliminar usuarios.*  ¿Por qué?
   - Ten en cuenta que la opción de eliminar miembros sólo está disponible para los admins. Si no ves la opción en la configuración, pídele al administrador que elimine los usuarios. Puedes encontrar el correo electrónico del administrador actual en la lista **Active users (Usuarios activos)**. También puedes pedir al usuario que [te ascienda a admin.](06-how-to-manage-admin-roles.md)
2. *Nuestro administrador de Miro ya no está en la empresa.*  ¿Cómo puedo eliminarlos?
   - Consulta el artículo: Mi Admin de Miro dejó la empresa
3. *¿Cómo puedo eliminar las licencias vacías?*
   - Si tienes licencias vacantes que quieres eliminar, sigue [esta guía](../../plans-billing/billing-and-payments/04-miro-billing.md).
