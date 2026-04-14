---
title: Bloquear usuarios desactivados
article_id: 11846063620882
translation_id: 11846063620882
locale: es
sidebar_position: 2
created_at: '2023-06-06T12:47:53Z'
updated_at: '2025-11-04T11:30:33Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-deactivation
---

Cuando un admin de empresa [desactiva a un usuario](01-deactivated-users.md), el usuario pierde el acceso a la suscripción Enterprise y ya no puede iniciar sesión con SSO. Los usuarios desactivados mantienen su acceso a otras suscripciones de Miro con el mismo correo electrónico.

También puedes bloquear a los [usuarios gestionados](06-managed-users-on-enterprise-plan.md) que hayas desactivado para evitar que accedan a otras suscripciones de Miro.

> **Disponible para:** plan Enterprise
> **Quién puede hacerlo:** admins de empresa

## Bloquear usuarios desactivados

**Cuando se active la configuración:** se bloqueará a los usuarios gestionados desactivados para que no puedan acceder a ninguna suscripción de Miro. Esta configuración se aplica a todos los usuarios que actualmente estén desactivados en tu suscripción y a cualquier usuario que desactives en el futuro.

**Cuando se desactive la configuración:** los usuarios gestionados desactivados mantendrán su acceso a otras suscripciones de Miro con su correo electrónico corporativo y su contraseña.

> Habilitar la configuración **Bloquear usuarios desactivados** afectará a todos los usuarios previamente desactivados en tu suscripción. Te recomendamos que antes de habilitar la configuración o verificar nuevos dominios mientras habilitas la configuración revises primero tu lista de usuarios desactivados para entender a quién se bloqueará.

### Cómo bloquear usuarios desactivados

1. Ve a **Configuración** > **Seguridad** > **Dominios gestionados**
2. Activa la opción **Bloquear usuarios desactivados**
   *![Bloquear usuarios desactivados en la consola de admins de empresas](../../../../../../docs/enterprise-administration/user-management/images/23921780232082_image.png)*
   *Bloquea a los usuarios desactivados en la consola de admins de empresas.*

## ¿Qué ven los usuarios bloqueados?

La sesión de los usuarios gestionados desactivados bloqueados se cerrará inmediatamente. La próxima vez que intenten iniciar sesión, verán uno de los siguientes mensajes:

![Cuenta](../../../../../../docs/enterprise-administration/user-management/images/21017430794898_Account%20deactivated.png)*El usuario intentó iniciar sesión con correo electrónico y contraseña*

![Correo electrónico](../../../../../../docs/enterprise-administration/user-management/images/21017417753746_Email%20not%20associated%20with%20an%20SSO%20account.png)*El usuario ha intentado iniciar sesión con SSO*

## Desbloquear usuarios desactivados

Los admins de empresa pueden desbloquear usuarios de tres maneras:

**Reactivar o volver a invitar al usuario**

Reactiva o vuelve a invitar al usuario a tu suscripción Enterprise donde se verifica el dominio. Este usuario obtiene acceso a todas las suscripciones de las que forma parte. Si no está usando activamente tu suscripción Enterprise, puedes asignarle una licencia [gratuita limitada](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md). Obtén más información sobre cómo invitar a miembros enGestionar invitaciones en el plan Enterprise.

**Desactiva la configuración Bloquear usuarios desactivados**

Esto desbloqueará a todos los usuarios gestionados desactivados y se les permitirá iniciar sesión en Miro con su correo electrónico corporativo. Esto no les dará acceso a tu suscripción Enterprise. Esta opción solo funciona si el usuario no ha sido eliminado de la suscripción. Ve a la configuración **Dominios gestionados** y desactiva **la opción Bloquear usuarios desactivados.**

**Eliminar el dominio**

Puedes eliminar el dominio de tu lista de dominios verificados. Esto desbloqueará a todos los usuarios gestionados de ese dominio, a menos que hayan sido eliminados de la suscripción. Para eliminar un dominio, en tu configuración de la empresa, ve a **Seguridad y cumplimiento** > **Colaboración** > haz clic en **Eliminar**, junto al nombre del dominio.

> **✏️** Bloquear el acceso de un usuario a Miro implica que no podrá iniciar sesión en otras suscripciones de Miro ni a través de SSO ni con su correo electrónico corporativo y su contraseña. Desbloquear al usuario no le da acceso a la suscripción Enterprise a menos que se le otorgue acceso explícitamente.

## Escenarios de bloqueo de usuarios

Usa esta tabla para entender mejor lo que sucede en los diferentes escenarios de bloqueo de usuarios.

|  |  |
| --- | --- |
| Acción | Resultado |
| **El usuario se bloquea** | |
| El admin de empresa desactiva al usuario gestionado | El usuario se bloquea |
| **Un miembro de tu suscripción Enterprise intenta invitar a un usuario gestionado** desactivado a su equipo | El usuario permanece bloqueado.  Quien invita verá un mensaje que aclarará que el usuario está desactivado. No se pueden invitar. Los admins pueden reactivar usuarios. |
| El admin de empresa desactiva y elimina a un usuario gestionado | El usuario se bloquea |
| El usuario gestionado se desactiva en IdP | El usuario se bloquea |
| El usuario gestionado se elimina de la aplicación/grupo de Miro en IdP | El usuario se bloquea |
| El admin de empresa agrega y verifica un dominio mientras la configuración está habilitada | Se bloquean todos los usuarios de los dominios recién verificados en la lista desactivada. |
| Alguien de otra suscripción (cualquier otra suscripción además de la que verifica el dominio) intenta invitar a tu usuario gestionado desactivado a su suscripción.   Esto también se aplica incluso si el usuario gestionado se elimina de tu suscripción. | El usuario permanece bloqueado.  Podrán recibir invitaciones a otras suscripciones y recibirán notificaciones de invitaciones, pero no podrán iniciar sesión en Miro. |
| **El usuario se desbloquea** | |
| El admin de empresa reactiva a un usuario gestionado desactivado | El usuario se desbloquea |
| El admin de empresa invita a un usuario gestionado desactivado o eliminado a volver a la suscripción. | El usuario es invitado y desbloqueado |
| El usuario gestionado se reactiva a través de SCIM | El usuario se desbloquea |
| Se vuelve a agregar al usuario gestionado a la aplicación/grupo de Miro en IdP y se sincroniza a través de SCIM | El usuario se desbloquea |
| **Un miembro de tu suscripción Enterprise invita a un** usuario gestionado eliminado a su equipo | Si la [configuración de invitaciones](03-invitation-settings-on-enterprise-plan.md) les permite a los miembros invitar a usuarios nuevos a sus equipos, se invita y se desbloquea al usuario. |
| **Escenarios mixtos** | |
| El dominio verificado se elimina del Control de dominio | Los usuarios desactivados se desbloquean del dominio eliminado.  Los usuarios eliminados permanecen bloqueados y deben volver a invitarlos a la suscripción para que se desbloqueen. |
| La configuración se deshabilita después de que se haya habilitado. | Todos los usuarios desactivados gestionados se desbloquean.  Los usuarios eliminados permanecen bloqueados y deben volver a invitarlos a la suscripción para que se desbloqueen. |

## Preguntas frecuentes

**¿Qué pueden ver otras suscripciones sobre usuarios desactivados bloqueados?**

Desactivar al usuario en tu suscripción lo desactivará solo en tu suscripción Enterprise. El bloqueo solo afectará a la capacidad de iniciar sesión en Miro usando el correo electrónico corporativo. El usuario parece activo en otras suscripciones, pero no puede iniciar sesión con su dirección de correo electrónico corporativa.

**Si se desactiva y elimina a un usuario, ¿se le bloqueará el acceso a Miro una vez que se habilite la configuración?**

Los usuarios permanecerán bloqueados después de que [los elimines de tu suscripción](01-deactivated-users.md). Eliminar al usuario tendrá algunas consecuencias: para más información, consulta nuestros escenarios de usuarios bloqueados y desactivados. La única manera de desbloquear a un usuario eliminado es volver a invitarlo a la suscripción con el dominio verificado. Si se elimina al usuario de la suscripción antes de habilitar la configuración, esto no aplica a ese caso.

**¿Esta configuración afecta a los usuarios no gestionados?**

No. Esta configuración solo afecta a los usuarios gestionados.
