---
title: Aprovisionamiento de usuarios en el plan Enterprise
article_id: 4403139914130
translation_id: 4403139914130
locale: es
sidebar_position: 13
created_at: '2021-07-01T07:59:23Z'
updated_at: '2025-11-25T16:05:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: scim
---

Con el aprovisionamiento automático, todos los nuevos usuarios dentro de tus dominios corporativos son dirigidos a tu suscripción de Enterprise y obtienen acceso a los activos de tu empresa.

Miro Enterprise proporciona varias opciones de aprovisionamiento: invitaciones, aprovisionamiento Just-in-Time (JIT), System for Cross-domain Identity Management (SCIM) y control de dominios.

> **Disponible para:** Plan Enterprise

## Invitaciones

Puedes invitar a usuarios a tu suscripción utilizando el botón **Invite members** en tu panel. Las invitaciones se envían de inmediato y no requieren ninguna configuración adicional.

Aprende más sobre cómo compartir tu trabajo y colaborar en Miro visitando [Administrar invitaciones en el plan Enterprise](05-manage-user-invitations-on-enterprise-plan.md) y [Compartir tableros e invitar a colaboradores](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).

![invite_members_button.jpg](../../../../../../docs/enterprise-administration/user-management/images/21017653284754_invite%20members%20button.jpg)*La opción para invitar miembros en el panel de Miro*

## Aprovisionamiento "justo a tiempo" (JIT)

El aprovisionamiento Just-in-Time (JIT), integrado con [inicio de sesión único (SSO)](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), añade automáticamente todos los nuevos usuarios registrados bajo tus dominios corporativos de SSO a un equipo específico en tu Plan Enterprise.
El aprovisionamiento JIT puede habilitarse fácilmente en la configuración de SSO de Miro. Aprende [cómo configurar SSO](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md).

![user_provisioning_jit_provisioning.png](../../../../../../docs/enterprise-administration/user-management/images/21017682931730_user_provisioning_jit_provisioning.png)*Habilitando el aprovisionamiento Just-in-Time (JIT) en la configuración de SSO*

## Sistema para la gestión de identidad entre dominios (SCIM)

SCIM, integrado con [inicio de sesión único (SSO)](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), te permite aprovisionar y administrar automáticamente a los usuarios en tu plan Enterprise a través de tu proveedor de identidad (IdP) elegido.

Con SCIM habilitado, puedes añadir usuarios a equipos específicos, actualizar sus detalles y correos electrónicos, y gestionar su estado de activación directamente dentro de tu IdP elegido. Esta función automatiza el intercambio de información de usuario entre tu cuenta de Miro y tu IdP.

SCIM automatiza el intercambio de información de usuario entre Miro y tu IdP, permitiéndote administrar el acceso de los empleados a tu plan Enterprise de forma centralizada desde el IdP.

Conoce más sobre las [funciones de SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) y revisa los pasos de configuración para [Entra ID](../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md), [OKTA](../security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md) o [OneLogin](../security-integrations/system-for-cross-domain-identity-management-scim/06-setting-up-automated-provisioning-with-onelogin.md).

## Control de dominio

[Control de dominio](../canvas-25-admin-features/domain-control/01-domain-control.md) te permite agregar automáticamente nuevos usuarios a tu suscripción de Enterprise, limitar la capacidad de los usuarios corporativos para crear suscripciones de Miro separadas y monitorear la actividad de los usuarios dentro de tu dominio.

Con el control de dominio, puedes establecer una regla de aprovisionamiento para tus usuarios corporativos:

- los usuarios recién registrados en tu dominio pueden solicitar acceso a tu suscripción
- los usuarios recién registrados en tu dominio se unen automáticamente a tu suscripción
- los usuarios recién registrados en tu dominio se unen automáticamente a tu suscripción y los usuarios de tu dominio no tienen permitido crear nuevos equipos de Miro

![Add-a-domain-Image1.png](../../../../../../docs/enterprise-administration/user-management/images/21017653288082_Add-a-domain-Image1.png)*Control de dominio en la configuración de seguridad de Miro*

## Cómo funciona la asignación de licencias

Cuando invitas a usuarios nuevos, los admins de empresa pueden elegir una licencia para el invitado en función de la configuración de la suscripción.

Los usuarios invitados por personas que no sean admins o que se hayan aprovisionado automáticamente a tu suscripción a través de JIT, SCIM o control de dominio, recibirán la *licencia predeterminada*:

- **para planes con licencias no flexibles (no FLP):** la licencia predeterminada es una licencia con acceso completo (si la organización tiene licencias con acceso completo insuficientes, los usuarios detectados automáticamente obtendrán una [licencia gratuita limitada](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md)).
- **para planes con el Programa de Licencias Flexibles (PLF):** la licencia predeterminada puede ser Free o [licencia gratuita limitada](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).

:::note
Aprende más sobre nuestros [modelos de licencias Enterprise](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md), [administración de licencias en el Programa de licencias flexibles](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md), cómo gestionar la asignación y mejora de licencias con [administración de solicitudes](09-request-management-on-enterprise-plan.md), y cómo seguir el uso de licencias con [gestión de activos de software](../security-integrations/software-asset-management/01-software-asset-management-miro-enterprise.md).
:::

## Preguntas frecuentes

Cuando el control de dominio está configurado para capturar nuevos usuarios, ¿funciona de manera similar a JIT al asignar automáticamente usuarios con dominios específicos a un equipo por defecto dentro de la suscripción Enterprise?

Sí, pero el control de dominio no requiere que el SSO esté configurado para el plan Enterprise. Puede funcionar sin SSO.

¿Podemos evitar que los usuarios aprovisionados automáticamente reciban una licencia con acceso completo hasta que empiecen a trabajar activamente en un tablero?

Sí, esto es posible con el [Programa de licencias flexibles](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).

¿Puedo configurar varias opciones de aprovisionamiento para mi suscripción Enterprise?

Sí, puedes usar múltiples opciones de aprovisionamiento al mismo tiempo.
