---
title: Cómo configurar el SSO de OKTA
article_id: 360023901054
translation_id: 360023901054
locale: es
sidebar_position: 7
created_at: '2019-05-31T11:32:41Z'
updated_at: '2025-11-25T16:05:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible para: [Empresa](../../../plans-billing/miro-plans/04-enterprise-plan.md),
    planes [Business](../../../plans-billing/miro-plans/06-business-plan.md) Configurado
    por: admins de empresa'
---

> *Se recomienda enfáticamente configurar el SSO en una ventana en modo incógnito por separado del navegador.* De esta manera, mantienes la sesión en la ventana estándar, lo que te permite desactivar la autorización de SSO en caso de que algo esté configurado de forma incorrecta.

[Si quieres configurar una instancia de prueba antes de habilitar el SSO en la producción, comunícate con el equipo de Soporte para obtener asistencia.](https://help.miro.com/hc/requests/new?referer=help-center-article) Solo se agregará a esta instancia de prueba a quienes configuren SSO.

> **⚠️ Consulta aquí nuestro artículo principal sobre SSO** **para conocer las reglas, las funciones compatibles y la configuración opcional desde Miro.**

## Configuración de Okta

### Cómo añadir y configurar la aplicación

Haz clic en la pestaña **Applications** (Aplicaciones) y elige **Browser App Catalogue** (Catálogo de aplicaciones para navegador):

![browse_app_catalog.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928758930_browse%20app%20catalog.jpg)
Sección de aplicaciones en Okta

Encuentra nuestra aplicación preconfigurada para una instalación fácil y haz clic en **Add** (Agregar):

![Miro_pre-configured_app.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928759570_Miro%20pre-configured%20app.jpg)
Miro en el catálogo de aplicaciones de Okta

Ponle a la aplicación en tu galería la etiqueta que prefieras (otros pasos son opcionales) y haz clic en **Next** (Siguiente) para cambiar a la pestaña **Sign-On options** (Opciones de inicio de sesión):

![general_settings.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928760466_general%20settings.jpg)
Ajustes generales de la aplicación de Miro

En **Sign-On Options** (Opciones de inicio de sesión) ya están completados todos los valores esperados y no se requieren más datos.

:::warning
Puedes agregar valores personalizados si lo prefieres, pero asegúrate de que el **Default Relay State** (Estado de retransmisión predeterminado) se mantenga *vacío*: nuestras aplicaciones independientes emplean el redireccionamiento al navegador del usuario final durante el procedimiento de autenticación y generan valores de RelayState únicos para ello. Si usas un valor predeterminado, Okta sobrescribirá nuestros datos y tus usuarios solo podrán acceder a la versión de navegador de Miro, pero no a las aplicaciones independientes (de escritorio, para tableta, para dispositivos móviles).
:::

![sign-on_options.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016941715730_sign-on%20options.jpg)
Métodos de inicio de sesión

Haz clic en **Finish** (Finalizar). Podrás volver y editar cualquier campo más tarde si es necesario.

### Formato de nombre de usuario

> El **formato de nombre de usuario de la aplicación** está establecido de manera predeterminada como el **nombre de usuario de Okta**, que está bien si tu nombre de usuario está en formato de correo electrónico. Como alternativa, establece el nombre de usuario como **email.**

:::warning
El correo electrónico es la identidad principal con la cual se reconoce al usuario en Miro y no debería actualizarse en Okta, a menos que tengas habilitado SCIM. Si no usas SCIM, pero necesitas actualizar las direcciones de los usuarios finales, comunícate con nuestro [equipo de Soporte](https://help.miro.com/hc/requests/new?).
:::

### Configuración de imágenes de perfil (opcional)

La configuración de un atributo personalizado, como la imagen de perfil, puede considerarse un proceso independiente. Sigue esta [guía](https://drive.google.com/file/d/1go4BJWzFpQS5R04WdN1Q4O5Dy93k4wGp/view) para establecer el atributo en Okta y, luego, [habilita el requisito de imagen de perfil](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) en Miro.

## Configuración de Miro

Desplázate hacia abajo a **SAML Signing Certificates** (Certificados de firma de SAML) para obtener los metadatos de IDP. Si no tienes certificados emitidos, primero crea uno.

Después de eso, haz clic en **Actions** (Acciones) y elige **View IdP metadata** (Ver metadatos de IdP) de esta forma:

![view_Idp_metadata.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928761234_view%20Idp%20metadata.jpg)
Obtener los metadatos de IdP

Se te dirigirá a una pestaña aparte que contiene toda la información.  Copia el certificado desde la línea que comienza con &lt;ds:X509Certificate&gt; y pégalo en los ajustes de SSO de Miro en el campo Key x509 Certificate/span>**.**

![certificate_in_Miro_SSO_settings.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928761746_certificate%20in%20Miro%20SSO%20settings.jpg)
 /span>Certificado Key x509 en ajustes de SSO de Miro

Regresa a la página de metadatos y copia la URL desde la línea **SingleSignOnService** después de **Location=**y pégala en **SAML Sign-in URL** (URL de inicio de sesión de SAML).

¡Listo!

Como paso final de los ajustes de Miro, agrega tus dominios y [verifícalos](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). También puedes configurar los ajustes opcionales.

Si tienes algún problema, consulta [nuestra lista de casos comunes y cómo resolverlos.](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)

## Probar la configuración de SSO en Miro

1. Completa los pasos anteriores para configurar tus ajustes SSO.
2. Haz clic en el botón **Probar configuración SSO**.
3. Revisa los resultados:

- Si no se encuentra ningún problema, se mostrará un mensaje de confirmación de que **la prueba de configuración SSO se ha realizado correctamente**.
- Si se encuentran problemas, se mostrará un mensaje de confirmación **Prueba de configuración SSO fallida**, seguido de mensajes de error detallados para orientarte sobre lo que hay que arreglar.

![prueba-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*Probar la configuración de SSO en Miro*
