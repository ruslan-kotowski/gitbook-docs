---
title: Invitar a usuarios
article_id: 360017730013
translation_id: 360017730013
locale: es
sidebar_position: 4
created_at: '2019-02-11T10:08:23Z'
updated_at: '2026-01-06T11:44:43Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: invitations
---

Invita a personas a tu equipo y tableros fácilmente para empezar a colaborar y crear juntos. Dependiendo de [la configuración de las invitaciones](02-invitation-settings.md), la opción de invitar a nuevos usuarios puede estar disponible solo para los admins o para todos los miembros.

:::note
Visita [este artículo](../../enterprise-administration/user-management/05-manage-user-invitations-on-enterprise-plan.md) para aprender cómo invitar usuarios en el plan Enterprise.
:::

## Invitar a miembros

Hay varias maneras en que puedes añadir miembros a tu equipo.

- Desde tu panel. Haz clic en **Invitar miembros** en la esquina superior derecha
  ![invite-members-dashboard.png](../../../../../../docs/administration/user-management/images/25007019083026_invite-members-dashboard.png)
  *La opción de invitar miembros desde el panel*
- Desde la Consola de admin: Abre la pestaña **Todos los usuarios**. Allí verás a todos los miembros del equipo y los usuarios invitados.

  ![admin-invite-users.png](../../../../../../docs/administration/user-management/images/25007019084178_admin-invite-users.png)
  *La opción para invitar a nuevos miembros desde la Consola de admin*

  Haz clic en **Invitar a nuevos miembros** en la esquina superior derecha e ingresa los correos electrónicos de quienes desees invitar. Puedes ingresar hasta 500 correos electrónicos en el módulo de invitación.

  ![invite_modal.jpg](../../../../../../docs/administration/user-management/images/21017416281746_invite%20modal.jpg)
  *Módulo de invitación*
- En este menú, también puedescopiar[**enlace de invitación al equipo**](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md): todos los que sigan el enlace podrán unirse a tu equipo (disponible en los planes [Free](../../plans-billing/miro-plans/09-free-plan.md), [Starter](../../plans-billing/miro-plans/08-starter-plan.md) y [Education](../../plans-billing/miro-special-pricing/03-education-plan.md)). Los administradores pueden habilitar o deshabilitar el enlace en la [configuración de invitaciones](02-invitation-settings.md)
- En el plan Free, **cada usuario** [**invitado a un tablero mediante correo electrónico**](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) es invitado al equipo y también se convierte en un miembro del equipo
- En el plan Starter, **cada editor** [**invitado a un tablero mediante correo electrónico**](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)se convierte en un miembro del equipo. Verás la siguiente notificación y también tendrás la opción de invitar al usuario con acceso para comentar sin añadirlo al equipo
  ![only_members_can_edit.jpg](../../../../../../docs/administration/user-management/images/21017429340690_only%20members%20can%20edit.jpg)
  *Una notificación que indica que solo los miembros pueden editar los tableros en este tipo de plan*

Tus invitados recibirán una invitación por correo electrónico y podrán unirse al trabajo de inmediato.

Si el invitado no está registrado en Miro, la invitación estará activa por 30 días. También recibirán una notificación por correo electrónico al 3.º y 7.º día si no la aceptan de inmediato. Al hacer clic en el enlace del correo de notificación, se les sugerirá [registrarse](../../getting-started/start-here/02-how-to-register-with-miro.md). Si un invitado no registrado no acepta la invitación dentro de los 30 días, esta expira y el usuario se elimina de la lista de **usuarios activos**.

Los usuarios registrados de Miro podrán encontrar tu equipo en la barra lateral izquierda de su [panel](../../getting-started/start-here/miro-dashboard/01-what-is-on-your-dashboard.md) tan pronto como los invites.

Si, por accidente, envías una invitación a una dirección de correo electrónico incorrecta o tienes un error de tipeo y quieres eliminar la invitación adicional, haz clic en los tres puntos junto al usuario invitado y selecciona **Revocar invitación.**

### Miembros de prueba en el plan Starter

:::note
Solo disponible para el [Plan Starter](../../plans-billing/miro-plans/08-starter-plan.md).
:::

Cuando invitas a miembros al equipo, en lugar de añadirlos de inmediato como una licencia de pago, se añadirán primero como **miembros** **gratuitos**.

La licencia de los usuarios seguirá siendo gratuita hasta que el usuario invitado realice alguna acción de pago dentro del equipo, como abrir un tablero o crear su propio tablero o proyecto.

Una vez que se realiza la acción de pago, la licencia se convierte en una prueba por 7 días y no se consume una licencia en este punto.

Los usuarios pueden tener acceso completo de pago de manera gratuita durante siete días, lo que les permite colaborar sin comprometerse con un costo de inmediato.

Durante la prueba, se puede ascender a los nuevos miembros a miembros con acceso completo o convertirlos en invitados en la sección **Todos los usuarios** en el admin.

Los miembros de prueba se convierten en miembros de pago si no se toma ninguna acción al finalizar la prueba (7 días). Si no quieres agregar a los miembros de prueba como **miembros con acceso completo del equipo** después de finalizar su prueba, puedes [eliminarlos](08-remove-users.md) del equipo o convertirlos en usuarios invitados en cualquier momento durante la prueba (lo que significa que podrán ver y comentar en el tablero específico al que fueron invitados explícitamente).

Ten presente que las pruebas para miembros solo están disponibles una sola vez para los miembros nuevos. Una vez que se use una prueba, los miembros que se vuelvan a agregar ocuparán una licencia de pago de inmediato.

Si el plan Starter se [mejora a Business Plan](https://help.miro.com/hc/articles/360011780620-How-to-Change-Your-Plan#h_8315f4f8-9f5b-4665-b271-e438aedaf289), todos los miembros de prueba actuales se convierten en miembros con acceso completo en el momento de la mejora.

El costo de la nueva licencia **se prorratea** por el tiempo restante en tu período de suscripción actual (exacto hasta un día), para que tus fechas de renovación para las nuevas licencias siempre coincidan con tus licencias existentes. Si tienes licencias vacantes durante tu período de suscripción y añades un nuevo miembro, no se aplicará ningún cargo. Para obtener más información sobre el sistema de cargos prorrateados, consulta nuestro artículo - [Facturación y pagos](../../plans-billing/billing-and-payments/04-miro-billing.md).

## Invitar a invitados

Puedes compartir tus tableros con usuarios mediante correo electrónico sin añadirlos a tu equipo como miembros. Estos usuarios se listarían como invitados en la configuración de tu Equipo.

:::warning
Ten en cuenta que los invitados no están disponibles en el [plan Free](../../plans-billing/miro-plans/09-free-plan.md).
:::

:::note
La opción para invitar a invitados puede estar restringida en [configuración de invitaciones](02-invitation-settings.md) en los planes Business.
:::

En los planes Starter y Education, puedes invitar a invitados que solo tengan acceso para ver o comentar.

En el plan Business, puedes agregar invitados a tus tableros en calidad de visualizadores, comentaristas o editores.

Estos usuarios están listados como **invitados** en tu consola de administración. Los administradores pueden convertirlos en miembros o eliminarlos del equipo/revocar la invitación.

Los invitados no pueden crear sus propios tableros en el equipo y no pueden acceder a [tableros compartidos del equipo](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) y proyectos. Si solicitan unirse al equipo, la notificación se enviará a los admins.

:::note
Aprende a convertir miembros en invitados en [esta página](../../using-miro/sharing-boards/07-collaboration-with-guests.md).
:::

## Invitar visitantes

También puedes compartir tus tableros con los visitantes. Esos usuarios no se añaden a tu equipo y pueden ver/comentar/editar tableros públicos sin ser usuarios registrados. La opción está disponible en todos los planes de pago. Más información: [Colaboración con visitantes](../../using-miro/sharing-boards/08-collaboration-with-visitors.md).

:::note
Ver la diferencia entre miembros, invitados y visitantes en [esta página](../../using-miro/sharing-boards/07-collaboration-with-guests.md).
:::

## Preguntas frecuentes

1. *Mi invitado no recibió el correo electrónico que envié con la invitación. ¿Cómo puede acceder a mi equipo?*
   - Pídele al usuario que se registre en Miro o que inicie sesión si ya tiene un perfil. El usuario encontrará tu equipo en la barra lateral izquierda de su [panel](../../getting-started/start-here/miro-dashboard/01-what-is-on-your-dashboard.md).
2. *Me invitaron a un equipo de Miro, pero no lo veo cuando inicio sesión. ¿Cómo puedo acceder al equipo?*
   - Intenta encontrar el equipo en la barra lateral izquierda de tu [panel](../../getting-started/start-here/miro-dashboard/01-what-is-on-your-dashboard.md) y cambia a ese equipo. Si no hay un equipo, asegúrate de estar autorizado en Miro con la misma dirección de correo electrónico con la cual te invitaron al equipo.
3. *No tengo un botón de Invitar a miembros en mi panel. ¿Por qué?*
   - Los admins han restringido la opción de invitar a nuevos miembros en las [configuraciones de invitación](02-invitation-settings.md). Ten presente que esta opción puede estar limitada para los admins de equipo en el plan Enterprise.
4. *¿Puedo invitar a usuarios sin que se registren en Miro?*
   - Sí, puedes [compartir tus tableros mediante enlaces públicos](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartir-tableros-a-traves-de-un-enlace-publico) con usuarios no registrados de forma gratuita.
5. *¿Qué hacer si accidentalmente invité a nuevos miembros de pago?*
   - Por favor, [sigue estos pasos](../../plans-billing/billing-and-payments/04-miro-billing.md).
