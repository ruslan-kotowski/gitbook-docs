---
title: Autenticación de dos factores (2FA) – guía del usuario
article_id: 27601422748434
translation_id: 27601422748434
locale: es
sidebar_position: 2
created_at: '2025-06-24T07:36:23Z'
updated_at: '2025-11-06T13:29:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: 2fa
availability:
  notes: 'Relevante para: Starter, Business, Education, Enterprise'
---

## ¿Qué es la autenticación de dos factores (2FA)?

La autenticación de dos factores (2FA) añade más seguridad a tus cuentas online. Cuando el admin de empresa activa la autenticación de dos factores (2FA), cada inicio de sesión en Miro usando tu correo electrónico y contraseña será seguido por una capa adicional de seguridad. Este paso adicional garantiza una protección mejorada para tu cuenta, requiriendo verificación más allá de tus credenciales de inicio de sesión habituales.

:::tip
Aprende cómo habilitar la autenticación de dos factores (2FA) para tu organización en [planes Enterprise](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md), y [todos los demás planes](01-two-factor-authentication-2fa.md).
:::

## Cómo configurar la autenticación de dos factores (2FA)

**Nuevos usuarios:** Durante tu proceso de [registro](https://miro.com/signup/) con tu dirección de correo electrónico de la empresa, se te pedirá que habilites 2FA.
 **Usuarios existentes:** En tu próximo [inicio de sesión](https://miro.com/login/), si tu organización requiere 2FA y no estás usando inicio de sesión único (SSO), se te pedirá que configures 2FA.

1. Descarga una aplicación de autenticación en tu dispositivo móvil. Las aplicaciones de autenticación, como Google Authenticator, Microsoft Authenticator y Authy, generan un código de un solo uso basado en tiempo (TOTP) para inicios de sesión seguros en Miro. Para saber qué aplicación de autenticación elegir, consulta con tu admin de empresa o administrador de TI.

2. Haz clic en **Tengo una aplicación de autenticación** en la pantalla de configuración de 2FA de Miro.

   ![2FA-setup-step-1-Confirmation-of-authenticator-app-download.png](../../../../../../docs/administration/security-compliance/images/27601397095698_2FA-setup-step-1-Confirmation-of-authenticator-app-download.png)
   *Confirmación de la descarga de la aplicación de autenticación*
3. Con la aplicación de autenticador, ahora tienes dos opciones:


   Escanea el código QR

   1. Abre tu aplicación de autenticador.
   2. Usa la aplicación para escanear el código QR.
   3. Después de escanear, haz clic en **Escaneé el código**
      en Miro.

      ![2FA-setup-step-2-Scan-QR-code.png](../../../../../../docs/administration/security-compliance/images/27601422721298_2FA-setup-step-2-Scan-QR-code.png)*Escaneando el código QR*

   Ingresa manualmente el código de Miro

   1. Si no puedes escanear el código QR, haz clic en **¿No puedes escanear el código QR?** en Miro.
   2. Miro te proporcionará un código de autenticación. **Copia** este código.
   3. Abre tu aplicación de autenticación y pega el código copiado.
   4. Después de agregar el código a la aplicación, haz clic en **Agregué el código** en Miro.

      ![2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png](../../../../../../docs/administration/security-compliance/images/27601397098898_2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png)*Copiando el código de Miro para pegarlo en la aplicación de autenticación*
4. La aplicación de autenticación generará un código de verificación de 6 dígitos. Ingresa este código en Miro y haz clic en **Verificar código**.

   ![2FA-setup-step-3-enter-6-digit-code.png](../../../../../../docs/administration/security-compliance/images/27601422725906_2FA-setup-step-3-enter-6-digit-code.png)
   *Verificando el código de 6 dígitos*
5. Después de verificar con éxito tu cuenta con el código de 6 dígitos, Miro proporcionará un código de recuperación. Haz clic en **Copiar** para guardar este código de forma segura. Es crucial tener este código ya que te permite restablecer tu 2FA en caso de que pierdas el acceso a tu aplicación de autenticación.

   Para confirmar que has registrado el código, selecciona **He anotado este código**, luego haz clic en **Continuar** para completar el proceso.

   ![Save-2FA-recovery-code.png](../../../../../../docs/administration/security-compliance/images/27601422727314_Save-2FA-recovery-code.png)*Guardando el código de recuperación*

## Iniciar sesión con autenticación de dos factores (2FA)

Una vez que hayas configurado exitosamente la autenticación de dos factores (2FA) para tu cuenta, cada vez que intentes iniciar sesión, Miro te pedirá que ingreses un código de seis dígitos de un solo uso basado en el tiempo (TOTP).

Este código lo genera tu aplicación autenticadora y proporciona una capa extra de seguridad para tu cuenta. Simplemente abre tu aplicación autenticadora, recupera el código actual y escríbelo en la página de inicio de sesión para acceder a tu cuenta.

![2fa-user-guide.png](../../../../../../docs/administration/security-compliance/images/27601397105298_2fa-user-guide.png)
*Iniciar sesión en Miro con 2FA*

Tienes tres intentos antes de que se te solicite reiniciar el proceso de inicio de sesión.

![Too-many-attempts.png](../../../../../../docs/administration/security-compliance/images/27601397107474_Too-many-attempts.png)*Demasiados intentos de inicio de sesión con 2FA*

### Confiar en dispositivos con autenticación de dos factores (2FA)

Si tu administrador lo ha configurado, puedes marcar la casilla para **Confiar en este dispositivo** cuando inicies sesión en tu cuenta con 2FA al usar un dispositivo seguro (no uses **Confiar en este dispositivo** si inicias sesión desde un equipo compartido o de acceso público). Al hacer esto, podrás iniciar sesión sin ingresar tu segundo factor, hasta que pase un período de tiempo especificado. Este período de tiempo es establecido por tu administrador y puede variar entre 7 y 90 días.

![2FA-signin.png](../../../../../../docs/administration/security-compliance/images/27601397108882_2FA-signin.png)

*La duración de la confianza en un dispositivo se muestra junto al recuadro cuando inicias sesión con la autenticación de dos factores*

Si no ves la opción para "Confiar en este dispositivo", entonces tu administrador no la ha habilitado para tu organización.

Si inicias sesión con un nuevo dispositivo—o después de haber borrado las cookies de tu dispositivo confiable—se requerirá 2FA nuevamente.

## Cómo restablecer la autenticación de dos factores (2FA)

Si encuentras incidencias con tu aplicación de autenticación, pierdes tu dispositivo o necesitas restablecer tu 2FA por cualquier otra razón, sigue estos pasos:

### Tengo un código de recuperación

1. Haz clic en **Restablecer la autenticación de dos factores**.
2. Usa el código de recuperación que guardaste durante tu configuración inicial de 2FA. Serás guiado nuevamente a través del proceso de configuración para reconfigurar tu aplicación de autenticación.

![Reset-two-factor-authentication.png](../../../../../../docs/administration/security-compliance/images/27601422733714_Reset-two-factor-authentication.png)*La opción para restablecer la autenticación de dos factores*

### No tengo un código de recuperación

Si has perdido tu código de recuperación o no puedes usar el flujo de recuperación automática, necesitarás solicitar que tu admin restablezca tu 2FA.

Los admins pueden restablecer la autenticación de dos factores solo para los usuarios cuyos dominios de correo están verificados en su organización, si el admin inicia el restablecimiento. Si el usuario solicita un restablecimiento, cualquier admin en la organización puede aprobarlo.

1. Haz clic en **Pedir a tu admin que restablezca**.
   ![2fa-user-reset.png](../../../../../../docs/administration/security-compliance/images/27601397113106_2fa-user-reset.png)
   *Pide a tu admin que restablezca tu 2FA si no tienes un código de recuperación*
2. Si perteneces a más de una organización que usa 2FA, tendrás que elegir a cuál organización deseas hacer la solicitud al admin.
3. Recibirás un correo electrónico con un código de verificación.
4. Ingresa el código de verificación.
5. Se mostrará una confirmación de que la solicitud fue enviada al admin que elegiste.
6. Cuando el admin restablezca tu 2FA, deberás seguir el proceso de configuración de 2FA la próxima vez que inicies sesión.

## Preguntas frecuentes

¿Por qué necesito configurar 2FA?

La autenticación de dos factores mejora la seguridad de tu organización.
Todos los usuarios que no utilizan inicio de sesión único (SSO) deben usar autenticación de dos factores para iniciar sesión si este requisito es aplicado por
el admin de empresa.

¿Tengo que usar 2FA cada vez que inicio sesión?

Sí. Después de completar la configuración inicial, debes usar tu aplicación de autenticación para cada inicio de sesión para garantizar que tu cuenta permanezca segura.

Intenté configurar 2FA pero recibí un error de "Código inválido", aunque mi código es correcto. ¿Qué debo hacer?

Asegúrate de que la zona horaria, la fecha y la hora de tu dispositivo estén configuradas correctamente. Si el problema persiste, intenta configurar 2FA en un dispositivo diferente.

¿Qué pasa si accidentalmente confío en un dispositivo compartido?

Si accidentalmente confías en un dispositivo compartido, tendrás que borrar
las cookies de Miro en ese dispositivo. Hacer esto es sencillo:

1. Haz clic en el icono de la deslizante en el lado izquierdo de la
   barra de direcciones de tu navegador.
2. Haz clic en "Cookies y datos del sitio" en el menú.
3. Luego haz clic en "Gestionar los datos del sitio en el dispositivo".
4. Haz clic en el icono de la papelera junto a cada URL listada allí
   para borrar las cookies y los datos del sitio.

Ten en cuenta que una vez que hayas borrado datos del sitio del dispositivo, tendrás
que iniciar sesión nuevamente usando la autenticación de dos factores.

¿Qué sucede si pierdo acceso a un dispositivo de confianza?

Si pierdes acceso a un dispositivo de confianza antes de que expire el período de confianza, puedes usar la opción **Cerrar sesión en todas partes** para eliminar el acceso de todos los dispositivos en los que hayas iniciado sesión (excepto de aquel que estés usando actualmente). Esto te cerrará la sesión en todos los demás dispositivos y revocará la 2FA de cualquier dispositivo de confianza. Puedes encontrar el enlace **Cerrar sesión en todas partes** en la configuración de tu perfil. Luego tendrás que realizar nuevamente el proceso de inicio de sesión con 2FA en los dispositivos a los que tengas acceso.
