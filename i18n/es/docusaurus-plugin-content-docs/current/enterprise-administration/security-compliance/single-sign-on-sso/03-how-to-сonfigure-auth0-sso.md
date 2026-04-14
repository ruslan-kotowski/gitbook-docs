---
title: Cómo сonfigurar Auth0 SSO
article_id: 360022496573
translation_id: 360022496573
locale: es
sidebar_position: 3
created_at: '2019-05-01T18:33:32Z'
updated_at: '2025-02-26T11:43:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '**Disponible para: Plan Business y plan** Enterprise/strong> Configurado
    por: admins de empresa'
---

*Se recomienda encarecidamente configurar la característica en una ventana en modo incógnito por separado del navegador.* *De esta manera, mantienes la sesión en la ventana estándar, lo que te permite desactivar la autorización de SSO en caso de que algo esté configurado de forma incorrecta.*

Si deseas configurar una instancia de prueba antes de activar SSO en la producción, solicítala a tu Account Executive o representante de ventas de Miro. Solo se agregará a esta instancia de prueba a quienes configuren SSO.

## Cómo crear la aplicación de Miro dentro de tu usuario

1. Crea la aplicación en tu lista de **Applications** (Aplicaciones).
   botón_crear_aplicación.jpg
   *Sección de aplicaciones Auth0*
2. Selecciona el tipo de aplicación **Aplicaciones Web normales**.
   lista_tipos_aplicaciones.jpg
   *Lista de tipos de aplicación*
3. Ve a la pestaña **Settings** (Ajustes) y asegúrate de que las opciones que aparecen hayan sido seleccionadas exactamente de la manera que se describe a continuación.
   ![mceclip0.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017725482002_mceclip0.png)


   |  |  |
   | --- | --- |
   | **Token Endpoint Authentication Method (Método de autenticación de endpoint mediante token)** | POST |
   | **Allowed Callback URL** (URL de devolución de llamada permitidas) | `https://miro.com/sso/saml` |
   | **Application Login URI (URI de inicio de sesión de la aplicación)** | `https://miro.com/sso/saml` |
   | **Allowed Origins (CORS)** (Orígenes permitidos de CORS) | `https://miro.com/` |
   | **JWT Expiration** (Expiración de JWT) | 36000 (predeterminado) |
4. Haz clic en **Mostrar configuración avanzada:**
   mceclip1.png

   y luego ve a **Certificados** y Copia tu Certificado de Firma x509:
   copiar_el_certificado.jpg
   *Pestaña Configuración avanzada en Auth0*
5. Cambia a Miro y abre tu configuración de SSO (los admins del plan Business encontrarán la configuración en la pestaña **Seguridad**, los admins del plan Enterprise tendrán que ir a la pestaña **Integraciones de empresa** ) y luego pega el **certificado de firma x509** en el campo correspondiente, como se muestra en la captura de pantalla de abajo:
   certificado_en_ajustes_SSO_Miro.jpg
   *Pestaña **Seguridad** de Miro con ajustes SAML*

## Configurar SAML para la aplicación

1. Vuelve a la página de configuración de la aplicación Auth0 y elige la pestaña **Complementos** y el complemento **SAML2**:
   catálogo_de_complementos.jpg
   *Catálogo de complementos de Auth0*Verás una ventana emergente con la configuración de la solicitud y la URL de devolución de llamada de la aplicación **:
   ajustes_de_complementos.jpg***Pestaña **Configuración** del addon*
2. Asegúrate de que la **URL** está configurada en **`https://miro.com/sso/saml`**La **configuración de** la solicitud debe ser la siguiente:

   ```
    "nameIdentifierFormat": "urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress",
    "nombreIdentificadorSondas": [
    "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress"
   ```
3. Cambia las pestañas a **Uso** y copia la URL de inicio de sesión del proveedor de identidad **:
   mceclip2.png
   *Campo URL de inicio de sesión del proveedor de identidad en Auth0***
4. Cambia a Miro nuevamente y pega la URL en el campo**SAML Sign-in URL** (URL de inicio de sesión de SAML).
5. Haz clic en **Save** (Guardar) para que los ajustes se apliquen a tu plan de Miro.

## Verificación y configuración

Ahora puedes regresar a la consola de Auth0 y volver a la pestaña **Settings** (Ajustes) del complemento.  Haz clic en Debug (Depurar) para activar el intento de inicio de sesión.

depurar.jpg
Activación del intento de inicio de sesión

Esto activará el intento de inicio de sesión de IdP y te permitirá ver los resultados.

Si tienes alguna dificultad, [comunícate con nuestro equipo de Soporte](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).

## Probar la configuración de SSO en Miro

1. Completa los pasos anteriores para configurar tus ajustes SSO.
2. Haz clic en el botón **Probar configuración SSO**.
3. Revisa los resultados:

- Si no se encuentra ningún problema, se mostrará un mensaje de confirmación de que **la prueba de configuración SSO se ha realizado correctamente**.
- Si se encuentran problemas, se mostrará un mensaje de confirmación **Prueba de configuración SSO fallida**, seguido de mensajes de error detallados para orientarte sobre lo que hay que arreglar.

![prueba-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*Probar la configuración de SSO en Miro*
