---
title: Cómo configurar el SSO de Google
article_id: 4716499382546
translation_id: 4716499382546
locale: es
sidebar_position: 6
created_at: '2022-03-18T18:12:44Z'
updated_at: '2025-11-25T16:08:20Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '**Disponible para: Plan Business y plan** Enterprise/strong> Configurado
    por: admins de empresa'
---

> Se recomienda enfáticamente configurar el SSO en una ventana en modo incógnito por separado del navegador. De esta manera, mantienes la sesión en la ventana estándar, lo que te permite desactivar la autorización de SSO en caso de que algo esté configurado de forma incorrecta.

Configurar Miro dentro de tu organización es más fácil que nunca con la app de integración que Google ha creado dentro de la Consola de administración del espacio de trabajo de Google. Esta app te permite configurar Google SSO para su uso con Miro, así como [el aprovisionamiento de usuarios SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/04-setting-up-automated-provisioning-with-google.md).

Este artículo se centra en la configuración de Google SSO para su uso con Miro.

Si deseas configurar una instancia de prueba antes de activar el SSO en la producción, solicítala a tu Account Executive o representante de Ventas. Solo se agregará a esta instancia de prueba a quienes configuren SSO.

:::tip
Consulta el [artículo sobre](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)  Miro [SSO](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)  para conocer las reglas, las funciones admitidas y los ajustes de configuración opcionales.
:::

Más información sobre la [configuración de Google SSO con Miro](https://support.google.com/a/answer/14100608#zippy=%2Cstep-set-up-google-as-saml-identity-provider) en el Centro de Ayuda de Google.

## Configurar Google SSO para Miro utilizando SAML

La configuración de Google SSO para autenticarse en Miro puede completarse en cuatro pasos:

1. Configurar Google como proveedor de identidad SAML
2. Configurar Miro como proveedor de servicios SAML
3. Activar Miro para usuarios
4. Prueba de autenticación

Configurar Google como proveedor de identidad SAML

1. Desde tu Consola de administración del espacio de trabajo de Google, haz clic en **Apps > Web y apps móviles**
2. En el panel Apps, haz clic en el menú desplegable **Añadir app**, elige "Buscar apps" y escribe "Miro".
3. Elige "Miro Web (SAML)" y haz clic en **Seleccionar**
4. En los "Detalles del proveedor de identidad de Google", en la Opción 2, comprueba que la "URL SSO", el "ID de entidad" y el "Certificado" están rellenados, y luego haz clic en **Continuar.** Copiarás estos valores más adelante cuando configures Miro
5. En los "Detalles del proveedor de servicios", añade los siguientes valores:
   **URL DE LA AEC:** https://miro.com/sso/saml
   **ID de entidad:** https://miro.com/
   **URL de inicio:** en blanco
   **Respuesta firmada:** dejar sin marcar
   ID de nombre CORREO ELECTRÓNICO
6. Haz clic en **Continuar**.
7. En "Asignación de atributos", en "Atributos del Directorio de Google", elige **Nombre** y luego **Apellido**, asegurándote de que se asignan a los atributos de la app.
8. Haz clic en **Finalizar**. Ahora verás tu app Miro añadida al Espacio de trabajo de Google
   ![google_sso_configuring_google_settings.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017515989394_google_sso_configuring_google_settings.gif)*Configurar el proveedor de identidad SAML de Google*

Configurar Miro como proveedor de servicios SAML

1. Abre una pestaña de incógnito en tu navegador e inicia sesión en el panel de Miro (miro.com/app/dashboard).
2. Haz clic en tu avatar en la esquina superior derecha y haz clic en **Configuración**
3. En la configuración de tu Empresa, haz clic en **Autenticación.** Si eres cliente de un plan Business, esta configuración está en **Seguridad**.
4. Haz clic en el conmutador para "Activar SSO para configurar el aprovisionamiento SCIM"
5. Accederás a la sección Autenticación de la configuración de la empresa. Haz clic en el conmutador **SSO/SAML**. Se te pedirá que hagas clic en **Activar** para habilitar el SSO para tu organización.
6. Para obtener **la URL de inicio de sesión SAML**, vuelve a tu Consola de administración del espacio de trabajo de Google y, dentro de la app Miro, haz clic en **DESCARGAR METADATOS.** Este panel te da la opción de copiar los valores necesarios
7. En **URL SSO**, haz clic en el botón **Copiar**. Vuelve a Miro y pega el valor en **URL de inicio de sesión SAML**
8. Repite este proceso para el **Certificado clave x.509** utilizando el Certificado en Google
9. Añade la información de tu **dominio**. Asegúrate de que ya has [configurado y verificado tu dominio](../../canvas-25-admin-features/domain-control/01-domain-control.md)
10. Haz clic en **Guardar![google_sso_configuring_miro_authentication.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017515990802_google_sso_configuring_miro_authentication.png)***Configuración de los ajustes de autenticación SSO en Miro*

Activar Miro para usuarios

1. Volver a la consola de administración del espacio de trabajo de Google
2. Si es necesario, haz clic en **Web y apps móviles** en el menú Apps y selecciona **Miro**
3. Haz clic en **Acceso usuarios**
4. Pulsa **ON para todos** y pulsa **Guardar![google_sso_turning_on_miro.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017528995474_google_sso_turning_on_miro.gif)***Activar la app Miro para todos los usuarios*

Si quieres activar Miro para unidades organizativas concretas, haz clic primero en el grupo en Unidades organizativas y, a continuación, haz clic en **ON.** Es posible que tengas que pulsar adicionalmente **SOBREPASAR** o **HEREDAR**.

Prueba de autenticación

1. En la Consola de administración del espacio de trabajo de Google, inicia la app Miro si es necesario.
2. En la sección Miro, haz clic en **PRUEBA DE CONEXIÓN SAML**
3. Debería aparecer una nueva pestaña con las opciones de inicio de sesión de Google SSO
   .GIF
4. Para probar la autenticación en Miro, abre una nueva pestaña de incógnito e inicia el panel de Miro (miro.com/app/dashboard).
5. Deberías ver una página de inicio de sesión. Haz clic en **Iniciar sesión con Inicio de sesión único** e inicia sesión con las credenciales de tu cuenta.
   ![google_sso_prueba_autenticacion.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017528996882_google_sso_testing_authentication.gif)*Probando la autenticación Google SSO con Miro*

También puedes hacer la prueba en Miro:

1. Completa los pasos anteriores para configurar tus ajustes SSO.
2. Haz clic en el botón **Probar configuración SSO**.
3. Revisa los resultados:
   1. Si no se encuentra ningún problema, se mostrará un mensaje de confirmación de que **la prueba de configuración SSO se ha realizado correctamente**.
   2. Si se encuentran problemas, se mostrará un mensaje de confirmación **Prueba de configuración SSO fallida**, seguido de mensajes de error detallados para orientarte sobre lo que hay que arreglar.![prueba-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)*Prueba de configuración SSO desde Miro*

> **⚠️** Si has configurado previamente el SSO para tu organización y necesitas volver a configurarlo, se recomienda encarecidamente **desactivar** el SSO en Miro antes de continuar en Google Admin Console; de lo contrario, podrías bloquearte a ti mismo en Miro. Para evitar un bloqueo, crea un usuario "rompe el cristal" con un correo electrónico con un dominio ajeno al que aparece en la configuración del SSO, como acmebreaktheglass@gmail.com. De lo contrario, puedes comunicarte con el servicio de Soporte y este puede deshabilitar el SSO para toda la organización.

Si quieres configurar el[aprovisionamiento de](../../security-integrations/system-for-cross-domain-identity-management-scim/04-setting-up-automated-provisioning-with-google.md)usuarios con Google, encontrarás instrucciones en el artículo "[Configurar el aprovisionamiento automatizado con Google](../../security-integrations/system-for-cross-domain-identity-management-scim/04-setting-up-automated-provisioning-with-google.md)".
