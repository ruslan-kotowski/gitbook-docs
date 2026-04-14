---
title: Agregar múltiples proveedores de identidad
article_id: 16287287497234
translation_id: 16287287497234
locale: es
sidebar_position: 1
created_at: '2024-01-10T10:51:24Z'
updated_at: '2026-02-18T08:59:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible para: Enterprise Configurado por: Admins de empresa'
---

:::note
Añadir múltiples proveedores de identidad es una función privada disponible exclusivamente para los clientes de Enterprise. Para acceder y habilitar esta función, contacta a tu Gerente de Cuenta de Miro o Gerente de Customer Success. El soporte de Miro no puede habilitar esta función.
:::

Usa varios proveedores de identidad (IdPs) para el inicio de sesión único (SSO). Esto es especialmente útil para grandes organizaciones con distintas sucursales o subsidiarias, cada una con su propio IdP pero que necesitan acceso a la misma suscripción de Miro.

## Preparación para añadir múltiples proveedores de identidad

Para asegurarse de que el [inicio de sesión único (SSO)](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) continúe funcionando después de agregar múltiples aplicaciones de proveedor de identidad, debes actualizar la configuración de la aplicación de IdP existente.

Entra ID y algunos otros IdP no admitirán el nuevo formato de configuración hasta que tu organización habilite la función privada de múltiples proveedores de identidad (multi-IdP). Para evitar interrupciones en el inicio de sesión, sugerimos organizar una llamada con tu gerente de Customer Success, quien te guiará paso a paso para habilitar la función privada de multi-IdP al mismo tiempo que se actualiza la configuración.

### Cómo configurar tus ajustes de Enterprise

1. Desactiva SCIM.
2. Actualiza la configuración de SSO.
3. Verifica tu funcionalidad de SSO.

#### Desactivar SCIM

Actualmente no ofrecemos soporte para [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) con múltiples IdPs. Para desactivar SCIM en tu plan Enterprise, ve a **Preferencias** > **Cuenta** > **Integraciones de Enterprise** y desactiva **SCIM Provisioning**.

#### Actualizar la configuración de SSO

**Configuración antigua**

Cuando el inicio de sesión único (SSO) de Miro fue configurado originalmente en tu IdP, es probable que se hayan utilizado los siguientes valores de configuración:

- **URL de Callback/ACS:** https://miro.com/sso/saml
- **ID de entidad:** https://miro.com

**Nueva configuración**

Para asegurar que el IdP sepa a cuál configuración dentro de Miro se refiere, los valores a continuación deben ser actualizados. Ve a **Configuración** > **Seguridad** > **Autenticación**.

Estos valores están disponibles en la configuración de inicio de sesión único una vez que tu organización haya habilitado la función privada de múltiples IdP y tendrán el siguiente formato:

- **Callback URL/ACS:** https://miro.com/sso/saml/&lt;org_id&gt;/&lt;saml_settings_id&gt;
- **Entity ID:** "https://miro.com/&lt;org_id&gt;/&lt;saml_settings_id&gt;

![Callback URL and Entity ID in the Enterprise admin console](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/23763575205778_image.png)

*Callback URL and Entity ID in the Enterprise admin console*

#### Verifica la funcionalidad de tu inicio de sesión único

Una vez que hayas terminado de actualizar la configuración de tu IdP, prueba que el inicio de sesión único esté funcionando correctamente cerrando sesión y volviendo a iniciar sesión.

## Agregar un nuevo proveedor de identidad (IdP)

El proceso para añadir nuevos IdP es similar a la [configuración de SSO](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) existente, pero incluye un par de cambios clave:

- **Nuevos campos:** 'Nombre de IdP' y 'Descripción de IdP' (opcional). Estos campos ayudan a los usuarios y admins a identificar el IdP correcto durante el inicio de sesión, especialmente si se utilizan múltiples IdPs.

  Debido a que estos campos se muestran en la configuración de administrador y pueden ser visibles para los usuarios cuando inician sesión a través de un inicio de sesión único, recomendamos encarecidamente definir estos nombres intencionalmente (por ejemplo, Unidad de Negocio o nombre del IdP).

  ![idP-name-and-IdP description.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016020733970_idP-name-and-IdP%20description.png)
*La opción para agregar un nombre de IdP y una descripción de IdP*
- **Campos de solo lectura:** 'URL de devolución de llamada' (URL de devolución permitida, URL del servicio de consumidor de aserciones personalizado, URL de respuesta) y 'ID de entidad' (Identificador, Identificador de confianza de la parte que confía) ahora se generan automáticamente en tu configuración de IdP de Miro una vez que tu organización ha habilitado la función privada de múltiples IdP.

  Anteriormente, estos valores eran estáticos ya que eran los mismos para todas las configuraciones de IdP. Una vez generados, también necesitarás copiar y pegar estos valores en los campos correspondientes en la configuración de tu proveedor de IdP.

  ![Callback-ID-and-Entity-ID-fields.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016034166290_Callback-ID-and-Entity-ID-fields.png)
*Campos de URL de devolución de llamada e ID de entidad*

## Gestión de múltiples proveedores de identidad (IdPs)

> **💡** Puedes añadir y habilitar hasta 20 proveedores de identidad a la vez.

Después de agregar los IdPs, cada configuración se puede activar o desactivar según sea necesario. Para desactivar un IdP, ve a **Configuración de la empresa** > **Cuenta** > **Autenticación**, y desactiva el IdP.

![Toggle-on-or-off-IdPs.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016034165010_Toggle-on-or-off-IdPs.png)
*La opción para activar o desactivar un IdP*

## Vista de inicio de sesión para dominios de correo electrónico con múltiples IdPs

Si el dominio de correo electrónico de un usuario está vinculado a varias configuraciones de IdP, pueden seleccionar una durante el inicio de sesión. Si estas configuraciones tienen dominios distintos, el usuario es direccionado automáticamente al IdP correspondiente.

![sso-screenshot.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/22437449166610_sso-screenshot.png)
*Vista de múltiples IdPs al iniciar sesión*
