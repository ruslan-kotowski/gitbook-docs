---
title: Autenticación de dos factores (2FA) para empresas – guía del usuario
article_id: 7935469290002
translation_id: 7935469290002
locale: es
sidebar_position: 2
created_at: '2022-10-04T09:00:42Z'
updated_at: '2025-11-06T13:50:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Relevante para: Starter, Business, Education, Enterprise'
---

## Qué es la autenticación de dos factores (2FA)

La autenticación de dos factores (2FA) añade más seguridad a tus cuentas online. Cuando tu admin de empresa activa la autenticación de dos factores (2FA), cada inicio de sesión en Miro con tu correo electrónico y contraseña estará seguido por una capa adicional de seguridad. Este paso extra asegura una mayor protección para tu cuenta, requiriendo verificación más allá de tus credenciales habituales de inicio de sesión.

:::tip
Aprende cómo habilitar la autenticación de dos factores (2FA) para tu organización en los [planes Enterprise](../../security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md) y en [todos los demás planes](../../../administration/security-compliance/01-two-factor-authentication-2fa.md).
:::

## Cómo configurar la autenticación de dos factores (2FA)

**Usuarios nuevos:** Durante tu proceso de [registro](https://miro.com/signup/) con tu correo electrónico corporativo, se te solicitará habilitar 2FA.
**Usuarios existentes:** En tu próximo [inicio de sesión](https://miro.com/login/), si tu organización requiere 2FA y no estás utilizando inicio de sesión único (SSO), se te solicitará configurar 2FA.

1. Descarga una aplicación de autenticación en tu dispositivo móvil. Las aplicaciones de autenticación, como Google Authenticator, Microsoft Authenticator y Authy, generan un código de un solo uso basado en el tiempo (TOTP) para accesos seguros a Miro. Para obtener orientación sobre cuál aplicación de autenticación elegir, consulta a tu admin de empresa o administrador de TI.

2. Haz clic en **Tengo una aplicación de autenticación** en la pantalla de configuración de 2FA de Miro.

   ![2FA-setup-step-1-Confirmation-of-authenticator-app-download.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653633554_2FA-setup-step-1-Confirmation-of-authenticator-app-download.png)
   *Confirmación de descarga de la aplicación de autenticación*
3. Usando la aplicación de autenticador, ahora tienes dos opciones:


   Escanear el código QR

   1. Abre tu aplicación de autenticador.
   2. Usa la aplicación para escanear el código QR.
   3. Después de escanear, haz clic en **Ya escaneé el código**
      en Miro.

      ![2FA-setup-step-2-Scan-QR-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683263122_2FA-setup-step-2-Scan-QR-code.png)*Escaneando el código QR*

   Ingresar manualmente el código de Miro

   1. Si no puedes escanear el código QR, haz clic en **¿No puedes escanear el código QR?** en Miro.
   2. Miro proporcionará un código de autenticación. **Copia** este código.
   3. Abre tu aplicación de autenticación y pega el código copiado.
   4. Después de agregar el código a la aplicación, haz clic en
      **Agregué el código** en Miro.

      ![2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653636754_2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png)*Copiando el código de Miro para pegarlo en la aplicación de autenticación*
4. La aplicación de autenticación generará un código de verificación de 6 dígitos. Ingresa este código en Miro y haz clic en **Verificar código**.

   ![2FA-setup-step-3-enter-6-digit-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653634706_2FA-setup-step-3-enter-6-digit-code.png)
   *Verificando el código de 6 dígitos*
5. Después de verificar exitosamente tu cuenta con el código de 6 dígitos, Miro proporcionará un código de recuperación. Haz clic en **Copiar** para guardar este código de forma segura. Es crucial tener este código ya que te permite restablecer tu 2FA en caso de que pierdas el acceso a tu aplicación de autenticación.

   Para confirmar que has registrado el código, selecciona **He guardado este código**, luego haz clic en **Continuar** para completar el proceso.

   ![Save-2FA-recovery-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683265554_Save-2FA-recovery-code.png)*Guardando el código de recuperación*

## Iniciar sesión con autenticación de dos factores (2FA)

Una vez que hayas configurado correctamente la autenticación de dos factores (2FA) para tu cuenta, cada vez que intentes iniciar sesión, Miro te solicitará que ingreses un código de seis dígitos generado por tiempo (TOTP).

Este código es generado por tu aplicación de autenticación y proporciona una capa adicional de seguridad para tu cuenta. Simplemente abre tu aplicación de autenticación, busca el código actual e ingrésalo en la página de inicio de sesión para acceder a tu cuenta.

![2fa-user-guide.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/20847806879634_2fa-user-guide.png)
*Iniciando sesión en Miro con 2FA*

Tienes tres intentos antes de que te solicitemos reiniciar el proceso de inicio de sesión.

![Too-many-attempts.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683267346_Too-many-attempts.png)*Demasiados intentos de inicio de sesión con 2FA*

### Confiar en los dispositivos autenticados con dos factores (2FA)

Si tu administrador lo ha configurado, puedes seleccionar la casilla de **Confiar en este dispositivo** al iniciar sesión en tu cuenta con 2FA cuando uses un dispositivo seguro (no uses **Confiar en este dispositivo** si inicias sesión desde una computadora compartida o de acceso público). Cuando haces esto, podrás iniciar sesión sin ingresar tu segundo factor, hasta que pase un período de tiempo especificado. Este período de tiempo es establecido por tu administrador y puede variar entre 7 y 90 días.

![2FA-signin.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/19612606396818_2FA-signin.png)

*La duración de confiar en un dispositivo se muestra junto a la casilla al iniciar sesión con autenticación de dos factores*

Si no ves la opción de "Confiar en este dispositivo", entonces tu administrador no la ha habilitado para tu organización.

Si inicias sesión con un nuevo dispositivo, o después de haber borrado las cookies en tu dispositivo de confianza, se requerirá 2FA nuevamente.

## Cómo restablecer la autenticación de dos factores (2FA)

Si encuentras problemas con tu aplicación autenticadora, pierdes tu dispositivo o necesitas restablecer tu 2FA por cualquier otra razón, sigue estos pasos:

### Tengo un código de recuperación

1. Haz clic en **Restablecer la autenticación de dos factores**.
2. Usa el código de recuperación que guardaste durante tu configuración inicial de 2FA. Se te guiará nuevamente a través del proceso de configuración para reconfigurar tu aplicación de autenticación.

![Reset-two-factor-authentication.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683268114_Reset-two-factor-authentication.png)*La opción para restablecer la autenticación de dos factores*

### No tengo un código de recuperación

Si perdiste tu código de recuperación o no puedes utilizar el flujo de auto-recuperación, deberás solicitar que tu admin restablezca tu 2FA.

Si tu dominio de correo electrónico no forma parte de los dominios verificados de tu organización, tu admin no podrá iniciar un restablecimiento por ti. Deberás solicitar el restablecimiento de 2FA tú mismo; entonces, tu admin podrá aprobarlo.

Los admins solo pueden restablecer la autenticación de dos factores para usuarios cuyos dominios de correo electrónico están verificados en su organización, si el admin inicia el restablecimiento. Si el usuario solicita un restablecimiento, entonces cualquier admin en la organización puede aprobarlo.

Sigue estos pasos:

1. Haz clic en **Pedir a tu admin que restablezca**.
   ![2fa-user-reset.png](https://help.miro.com/hc/article_attachments/24650801878290)
   *Pide a tu admin que restablezca tu 2FA si no tienes un código de recuperación*
2. Si perteneces a más de una organización que usa 2FA, necesitarás seleccionar a cuál admin de la organización quieres hacerle la solicitud.
3. Recibirás un correo electrónico con un código de verificación.
4. Ingresa el código de verificación.
5. Se mostrará una confirmación de que la solicitud fue enviada al admin elegido.
6. Cuando el admin restablezca tu 2FA, necesitarás completar el proceso de configuración de 2FA la próxima vez que inicies sesión.

## Preguntas frecuentes

¿Por qué necesito configurar 2FA?

La autenticación de dos factores mejora la seguridad de tu organización. Todos los usuarios que no utilicen inicio de sesión único deben usar la autenticación de dos factores para iniciar sesión si este requisito es aplicado por el admin de tu empresa.

¿Tengo que usar 2FA cada vez que inicio sesión?

Sí. Después de completar la configuración inicial, debes usar tu aplicación de autenticación para cada inicio de sesión para asegurar que tu cuenta siga siendo segura.

intenté configurar 2FA, pero recibí un error de "Código inválido", aunque mi código es correcto. ¿Qué debo hacer?

Asegúrate de que la zona horaria, la fecha y la hora de tu dispositivo estén configuradas correctamente. Si el problema persiste, intenta configurar 2FA en un dispositivo diferente.

¿Qué hago si accidentalmente confío en un dispositivo compartido?

Si confías accidentalmente en un dispositivo compartido, necesitarás borrar las cookies de Miro en ese dispositivo. Hacer esto es simple:

1. Haz clic en el icono de deslizador en el lado izquierdo de la barra de direcciones de tu navegador.
2. Haz clic en "Cookies y datos del sitio" en el menú.
3. Luego haz clic en "Administrar los datos del sitio en el dispositivo."
4. Haz clic en el ícono de la papelera al lado de cada URL listada allí para borrar las cookies y datos del sitio.

Ten en cuenta que una vez que hayas borrado los datos del sitio desde el dispositivo, tendrás que iniciar sesión nuevamente usando la autenticación de dos factores.

¿Qué sucede si pierdo acceso a un dispositivo de confianza?

Si pierdes acceso a un dispositivo de confianza antes de que el período de confianza haya expirado, puedes usar la opción **Cerrar sesión en todas partes** para eliminar el acceso de todos los dispositivos con sesión iniciada (excepto el dispositivo que estás utilizando actualmente). Esto cerrará tu sesión en todos los demás dispositivos y revocará el 2FA de cualquier dispositivo de confianza. Puedes encontrar el enlace **Cerrar sesión en todas partes** en la configuración de tu perfil de usuario. Luego deberás pasar nuevamente por el proceso de inicio de sesión con 2FA en los dispositivos a los que tengas acceso.
