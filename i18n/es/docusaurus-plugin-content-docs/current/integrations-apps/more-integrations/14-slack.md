---
title: Slack
article_id: 360017572494
translation_id: 360017572494
locale: es
sidebar_position: 15
created_at: '2019-02-11T10:13:25Z'
updated_at: '2025-02-26T12:10:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: slack-ms-teams
---

Recibe notificaciones de Slack de nuevos comentarios y menciones en tus tableros y otros cambios relacionados con tu perfil, comparte con facilidad tus tableros de Miro desde Slack y abre automáticamente los enlaces de los tableros. Lee el artículo para aprender a conectar tu Slack a Miro y obtén acceso a todas las atractivas características.

:::note
A algunos usuarios de Slack se les sugiere que se registren fácilmente en Miro a través de Slack cuando hacen clic en un enlace a un tablero de Miro publicado en un canal de Slack.  Por el momento, la característica está en versión beta y es administrada por Slack. No requiere que nuestra aplicación esté instalada en el espacio de trabajo de Slack.
Los administradores de espacios de trabajo tienen la opción de desactivar por completo la función Sign in with Slack (Iniciar sesión con Slack) en la configuración del espacio de trabajo de Slack (App Management Settings [Configuración de administración de aplicaciones] > Sign in with Slack Settings [Configuración para iniciar sesión con Slack]). /span> El Organigrama de Enterprise y sus espacios de trabajo no se incluyen en el lanzamiento en la versión beta.
:::

:::note
Para obtener asistencia para la aplicación de Slack, envía un email a [slack_integration_support@miro.com](mailto:slack_integration_support@miro.com) o visita [Cómo contactar al soporte de Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).
:::

## Activar la aplicación

El usuario es el encargado de configurar la integración de la aplicación Slack para su propio perfil. Para habilitar la integración, abre [Profile settings (ajustes de perfil)](../../using-miro/managing-your-profile/01-profile-settings.md) de Miro.

ir_a_configuración_de_perfil.jpg
[Cómo llegar a la configuración de perfil desde la pizarra de Miro](https://miro.com/app/dashboard/)

Pasa a la pestaña **Integrations** (Integraciones), busca **Miro feed (Slack App) [Feed de Miro (Aplicación de Slack)]** y haz clic en **Connect** (Conectar):

conectar_Slack.jpg
Conectar la aplicación Slack

Otra opción es habilitarla directamente en la [pestaña Notifications (Notificaciones](https://miro.com/app/account/profile/notifications/)):

conectar_Slack_desde_notificaciones.jpg
Activar la aplicación de Slack en la página de notificaciones

Se te redireccionará a autorizar en Slack. Ingresa tus credenciales e inicia sesión en Slack.

autorizar_Slack.jpg
Permitir el acceso de Miro al espacio de trabajo

## Configuración de notificaciones

Personaliza el feed que recibirás eligiendo los eventos sobre los cuales quisieras recibir notificaciones.

Puedes hacer un seguimiento de los siguientes eventos:

- registro de invitados;
- alguien solicita acceso a un equipo o tablero;
- te invitaron a un proyecto;
- se compartió un tablero contigo;
- hay un nuevo comentario en tu tablero o una respuesta a tu comentario en un tablero;
- alguien te @mencionó en un comentario o una respuesta.

Abre la [página de Notificaciones](https://miro.com/app/account/profile/notifications/) y configura tus preferencias:

notification_settings.jpg
Configuración de notificaciones

Ten en cuenta que, en algunos casos, la notificación se te enviará *solo si quien notifica decide* enviarla.

## Reacción a notificaciones directamente en Slack

Cuando alguien solicita acceso a tu tablero, puedes otorgar derecho en Slack. Elige la opción y haz clic en el botón:

reaccionar_en_Slack.jpg
Conceder acceso a un tablero en el canal de Slack

## Abrir enlaces de tablero

La versión más reciente de la aplicación de Slack para Miro abre enlaces a tableros de Miro mediante la inclusión de nombres, descripciones y miniaturas de los tableros.

abrir_enlace_tablero.jpg
*/span>Nombre, descripción y miniatura de tableros en el canal de Slack*

Reinstala tu integración de Slack para obtener acceso a la característica: ve a **Profile settings (Ajustes de perfil**) de Miro > Integrations (Integraciones) y haz clic en **Log out** (Cerrar sesión) junto a **Miro Feed (Slack App)** (Feed de Miro [Aplicación de Slack]).  Luego, haz clic en Connect (Conectar) y vuelve a autorizar.

:::note
Para reautorizar, es posible que tengas que recibir la aprobación del administrador del Espacio de trabajo de Slack.
:::

Para configurar una miniatura de tablero de Miro, accede a tu tablero y abre la tarjeta de información; para ello, haz clic en el título en la esquina superior izquierda de tu tablero. En la ventana emergente, haz clic en la imagen en la esquina superior izquierda y carga una imagen desde tu dispositivo o selecciona una sección del tablero. La miniatura aparecerá en Slack cuando compartas el enlace del tablero.

cambiar_miniatura_de_tablero.gif
Configuración de miniatura de tablero

## Cómo compartir un tablero desde Slack

Cuando se publica un enlace de tablero en Slack verás una notificación que muestra a los usuarios que no tienen acceso al tablero. Puedes invitarlos con facilidad al tablero directamente a través de Slack.  No dudes en [hacer público el tablero](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) para que cualquier persona con el enlace pueda verlo/comentarlo.

compartir_desde_Slack.jpg
/span>Cómo compartir un tablero de Miro desde Slack /em>

>  Si no tienes la opción disponible, reinstala la aplicación en la configuración o pídele a tu administrador que actualice el plugin en Slack Marketplace.

## Creación de un tablero desde Slack

Puedes usar el acceso directo de Miro para crear un tablero desde Slack.  Busca en Miro y elige **Create a board** (Crear tablero).

acceso_directo_Miro.jpg
Creación de un tablero desde Slack

Ingresa un título para el tablero, selecciona un equipo de Miro y agrega un mensaje breve para enviar junto con el enlace al tablero recién creado en Slack.

diálogo_crear_tablero.jpg
/span>Configuración de parámetros para un tablero nuevo en Slack

Una vez creado el tablero, se enviará el mensaje al canal o la conversación junto con el enlace del tablero.

nuevo_mensaje_tablero.jpg
Se publicará un mensaje después de crear un tablero nuevo desde Slack

Si algunos miembros del canal no tienen acceso al tablero recién creado, se te sugerirá que [compartas el tablero con ellos desde Slack](#h_007785b5-df52-43e2-9eb0-ccb53b795955).

## Cómo desactivar la aplicación

Para desactivar la integración, ve a **Profile settings (Configuración de perfil) > Integrations (Integraciones)** y haz clic en **Log out** (Cerrar sesión):

cerrar_sesión_Slack.jpg
Cómo deshabilitar el feed de Miro

Para eliminar la aplicación de Slack por completo, abre los ajustes de canal de **Miro** en Slack y haz clic en **Configuration** (Configuración).

configuración_Slack_Miro.jpg
Configuración de la aplicación de Miro para Slack

Se te redirigirá a la página de configuración de la aplicación de Miro. Desplázate hacia abajo, busca tu nombre en la lista de usuarios autorizados y haz clic en **Revoke** (Revocar).

revocar_acceso.jpg
Eliminación del acceso de Miro a Slack

Los Administradores del espacio de trabajo también verán la opción de eliminar la aplicación en *todo el espacio de trabajo*.

eliminar_aplicación.jpg
Eliminación de la aplicación de Slack

## Preguntas frecuentes y posibles problemas

1. Si un usuario añade Miro a Slack, ¿podrá Miro leer sus canales de Slack?
- No, Miro sólo viverá la información básica sobre los canales públicos del espacio de trabajo. Significa que Miro podrá leer la lista de nombres de los canales y no podrá leer los mensajes de los canales.

2. *Recibo el mensaje "Algo ha ido mal" cuando intento conectar el feed de Miro para Slack.*
- Comprueba si tu navegador permite las ventanas emergentes del dominio miro.com. Puede haber una página adicional en la que se pidan permisos de la aplicación./span>

3. 3. *No recibo notificaciones de Miro-Slack y reinstalar la aplicación Miro en Slack no es de ayuda.*  ¿Cómo puedo solucionarlo?
- Intenta volver a conectar Miro y Slack en el lado de Miro**(Configuración del perfil > Integraciones).**
