---
title: Cómo configurar el inicio de sesión único de Entra ID
article_id: 360022722233
translation_id: 360022722233
locale: es
sidebar_position: 5
created_at: '2019-05-07T12:03:08Z'
updated_at: '2025-11-25T16:04:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible para: plan Business y plan Enterprise Rol requerido: Admins de
    empresa'
---

> *💡 Se recomienda encarecidamente configurar el inicio de sesión único en una ventana en modo incógnito de tu navegador.* De esta manera, mantienes la sesión en la ventana estándar, lo que te permite desactivar la autorización de inicio de sesión único en caso de que algo esté configurado de forma incorrecta.

Si deseas configurar una instancia de prueba antes de habilitar el inicio de sesión único en producción, por favor [comunícate con el equipo de Soporte](https://help.miro.com/hc/requests/new?referer=help-center-article) para recibir asistencia. Solo se agregará a esta instancia de prueba a quienes configuren el inicio de sesión único.

> **⚠️ Consulta nuestro artículo principal sobre inicio de sesión único** [**aquí**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **para conocer las reglas, las funciones compatibles y la configuración opcional desde Miro.**

## Añadir y configurar la aplicación

 1. Encuentra la aplicación preconfigurada de Miro en la Galería de aplicaciones Enterprise de Entra ID ([Enterprise Applications](https://portal.Entra.com/#blade/Microsoft_AAD_IAM/StartboardApplicationsMenuBlade/AllApps/menuId/) > +Nueva aplicación).

2. Crea la aplicación y haz clic en **2.** **Configurar el inicio de sesión único** (o selecciona **inicio de sesión único** del lado izquierdo y selecciona el método de inicio de sesión **SAML**).

3. Verás que la **configuración básica de SAML** ya está en marcha:

:::warning
Si después de que todo esté configurado, el inicio de sesión único falla, intenta cambiar el ID de entidad de `https://miro.com` a `https://miro.com/`
:::

:::warning
La URL de inicio de sesión, el estado de relay y la URL de finalizar sesión (para el inicio de sesión único) deben quedar vacíos, ya que estas funcionalidades no son compatibles.
:::

Los **Atributos y Reclamos** también están en marcha:

:::warning
Ten en cuenta que:
a) la UPN se convertirá en el parámetro principal por el cual un usuario en Miro será reconocido y este parámetro no se podrá actualizar desde el lado de Entra. Cuando necesites actualizar los correos electrónicos de los usuarios en Miro sin usar SCIM, por favor [comunícate con nuestro equipo de soporte](https://help.miro.com/hc/requests/new?referer=help-center-article).
b) Miro acepta [**Nombre,** **Apellido**, **Nombre a mostrar** e **Imagen de perfil**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). Otros atributos no son compatibles mediante el inicio de sesión único, pero se pueden transferir mediante [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).
:::

### Creando el certificado

1. En Microsoft Entra, asegúrate de que la **Certificado de Firma SAML** > **Opción de Firma** sea **Firmar Aserción SAML** o **Firmar respuesta y aserción SAML**.

2. **Descargar** el **archivo Base64**.

## Configurar inicio de sesión único en tu plan de Miro

1. Abre el archivo **Base64** descargado en un editor de texto, y luego copia el certificado **x509** del archivo.

2. En Miro, en **Seguridad > Autenticación**, pega el certificado **x509** copiado en el cuadro de **Certificado Key x509**.

3. En la interfaz de configuración de Microsoft Entra, copia la **URL de inicio de sesión**, y luego dirígete a la página de **Seguridad > Autenticación** de Miro, y pégala en el cuadro de **URL de inicio de sesión de SAML**.

4. En la página de **Seguridad >**  **Autenticación** de Miro, en la sección **Usuarios de estos dominios iniciarán sesión usando inicio de sesión único**, asegúrate de agregar al menos un dominio de empresa.

:::warning
En Miro, asegúrate de que **Sincronizar fotos de perfil desde IdP** no esté seleccionado. Entra ID no admite la sincronización de fotos de perfil de usuario. Cuando la opción de **Sincronizar fotos de perfil desde IdP** no está seleccionada, los usuarios pueden establecer sus propias fotos de perfil.
:::

4. Haz clic en **Guardar**.

La configuración de SSO ya está completa.

## Cómo configurar los reclamos cuando UPN y el correo electrónico difieren

Puedes configurar los ajustes para usar cualquier atributo de Entra que esté en formato de correo electrónico como el **NameID** en Miro.

#### **Inicios de sesión iniciados por IdP y SP**

*Para el inicio de sesión iniciado por IdP*, Entra envía a Miro el valor que decides usar como el **NameID** (**usuario.mail**en el ejemplo a continuación).

Con este flujo, tus usuarios finales acceden a Miro mediante el ícono de la consola de su portal (por ejemplo, en `https://myapplications.microsoft.com/`). Desde allí, se envía una solicitud a Miro y *el usuario inicia sesión usando el **NameID** que definiste.*Miro espera que este atributo coincida con el **correo electrónico** del usuario en Miro. Una incompatibilidad resultará en la autenticación fallida.

*Para el inicio de sesión iniciado por SP*, Miro enviará una solicitud específicamente para la **UPN** del usuario y esperará que coincida con el **correo electrónico** del usuario en Miro. Una incompatibilidad resultará en la autenticación fallida.

Ahora, se espera que el campo de la **URL de inicio de sesión de SAML** en tus ajustes de Miro contenga la **URL de inicio de sesión** de la aplicación Miro de tu instancia de Entra. Esta será la URL a la que Miro dirigirá al usuario desde la [página de inicio de sesión de Miro](https://miro.com/sso/login/).

Cuando el usuario es dirigido a la URL de inicio de sesión desde la aplicación, se genera la solicitud de SAML. Con este flujo, el usuario inicia sesión con la dirección de correo que introdujo en la página de inicio de sesión de Miro y que Miro entonces solicita de Entra, requiriendo que sea el atributo UPN.

#### **Cómo configurar**

Para permitir que tus usuarios accedan a Miro con el **correo** de Entra en lugar de **UPN**, puedes completar el campo de **URL de inicio de sesión SAML** en Miro con la URL de la aplicación desde la consola de Entra. Luego, el flujo iniciado por SP será de la siguiente manera:

1. El usuario accede a Miro ingresando su correo de Miro, que es el correo que tienen en Miro. Miro comprende que la persona debe haber iniciado sesión en el perfil de usuario definido.
2. El usuario se dirige al enlace de su aplicación que se usa para el inicio de sesión iniciado por IdP.
3. El enlace usa el atributo  **NameID**  *que definiste* y lo envía a Miro.
4. Por lo tanto, el usuario se registra en Miro en el perfil de usuario definido previamente con el **NameID** que definiste.

Si deseas habilitar también el aprovisionamiento automático para Miro, consulta [este artículo](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).

Si tuviste algún problema durante la configuración, consulta [este artículo](../../../using-miro/tools/troubleshooting/10-i-can't-log-in-via-sso.md).

## Herramienta de prueba de Entra

Para llegar a la herramienta de prueba, elige la pestaña **Inicio de sesión único** en la configuración de tu aplicación y desplázate hasta la parte inferior de la sección.

Entra sugiere usar el proceso de inicio de sesión de prueba para verificar la conexión y solucionar un mensaje de error. Después de la prueba, recibirás instrucciones sobre cómo resolver la situación.

Ten en cuenta con qué credenciales administradas por Entra/ADFS se autentica tu estación de trabajo. Si intentas usar un conjunto diferente para iniciar sesión en Miro, el intento de inicio de sesión puede fallar, ya que el proveedor de identidad transfiere tu conjunto principal de credenciales y hay una incompatibilidad. Por ejemplo, esto puede ocurrir si eres el administrador de inicio de sesión único y pruebas el procedimiento de inicio de sesión bajo diferentes credenciales de usuario.

## Como alternativa, puedes probar en Miro

1. Completa los pasos anteriores para configurar tu configuración de inicio de sesión único.
2. Haz clic en el botón **Probar configuración de SSO**.
3. Revisa los resultados:
   1. Si no se encuentran incidencias, se mostrará un mensaje de confirmación **La prueba de configuración de SSO fue exitosa**.
   2. Si se encuentran incidencias, se mostrará un mensaje de confirmación **Error en la prueba de configuración de SSO**, seguido de mensajes de error detallados para guiarte sobre lo que hay que corregir.

##
