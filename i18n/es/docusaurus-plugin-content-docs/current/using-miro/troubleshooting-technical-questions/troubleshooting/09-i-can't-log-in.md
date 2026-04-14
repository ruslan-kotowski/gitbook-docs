---
title: "No puedo iniciar sesi\xF3n"
article_id: 360020993079
translation_id: 360020993079
locale: es
sidebar_position: 9
created_at: '2021-04-09T06:31:47Z'
updated_at: '2025-11-25T16:04:24Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Sigue esta guía si tienes problemas para iniciar sesión en tu perfil de Miro.

## Problemas con el correo electrónico o la contraseña

Mi correo electrónico/contraseña no funciona

Aquí tienes dos soluciones que puedes explorar:

1. Verifica que el correo electrónico y la contraseña que usas para iniciar sesión no contengan errores de tipeo.
2. Si las credenciales que ingresas son correctas, [restablece la contraseña](../../managing-your-profile/05-how-to-change-your-password.md).
3. Si tu correo electrónico o contraseña incluye los símbolos **& " < o >**, [comunícate con nuestro equipo de soporte.](https://help.miro.com/hc/requests/new?)

:::warning
Ten en cuenta que tu **perfil se bloquea** después de 10 intentos de ingresar tu correo electrónico y tu contraseña. Es posible que debas [desbloquear el perfil](../../tools/troubleshooting/14-profile-lockout.md) primero y luego, restablecer tu contraseña.
:::

No puedo restablecer mi contraseña

Si no recibes un correo electrónico para restablecer la contraseña, puede haber tres razones:

1. **El correo electrónico es incorrecto**
Asegúrate de que no haya errores de tipeo en el correo electrónico que enviaste. Si encuentras un error, vuelve a intentar enviar la solicitud de restablecimiento.

2. **El correo electrónico aún no está registrado en Miro**
En este caso, el enlace de restablecimiento de la contraseña no se enviará a tu dirección de correo electrónico. Registra un nuevo perfil en la [página de registro](https://miro.com/signup/). Si tu correo electrónico está registrado, verás el mensaje correspondiente:
![mceclip0.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695734034_mceclip0.png)

3. **Hay problemas en la entrega del correo electrónico**

- Abre las carpetas de **Spam, Promociones, Correo no deseado, Redes sociales** y **Actualizaciones**, y comprueba si el mensaje de solicitud de restablecimiento se encuentra en alguna de ellas.
- También puede ocurrir que un firewall impida que el correo electrónico llegue a tu bandeja de entrada.

  Comunícate con tu *admin de sistema* y pídele que incluya nuestros dominios y subdominios en la lista de admitidos: [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) y [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/). Tú también deberás agregar el IPS de nuestro sistema de envío de correos electrónicos a la lista de admitidos.

  Esta es la lista de IP dedicadas: 198.2.178.132, 198.2.178.117, 198.2.128.203, 198.2.178.252, 198.2.178.205. [Consulta este artículo](../../tools/troubleshooting/02-allowlist-miro-mailers.md) con más información sobre los remitentes que debes incluir en la lista de admitidos.

Restablecí mi contraseña, pero aún no puedo iniciar sesión

Si aún no puedes acceder a tu perfil:

1. Asegúrate de introducir la nueva contraseña.
2. Inicia sesión en el modo privado (incógnito) del navegador o prueba con otro navegador.

Inicio sesión con un correo electrónico, pero se me redirecciona y aparezco con otro correo electrónico

Este problema puede ocurrir si usas un método de autenticación alternativo para iniciar sesión (Google, Slack, Office 365, Apple ID, Facebook).

![new-sing-in-third-party.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725436050_new-sing-in-third-party.png)
*Opciones de inicio de sesión alternativas en la página de inicio de sesión*

Es posible que hayas vinculado accidentalmente tu dirección de correo electrónico de Google/Office 365/etc. a tu perfil de Miro registrado con un correo electrónico diferente. Si eso sucede, prueba lo siguiente:

1. Elimina la asociación incorrecta de correo electrónico. Para ello, ve a **Configuración del perfil** > **Integraciones** y haz clic en **Cerrar sesión** junto a Google/Office 365/etc.
   ![remove_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725424658_remove%20connection.jpg)
   *Eliminar la asociación con el inicio de sesión de Google*
2. Cierra sesión e inicia sesión con tu correo electrónico de nuevo.

:::note
Configura una conexión con el correo electrónico de Google/Office 365/Slack que coincida con el de tu perfil de Miro para evitar el problema.
:::

## El inicio de sesión único no funciona

Consulta el artículo [Posibles problemas con el inicio de sesión único (SSO)](../../tools/troubleshooting/10-i-can't-log-in-via-sso.md).

## Carga interminable al iniciar sesión

Para los usuarios que tienen problemas para cargar el contenido después de ingresar sus credenciales de Miro, recomendamos lo siguiente:

1. Iniciar sesión en un **navegador diferente**.
2. Inicia sesión usando el **modo privado (incógnito) del navegador.** Si el problema no se reproduce en el modo incógnito o en otro navegador, limpia la caché de tu navegador.

   Cómo limpiar el caché de Chrome

   1. Ve a `https://miro.com/` y abre las **herramientas para desarrolladores** de Chrome (**Command + Option + J** *en Mac* o **Ctrl + Shift + J** *en Windows*).
   2. Selecciona la pestaña **Aplicación > Almacenamiento**. Verás el botón azul **Borrar datos del sitio.**​  Haz clic en el botón y se deberían eliminar los datos de Miro guardados en el navegador Chrome para que puedas iniciar una nueva sesión de trabajo.
   ![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)
   *Opción para borrar los datos del sitio en Chrome*
3. Si usas una **VPN**, desactívala/actívala.
4. Consulta con el departamento de TI si tu empresa usa firewalls o un proxy que pudiera bloquear a Miro. Sigue [estos lineamientos](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md) para **incluir Miro en la lista de admitidos** o proporcionar un bypass.
5. Comprueba tu conexión a Internet. Si el ancho de banda de tu red no alcanza el mínimo de 8 Mb/s, **cambia a otra red, preferiblemente** **más rápida**.
6. Intenta conectarte a un **punto de acceso móvil**, si está disponible. A continuación, vuelve a conectarte a tu red original.
7. Si eso no ayuda, [envía una solicitud](https://miro.com/contact/recover/) y [remite los registros de la consola del navegador a soporte](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

## Problemas de inicio de sesión en la aplicación de escritorio de Miro

1. Si no puedes acceder a Miro en la aplicación de escritorio, inicia sesión con el navegador. Si aun así no puedes iniciar sesión, sigue los pasos anteriores. Si puedes acceder a Miro en el navegador, sigue los pasos que se indican a continuación.
2. Restablece los datos de la aplicación.

Cómo restablecer los datos de la aplicación en Windows

Presiona **Alt > Ayuda** y elige restablecer los datos de la aplicación, como se muestra en la siguiente captura de pantalla:

​​![reset_app_data_on_Windows.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725434514_reset%20app%20data%20on%20Windows.jpg)
*Restablecer los datos de la aplicación en la aplicación de escritorio de Windows*

Si no puedes encontrar el menú, probablemente uses la aplicación descargada desde MS Store. En este caso, para restablecer los datos de la aplicación, abre **Configuración de Windows** > **Aplicaciones** > **Aplicaciones y funciones** > busca **Miro** en la lista > **Opciones avanzadas**> **Restablecer**.

Si esto no ayuda a proceder de inmediato para eliminar todos los archivos de la aplicación de **C:\Users\username\AppData\Roaming\RealtimeBoard** y **C:\Users\username\AppData\Local\RealtimeBoard**

> **✏️** Si la carpeta Appdata está oculta, **consulta aquí cómo**  puedes visualizarla.

Cómo restablecer los datos de la aplicación en Mac

Haz clic en **Miro** en el menú superior y elige Restablecer los datos de la aplicación como se muestra en la captura de pantalla a continuación:

![reset_app_data_on_Mac.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695741458_reset%20app%20data%20on%20Mac.jpg)
*Restablecer los datos de la aplicación en Mac*

A continuación, vuelve a intentar iniciar sesión en la aplicación y comprueba si se resolvió el problema.

Si el restablecimiento de los datos no ayuda de inmediato, abre una ventana de Finder > presiona **Command + Shift + G** > pega **~/Library/Application Support/RealtimeBoard**y elimina todos los archivos de la aplicación.

3. Si el problema persiste, asegúrate de estar usando la versión más reciente de la aplicación descargada [de nuestro sitio web.](https://miro.com/apps/)

## Inicio de sesión con Google/Office 365/Slack/etc.

No puedo iniciar sesión mediante Google/Office/Slack/etc.

1. Inicia sesión en Miro con tus credenciales convencionales (correo electrónico y contraseña). Si no recuerdas o no tienes la contraseña, [restablécela](../../managing-your-profile/05-how-to-change-your-password.md).
2. Ve a **Configuración del perfil** > **Integraciones**, haz clic en **Cerrar sesión** junto a Google/Office 365/etc. y vuelve a configurar la conexión.
   ![remove_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725424658_remove%20connection.jpg)
   *Eliminar la asociación con el inicio de sesión de Google*

No puedo iniciar sesión mediante Google, Office, Slack, etc. en la aplicación de escritorio

Explora estos pasos de resolución de problemas.

Solía iniciar sesión en Miro a través de Google/Office 365/etc., pero mi servicio de correo electrónico ha cambiado. ¿Cómo puedo iniciar sesión ahora?

Inicia sesión en Miro con las credenciales de tu nuevo servicio (correo electrónico y contraseña). Si no recuerdas o no tienes la contraseña, [restablécela](../../managing-your-profile/05-how-to-change-your-password.md).

## Problemas de inicio de sesión en tabletas/móviles

1. Comprueba si puedes iniciar sesión en la versión del navegador. Si no puedes, recomendamos estos pasos de solución de problemas.
2. Si puedes iniciar sesión desde el navegador, es posible que los datos de autenticación del dispositivo estén dañados. Ve a **Configuración de la aplicación > Almacenamiento > Borrar almacenamiento** o reinstala la aplicación de Miro en tu dispositivo.

## Consejos de resolución de problemas

Si no pudiste encontrar una solución en la información anterior, inicia sesión en Miro con **otro navegador** o en **modo incógnito**. Si todo está bien en el modo incógnito de tu navegador, limpia el caché y las cookies del navegador e inicia sesión en Miro en el modo estándar.

Cómo limpiar el caché de Chrome

1. Ve a `https://miro.com/` y abre las **herramientas para desarrolladores** de Chrome (**Command + Option + J** *en Mac* o **Ctrl + Shift + J** *en Windows*).
2. Selecciona la pestaña **Aplicación > Almacenamiento**. Verás el botón azul **Borrar datos del sitio.**​  Haz clic en el botón y se deberían eliminar los datos de Miro guardados en el navegador Chrome para que puedas iniciar una nueva sesión de trabajo.

![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)
*Opción para borrar los datos del sitio en Chrome*

Si nada de esto ayuda, [comunícate con el soporte de Miro](https://miro.com/contact/recover/). Describe el problema en detalle.

:::note
Si tienes inconvenientes para registrarte con Miro, [consulta Problemas con el código de confirmación](../../tools/troubleshooting/12-issues-with-confirmation-code-or-password-reset-emails.md).
:::
