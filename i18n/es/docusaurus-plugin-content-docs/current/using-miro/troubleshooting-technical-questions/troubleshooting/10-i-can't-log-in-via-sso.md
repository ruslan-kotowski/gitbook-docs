---
title: "No puedo iniciar sesi\xF3n v\xEDa SSO"
article_id: 360019271654
translation_id: 360019271654
locale: es
sidebar_position: 10
created_at: '2019-03-07T15:50:03Z'
updated_at: '2025-11-25T16:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Obtén consejos para ti y tus admins de IT para la resolución de problemas relacionados con el inicio de sesión único (SSO).

> **✏️** Obtén más información sobre [la configuración de SSO de Miro](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) y [SCIM de Miro](https://developers.miro.com/docs/scim).

## Errores de SSO de Miro

Si ves alguno de estos mensajes de error de SSO, explora las soluciones que se indican a continuación.  Puede que necesites ayuda de tu departamento de IT o de los admins de empresa.

Tu correo electrónico no está asociado a una cuenta de SSO

Esto sucede cuando la dirección de email que has introducido en Miro no se reconoce como un usuario que debería ser autenticado vía SSO.

Posibles causas:

- **No eres miembro de ninguna subscripción que tenga el SSO establecido como requisito de inicio de sesión**.  Inicia sesión de forma tradicional (email y contraseña) o ponte en contacto con tu admin para recibir una invitación a la subscripción de tu empresa.
- **Se supone que debes iniciar sesión con el SSO, pero hay una confusión con tu dirección de email**.  Tal vez tengas varios emails (o alias) y la invitación al plan con SSO establecido se envió a tu otra dirección. Inicia sesión con otra dirección de correo electrónico.

Tu correo electrónico no está asociado a una cuenta de SSO. Solicita acceso desde tu admin de empresa

Esto suele ocurrir en dos circunstancias:

- **Tu perfil de usuario en el sistema del proveedor de identidad no tiene permiso para iniciar sesión en Miro (no tienes un rol asignado)**.  Si este es el caso, es probable que no encuentres el mosaico de Miro en el panel MyApps de tu proveedor. Ponte en contacto con el admin de tu proveedor para obtener los permisos necesarios. /span>
- **Cambiaste tu correo electrónico recientemente** y el cambio no se ha aplicado correctamente en todos los sistemas, creando así conflictos.  Ponte en contacto con tu admin para aclarar la situación y, si es necesario, ellos se pondrán en contacto con nosotros para aprobar los cambios oportunos.

Si no puedes iniciar sesión en Miro usando el SSO, puedes solicitar acceso a los admins de empresa haciendo clic en el botón correspondiente en la[página de inicio de sesión SSO de Miro](https://miro.com/sso/login/).

![sso-nuevo-acceso.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/20463017477778_sso-new-sign-in.png)*La opción de solicitar acceso a los admins de empresa*

Debes ingresar el código de confirmación enviado a tu dirección de email.  Una vez que ingreses el código, se enviará una notificación a los admins de la subscripción de tu empresa para que sepan que necesitas asistencia.

Algo salió mal" No se ha podido validar la firma de la respuesta

Esto significa que hay algún problema con tu configuración de SSO de Miro o con tu proveedor de identidad. Es probable que ninguno de tus compañeros pueda iniciar sesión. Ponte en contacto con tu departamento de IT o con el admin del proveedor de identidad para que puedan verificar los siguientes puntos:

- La respuesta SAML debe contener la *aserción* firmada.  Este es un requisito de Miro.
- Tu proveedor de identidad puede estar tratando las respuestas firmadas de una manera específica.  Por ejemplo, Google SSO *desmarca*/span> la aserción cuando se firma la *respuesta*. Si ese es el caso, desmarca la respuesta.
- La respuesta SAML contiene la aserción firmada requerida, pero el valor del certificado X.509 que debería validarla no está presente (también puede ocurrir si tu VPN/firewall [bloquea partes de la transferencia de datos](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)).  Asegúrate de que el valor del certificado X.509 se pase en el tráfico SAML a Miro.
- La respuesta SAML contiene un *valor de certificado X.509 diferente al añadido en la* [configuración de Miro](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), por lo que hay una falta de concordancia y la validación falla.  Comprueba que los valores de certificado del proveedor de identidad (IDP) y de Miro coincidan.

Algo salió mal" No se proporcionó usuario en la respuesta SAML.

Esto significa que hay un problema de configuración en tu proveedor de identidad, ya sea en la configuración general o en tu perfil de usuario específico.  Ponte en contacto con tu departamento de IT o con el admin del proveedor de identidad para que puedan verificar los siguientes puntos:

- El formato del nombre de usuario (ID de nombre, ID único de usuario) de tu configuración de SSO no está especificado o está establecido en un atributo que no es un correo electrónico, por lo que el valor de usuario enviado a Miro no se reconoce.  Especifica el nombre de usuario como DirecciónDeEmail /span>**en el proveedor de identidad (o como cualquier otro atributo que esté en formato de email).**
- La respuesta SAML no contiene el valor de email del usuario, por lo que no puede reconocerlo (esto también puede ocurrir si tu VPN o firewall [bloquea partes de la transferencia de datos](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)).  Asegúrate de que el email se pase en el tráfico SAML a Miro.
- La respuesta SAML está cifrada.  Por favor, no uses el cifrado, ya que Miro no cuenta con esta característica.

Algo salió mal" La respuesta SAML no es correcta

Esto suele ocurrir cuando hay problemas con tu perfil en el proveedor de identidad.
Posibles causas:/span>

- **Tu perfil de usuario en el sistema del proveedor de identidad está configurado de forma incorrecta**.  Por ejemplo, no se te da permiso para iniciar sesión en Miro (no tienes una función asignada). Si este es el caso, es probable que no encuentres el mosaico de Miro en el panel MyApps de tu proveedor. Ponte en contacto con el admin de tu proveedor para obtener los permisos necesarios.
- **Tu perfil de usuario en el sistema del proveedor de identidad está configurado correctamente, pero tiene restricciones**.  Por ejemplo, hay restricciones de IP, por lo que solo se te permite iniciar sesión desde ciertos lugares. Comunícate con el admin de tu proveedor de identidad y pregúntale sobre tus permisos.

Para autorizar con SSO, utiliza el enlace URL proporcionado por tu empresa

Esto significa que no debes acceder a Miro desde esta página o que la configuración de SSO de tu plan Enterprise de Miro está incompleta.  En este caso, es posible que puedas iniciar sesión desde tu panel de MyApps.
Posibles causas:/span>

- **Tu IDP está configurado solo para** [el inicio de sesión iniciado por IdP](https://blogs.oracle.com/dcarru/sp-vs-idp-initiated-sso) **y no deberías poder iniciar sesión desde la página de inicio de sesión de Miro.**  Inicia sesión a través del enlace proporcionado desde tu panel MyApps o comunícate con tu admin de empresa para obtener instrucciones.
- **El SSO está habilitado en tu plan Enterprise de Miro, pero la configuración está incompleta**.  Ponte en contacto con tu departamento de TI o con el admin del proveedor de identidad para que terminen la configuración de acuerdo con estas instrucciones./span>

## Errores Entra o ADFS

La configuración de inicio de sesión único no está disponible para esta aplicación en la experiencia de aplicaciones Enterprise.

El texto completo del mensaje: La configuración de inicio de sesión único no está disponible para esta aplicación en la experiencia de aplicaciones Enterprise Miro (antes RealtimeBoard) es una aplicación multi-arrendatario y la aplicación es propiedad de otro arrendatario.
*Para cambiar propiedades como la URL de respuesta y los identificadores, ponte en contacto con el propietario de la aplicación.*Ponte en contacto con tu departamento informático y pídeles que comprueben la configuración del SSO. Lo más probable es que ya haya una app Miro configurada en tu Entra ID en la que se utiliza nuestro identificador (`https://miro.com/)` y, por tanto, se toma. Entra es más o menos único en el sentido de que este proveedor de identidad exige que el identificador (Entity ID) sea único.
Para resolver posiblemente la situación, te aconsejamos que compruebes las aplicaciones de empresa de tu instancia de Entra y utilices la que ya tengas configurada para tu configuración de Miro.
Si estás seguro de que no hay otras apps de Miro en las apps de tu empresa, prueba a copiar una nueva app de Miro de la galería Entra.

Se ha producido un error. Ponte en contacto con tu admin para obtener más información

Comparte este post de la comunidad con tu departamento informático: Se ha producido un error. Ponte en contacto con tu admin para obtener más información

No se ha otorgado el acceso: error AADSTS50105

![mceclip3.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044185746_mceclip3.png)
Comparte este artículo de la comunidad con tu departamento informático: [Error "Rol no asignado".](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50105-user-not-assigned-role)

Aplicación mal configurada: error AADSTS650056

![mceclip2.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044184722_mceclip2.png)
Revisamos la documentación de Microsoft en busca del error AADSTS650056 (así como algunas sugerencias de la comunidad) y parece que el error puede ser causado por los cambios que agregaste a los permisos de la aplicación. Es posible que tu admins de Entra tenga que dar su consentimiento a la app Miro para permitir que los usuarios finales se autentiquen en Miro. Este tutorial de Microsoft debería ser útil en este caso.

Lee [el artículo support.microsoft.com sobre otros posibles errores de SSO](https://support.office.com/article/how-to-troubleshoot-issues-that-you-encounter-when-you-sign-in-to-office-apps-for-mac-ipad-iphone-or-ipod-touch-when-using-active-directory-federation-services-e44357b4-c9c4-4580-a946-ef5dabdb98cd?ui=en-US&rs=en-US&ad=US).

## Errores de Google SAML

Consulta [esta sección de la documentación de Google](https://support.google.com/a/answer/6301076?hl=en), que enumera errores posibles y da instrucciones sobre cómo resolver la situación.

## Problemas para iniciar sesión en la aplicación de Miro vía SSO en la aplicación de escritorio, tableta o móvil

Si no puedes iniciar sesión en la aplicación de Miro vía SSO en un dispositivo de escritorio, una tableta o un dispositivo móvil, pero puedes iniciar sesión en la [versión del navegador](https://miro.com/app/), realiza lo siguiente:

1. Elimina la aplicación desde el dispositivo y vuelve a instalarla.  Para la aplicación de escritorio, asegúrate de eliminar todas las carpetas de la aplicación siguiendo estas instrucciones/span>. La causa más común de este problema es la caché con problemas, por lo que debería ser de ayuda eliminar todo y volver a instalar desde cero.
2. Cambia el navegador predeterminado de tu dispositivo a otro para ver si, con un navegador diferente, puedes completar el proceso.  Asegúrate de que tu navegador preferido permita cookies de terceros/span>.
3. Comprueba si tu proveedor de identidad *no* administra el parámetro **RelayState**. Es un token único que Miro genera y usa para reconocer que se debería devolver al usuario a la aplicación, en lugar de permanecer en la página del navegador. Revisa si tienes campos en tu configuración de IdP que administren RelayState que estén vacíos (el campo podría tener un nombre, por ejemplo, en Okta sería **Default RelayState**, en Google SSO *Start URL*).
4. Si el problema persiste, es posible que este dispositivo específico no pueda acceder al entorno SSO de la empresa.  Consulta con tu departamento de TI para verificar si existe alguna restricción con respecto a dispositivos específicos para el uso de SSO. Por ejemplo, con soluciones MDM, pueden surgir problemas si Miro no está en la lista de aplicaciones permitidas/span>[.](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)
5. Para la aplicación de escritorio de Miro en específico: comprueba que el esquema de nuestra aplicación funciona correctamente para ti y que no está dañado.  Para hacer lo anterior, ingresa **miroapp://** en la línea de dirección de tu navegador preferido y haz clic para abrirlo *como sitio web* (no presiones simplemente Enter; esa acción solo iniciará una búsqueda).
   ![mceclip0.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695734034_mceclip0.png)
   En este momento, se supone que debes obtener un ​ventana emergente que te instruye para abrir la app Miro. Si no sucede, el esquema puede estar roto. Para comprobar si el esquema está instalado correctamente, sigue las instrucciones para Windows o Mac (esto no corresponde para la versión de la aplicación de Miro de MS Store).

   Para Windows Para Mac

   1. Ve a la [aplicación del Editor del registro.](https://support.microsoft.com/windows/how-to-open-registry-editor-in-windows-10-deab38e6-91d6-e0aa-4b7c-8878d9e07b11)
   2. Presiona Ctrl + F y busca **miroapp.**  Tu registro debería verse así:/strong>
      mapa_editor_registro.png

   1. Ejecuta el siguiente comando en la aplicación terminal:

      **sudo /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/LaunchServices.framework/Versions/A/Support/lsregister -dump URLSchemeBinding | grep miroapp**

      El resultado debería verse como esto:

      ![](/attachments/token/I53o1MUemZ9TqkRlz9dQ7ndsr/?name=image.png)

Si tu situación es diferente (el archivo del esquema no se muestra en el registro o se muestra en una ruta diferente, por ejemplo), prueba instalar nuevamente la aplicación [desde nuestro sitio web](https://miro.com/apps/).

Si eso no ayuda, comunícate con tu equipo de TI y pídele que verifique la situación, especialmente los siguientes puntos:

- Si los protocolos URI personalizados están permitidos.  Si están bloqueados, es posible que no se pueda instalar nuestro esquema durante el proceso de instalación de la aplicación.
- Si el registro está sujeto a otras restricciones o políticas que puedan evitar o modificar la instalación estándar.

## Mi email cambió y no puedo iniciar sesión en mi perfil vía SSO

Ten en cuenta que, si tu organización utiliza SSO, el cambio de dirección de email debe hacerse tanto desde Miro como desde el proveedor de identidad antes de que un usuario final pueda usar sus nuevas credenciales para iniciar sesión en Miro.  Si el cambio no se ha hecho antes de tu siguiente inicio de sesión, tu email se reconoce como un nuevo usuario y puedes tener problemas para iniciar sesión en Miro.

Ponte en contacto con tu admin para aclarar la situación.  Quizás tu admin y tú tengáis que poneros en contacto con el equipo de Soporte de Miro/span> [para que podamos borrar tu nuevo perfil vacío y cambiar la dirección de correo electrónico en el perfil existente.](../../tools/troubleshooting/06-contacting-miro-support.md)  Proporciona la siguiente información:

- Tu nueva dirección de correo electrónico y tu antigua dirección de correo electrónico.
- Copia al admin de Miro de tu empresa y pídele que envíe una confirmación de que podemos continuar con el cambio (requerido por motivos de seguridad).

:::note
Si no pudiste encontrar una solución arriba, [comunícate con el equipo de Soporte de Miro](https://miro.com/contact/recover/).
:::
