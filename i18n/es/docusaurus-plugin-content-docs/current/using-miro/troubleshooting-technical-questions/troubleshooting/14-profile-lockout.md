---
title: Bloqueo de perfil
article_id: 360017571374
translation_id: 360017571374
locale: es
sidebar_position: 14
created_at: '2019-02-11T10:08:55Z'
updated_at: '2026-02-24T12:02:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

El bloqueo de perfil es estándar paratodos los usuarios y planes de Miro, y no es posible la personalización. Los usuarios que intenten [autenticarse a través de proveedores de identidad externos](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) no se verán afectados por esta función.

Después de un inicio de sesión erróneo en tu perfil, tienes **10 intentos** para colocar una contraseña correcta en un par de correo electrónico-contraseña. Los primeros 5 intentos son estándar sin complejidad adicional.

Los siguientes intentos añadirán un captcha (solo para las aplicaciones web y de escritorio). Si no logras proporcionar la contraseña correcta **10 veces seguidas** para un par de correo electrónico-contraseña, tu perfil de usuario se bloqueará durante**1 hora**, durante la cual todos los intentos de iniciar sesión en el perfil fallarán incluso si se proporciona la contraseña correcta.

:::tip
Durante la hora de bloqueo, puedes intentar iniciar sesión sin contraseña o con un proveedor social.
:::

Cuando tu perfil de usuario se bloquea, Miro te envía un mensaje de correo electrónico con un código de seis dígitos para desbloquear el perfil. El enlace en el mensaje de correo electrónico te redirige a la página de confirmación, en la que tendrías que proporcionar el código de seis dígitos. Si el código proporcionado es correcto, el perfil se desbloquea y se restablecen todos los intentos. En el mensaje de correo electrónico también se sugiere que cambies la contraseña.

El perfil bloqueado se desbloquea **automáticamente** en 1 hora y todos los intentos fallidos se restablecen.

### Qué hacer si no recibes el código

Si no puedes encontrar el mensaje de correo en tu bandeja de entrada, prueba estos pasos de resolución de problemas:

- Asegúrate de que no haya errores de tipeo en la dirección de correo electrónico que enviaste. Si encuentras un error de tipeo, intenta iniciar sesión con la dirección correcta.
- Abre tus carpetas de **Spam, Promociones, Correo no deseado, Social** y **Actualizaciones** y verifica si el correo de confirmación de Miro está ahí.
- Verifica si tu bandeja de entrada está llena para asegurarte de que no hayas llegado al límite de memoria en tu cuenta de correo electrónico. Si está llena, es posible que tengas que eliminar algunos mensajes existentes para recibir nuevos. Después de eliminar correos, haz clic en **Enviar código nuevamente** para recibir un correo de registro.
- También es posible que un firewall esté impidiendo que el correo electrónico llegue a tu bandeja de entrada. Comunícate con el *administrador de tu sistema* y pídele que incluya nuestros dominios y subdominios como autorizados: [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) y [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/). [Aquí tienes un artículo](../../tools/troubleshooting/02-allowlist-miro-mailers.md) con más información sobre los correos que debes incluir en la lista de admitidos.
- Usuarios de AOL/CompuServe: asegúrense de que los Controles de correo electrónico estén configurados para recibir mensajes de correo electrónico de Internet. Si tienen bloqueado el correo electrónico de Internet, deben cambiar los Controles de correo electrónico; para ello, deben ingresar en **Mail Controls** en AOL o CompuServe. Después de eso, deben regresar a nuestro formulario de registro para reenviar el código de confirmación.
- Por lo habitual, el código debería llegar de inmediato, pero debido a las peculiaridades de tu sistema de correo, podrías tener que esperar hasta 24 horas.
- Si ninguna de las soluciones ayuda, [informa del problema al soporte de Miro](../../tools/troubleshooting/06-contacting-miro-support.md).
