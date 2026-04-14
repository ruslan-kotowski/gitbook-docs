---
title: Licencia gratuita limitada
article_id: 360011746739
translation_id: 360011746739
locale: es
sidebar_position: 4
created_at: '2020-02-05T07:29:16Z'
updated_at: '2026-02-19T10:40:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
---

Cuando los usuarios nuevos se unen a una suscripción de Miro, dependiendo del [modelo de licencias de Enterprise](02-enterprise-licensing.md), se les puede asignar una licencia gratuita limitada.

> **Relevante para:** plan Enterprise

## ¿Cuándo se asigna a los usuarios una licencia gratuita limitada?

**En el programa de licencias flexibles (PLF)**, se puede asignar la licencia gratuita limitada a un usuario cuando:

- La licencia predeterminada para nuevos usuarios se configura como gratuita limitada
- El admin de empresa invita al usuario y selecciona la licencia gratuita limitada para él o ella en la ventana de invitación
- El admin de empresa concede al usuario una licencia gratuita limitada en **configuración de la empresa > usuarios activos**

:::note
Aprende más sobre el [Programa de licencias flexibles (PLF)](03-flexible-licensing-program-flp.md) y [la gestión de licencias en el PLF](05-license-management-on-the-flexible-licensing-program-flp.md).
:::

**En licencias no flexibles (que no sean FLF)**, se puede asignar una licencia gratuita limitada a un usuario en las siguientes situaciones:

- El usuario es capturado automáticamente (por [Control de dominio](../../canvas-25-admin-features/domain-control/01-domain-control.md) o [aprovisionamiento justo a tiempo](../../user-management/13-user-provisioning-on-enterprise-plan.md)) en una organización que no tiene suficientes licencias Avanzadas, Estándar o Completa (heredada) durante su registro en Miro.
- El usuario es invitado a un equipo dentro de una organización que no tiene suficientes licencias Avanzadas, Estándar o Completa (heredada).

Cuando se invita a varios usuarios al mismo tiempo, todos reciben licencias según el orden de sus correos electrónicos en la lista de invitados. Si la organización no tiene suficientes licencias, los usuarios que están al final de la lista recibirán una licencia gratuita limitada. En este caso, quien invita recibirá una notificación emergente sobre el acceso limitado de algunos usuarios.

## Cómo funcionan las licencias gratuitas limitadas para los usuarios

Los usuarios con licencia gratuita limitada pueden ver y comentar en los tableros de los equipos en los que participan, y solicitar permiso de edición y una licencia estándar o una licencia completa (anterior) a los admins de empresa. También pueden descubrir y unirse a equipos de la organización junto con otros miembros.

:::note
Los admins de empresa pueden [configurar la administración de solicitudes](../../user-management/09-request-management-on-enterprise-plan.md).
:::

### Acceso a tableros con licencia gratuita limitada

Los siguientes permisos para ver, comentar o editar aplican a usuarios con una licencia gratuita limitada:

|  |  |
| --- | --- |
| **Cómo se compartió el tablero** | **Nivel de acceso** |
| Enlace público | Los usuarios con licencia Free restringida pueden ver y/o editar según el nivel de acceso otorgado. |
| Enlace de equipo o empresa | Los usuarios con licencia Free restringida pueden ver y/o comentar según el nivel de acceso otorgado. |
| [Enlace incrustado](../../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md) | Los usuarios con licencia gratuita limitada pueden ver o comentar según el nivel de acceso otorgado.  Los usuarios con licencia gratuita limitada no podrán editar ni solicitar acceso de edición, incluso si el acceso de edición se otorga a través de los permisos de inserción. |

## Cómo gestionar licencias gratuitas limitadas

> **Quién puede hacerlo:** Admins de empresa

En todas las suscripciones, el admin de empresa puede mejorar el plan de una licencia de usuario de gratuita limitada a una licencia estándar o completa (anterior) en la sección **Usuarios activos** de la configuración de su equipo o empresa.

**Programa de Licencias Flexibles (FLP)**

En las suscripciones del Programa de Licencias Flexibles (PLF), el admin de empresa también puede bajar de categoría una licencia Avanzada, Estándar o Completa (legado) a una licencia gratuita limitada en cualquier momento.

Cuando un usuario con licencia gratuita limitada solicita acceso a edición, los admins de empresa reciben la solicitud en función de su [configuración de administración de solicitudes](../../user-management/09-request-management-on-enterprise-plan.md).

:::note
Aprende más sobre [la gestión de licencias en el Programa de Licencias Flexibles](05-license-management-on-the-flexible-licensing-program-flp.md).
:::

## Preguntas frecuentes

**¿Qué sucede con mis licencias gratuitas limitadas cuando agrego más licencias estándar o completas (legado) a mi plan que no es FLP?**

Los usuarios existentes con licencia gratuita limitada no se actualizan automáticamente a las nuevas licencias estándar o completas (legado). Los admins de empresa pueden mejorar las licencias de forma manual.
