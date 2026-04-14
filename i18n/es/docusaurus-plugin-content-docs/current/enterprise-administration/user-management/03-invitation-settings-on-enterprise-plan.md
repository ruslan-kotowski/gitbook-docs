---
title: "Configuraci\xF3n de las invitaciones en el plan Enterprise"
article_id: 4412315533842
translation_id: 4412315533842
locale: es
sidebar_position: 3
created_at: '2021-12-13T04:56:26Z'
updated_at: '2026-02-19T10:56:01Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: invitations
---

Configura las invitaciones de tu plan Enterprise para administrar quién puede invitar usuarios nuevos. Puedes personalizar la configuración de tus invitaciones para cumplir con los requisitos de tus equipos y de la empresa en general.

> **Disponible para**: plan Enterprise
> **Quién puede hacerlo:** admins de empresa

:::tip
Si eres nuevo en Miro, aprende más sobre [configuración de Equipo y Compañía](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md).
:::

## Configuración de las invitaciones del equipo

Para lograr una colaboración más fluida, permite que **todos los miembros del equipo** inviten a nuevos Miembros al equipo. Si prefieres tener más control sobre las invitaciones al equipo, puedes restringir esta opción a los admins de empresa y/o de equipo, para que todas las solicitudes de invitación se envíen a través de [administración de solicitudes](09-request-management-on-enterprise-plan.md). También puedes controlar si los usuarios pueden invitar a [invitados](../../using-miro/sharing-boards/07-collaboration-with-guests.md) a los equipos.

### Cómo configurar las invitaciones al equipo

Para gestionar la configuración de invitaciones al equipo, en la Consola de Administración ve a **Equipos** y selecciona tu equipo. Se abrirá el panel de tu equipo. Bajo **Invitación**, selecciona una de las siguientes opciones:

- **Admins de empresa únicamente**
  Solo los admins de empresa pueden agregar miembros nuevos al equipo.
- **Admins de empresa y de equipo**
  Los admins de empresa y de equipo pueden invitar miembros nuevos al equipo.
- **Todos los miembros del equipo**
  Todos los miembros del equipo pueden invitar miembros nuevos al equipo.

:::note
En [suscripciones del Programa de licencias flexibles (PLF)](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md), la configuración de invitaciones del equipo se complementa con las preferencias de invitación de la empresa.
:::

### Cómo configurar las invitaciones para invitados

Los admins de empresa pueden permitir o restringir la opción para que los miembros inviten a [invitados](../../using-miro/sharing-boards/07-collaboration-with-guests.md). Los invitados solo pueden acceder a los tableros a los que están invitados y no requieren una licencia.

Actualiza la configuración de las invitaciones de los invitados en **Equipos** > selecciona tu equipo > **Configuración** > **Permitir invitados para el equipo [Nombre].**

:::note
Los admins de empresa pueden habilitar la desactivación automática de invitados después de 30 días de inactividad.
:::

## Escenarios posibles para las invitaciones

:::tip
Dependiendo de la [administración de solicitudes](09-request-management-on-enterprise-plan.md), las solicitudes para compartir un tablero o invitar a un usuario a un equipo pueden enviarse directamente a los admins de empresa, a personas específicas por correo electrónico, o se puede crear un ticket de servicio.
:::

**Invitar a miembros nuevos a un equipo**

Si los invitados no están permitidos y los miembros no tienen autorización para invitar a miembros nuevos, cuando intenten compartir un tablero verán la notificación a continuación y deberán enviar una solicitud.

**Otorgar el rol de propietario o copropietario**

Si los miembros no están autorizados a invitar a miembros nuevos e intentan asignar el rol de propietario o copropietario a un invitado o un [miembro de una cuenta gratuita limitada](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) en un tablero específico, verán la notificación a continuación y deberán enviar una solicitud.

**Invitar a un usuario externo o invitado a editar un tablero**

:::note
Los invitados externos son invitados fuera del dominio de tu empresa. Tendrán un correo electrónico de una empresa externa.
:::

Si los miembros no están autorizados a invitar a nuevos miembros al equipo y los invitados con acceso de edición no están habilitados para el equipo, cuando intenten invitar a un usuario externo para editar un tablero, los usuarios verán la notificación a continuación y deberán enviar una solicitud. Después de enviar la solicitud, el invitado será agregado al tablero con acceso a comentarios, lo que le permitirá agregar comentarios en el tablero pero no editar su contenido.

## Ajustes de invitaciones de la empresa

La configuración de invitaciones de la empresa controla quién puede invitar a nuevos miembros a tu suscripción Enterprise. A todos los nuevos miembros se les otorga una licencia Avanzada, Estándar, Completa (antigua), Gratis o Gratis Restringida, dependiendo de tu [modelo de licenciamiento](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md) y [licencia predeterminada](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).

### Cómo configurar la configuración de invitaciones de la empresa

> **Disponible para**: [Programa de Licencias Flexibles (PLF)](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)

Para gestionar la configuración de invitación de la empresa, ve a **Configuración de empresa** > **Seguridad** > **Compartir** > **Invitación** y selecciona una de las siguientes opciones:

**Admins de empresa únicamente**
Solo los admins de empresa pueden otorgar licencias a los miembros nuevos. Los admins de equipo y los miembros solo pueden invitar a miembros existentes de la empresa a sus equipos, y no pueden activar licencias nuevas.

**Admins de empresa y admins de equipo**
Los admins de empresa y de equipo pueden invitar a miembros nuevos y añadir nuevas licencias. Los admins de equipo solo pueden invitar a miembros nuevos a equipos en los que son admins de equipo.

**Todos los miembros**
Cada miembro de la suscripción de Enterprise puede agregar nuevas licencias invitando a personas a su equipo, siempre que las invitaciones estén permitidas para **Todos los miembros del equipo** en la configuración de invitaciones del equipo.

## Cómo se articulan las configuraciones de empresa y equipo

La configuración de la empresa complementa la configuración de invitaciones del equipo. Los admins de empresa pueden configurar quién puede invitar a usuarios a un equipo específico en la configuración de equipos. Esto significa que los admins de empresa pueden permitir que los miembros y los admins de equipo gestionen sus propias invitaciones y colaboraciones de equipos, pero los admins de empresa siguen controlando las licencias en la configuración de la empresa.

## Desactivación automática de invitados

Configura la desactivación automática de invitados después de 30 días de inactividad. Usa esta función para eliminar invitados y mantener tu suscripción segura.

Cuando la función está activada, todos los invitados (independientemente de su dominio) que no hayan estado activos en tus equipos de Enterprise en un plazo de 30 días se desactivarán automáticamente. No es posible personalizar el período de 30 días.

Esta configuración se aplica a todos los equipos de la organización.

Ve a las **configuraciones de la compañía** > **Seguridad** > **Compartir** y activa **Desactivar automáticamente a los invitados**.

:::tip
Tan pronto como el ajuste se active, la acción se registrará en los [registros de auditoría](../security-integrations/security-management/01-audit-logs.md) como **Configuración de expiración de usuarios externos habilitada/deshabilitada**. Los eventos de desactivación también se registrarán en los [registros de auditoría](../security-integrations/security-management/01-audit-logs.md). El actor se mostrará como **Miro Automation**.
:::
