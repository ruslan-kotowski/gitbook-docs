---
title: Enviar a pantalla
article_id: 4406230245010
translation_id: 7697999106450
locale: es
sidebar_position: 10
created_at: '2022-09-19T08:34:09Z'
updated_at: '2026-04-10T12:05:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: interactive-displays
---

Comienza a colaborar en segundos. Usa la función Enviar a pantalla para iniciar cualquier tablero de Miro en tu pantalla interactiva.

> ***Actualizaciones de la interfaz de usuario de Miro en despliegue gradual***
> Miro está mejorando la interfaz de usuario del tablero para que sea más inclusiva e intuitiva, e introduciendo una evolución de los proyectos llamada Espacios. El despliegue se producirá gradualmente para todas las cuentas de Miro a lo largo de varias semanas.
>
> En caso de que ya tengas la interfaz de usuario y el diseño de Espacios mejorados, este artículo puede describir los puntos de entrada que han cambiado.
>
> Para ver la documentación más actualizada, consulta [la nueva interfaz de usuario simplificada de Miro](../../using-miro/working-on-the-board/02-miro's-new-simplified-user-interface.md).
>
> Este artículo se actualizará cuando se haya completado el lanzamiento.

Aprende [a configurar Miro en tu pantalla interactiva](07-interactive-displays.md).

## Cómo usar Enviar a pantalla

1. En tu pantalla interactiva, abre la aplicación de Miro o abre el navegador y ve a [miro.com/displays](https://miro.com/displays/).
2. Abre el tablero de Miro en tu dispositivo personal.

**Desde tu portátil o tableta**

1. Desde el tablero de Miro en tu portátil o tableta, en la barra del tablero selecciona los tres puntos verticales.
   Se abrirá el menú **Principal**.
2. Selecciona **Enviar a la pantalla interactiva**.
3. Ingresa el código de sincronización único que ves en la pantalla interactiva. Esto enviará el tablero desde tu computadora portátil o tableta a la pantalla.

**Desde tu dispositivo móvil**

:::note
Si utilizas un dispositivo móvil, asegúrate de descargar la app móvil de Miro para [iOS](https://apps.apple.com/us/app/miro-collaborative-whiteboard/id1180074773) o [Android](https://play.google.com/store/apps/details?id=com.realtimeboard&hl=en&gl=US) primero.
:::

1. Desde el tablero de Miro en tu dispositivo móvil, toca el ícono de **configuración** en la esquina superior derecha.
   **![board_settings.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4967840616850_board%20settings.jpg)**
   *Abriendo las configuraciones del tablero en la app móvil*
2. Pulsa **Enviar a pantalla interactiva.**
   **![send_to_interactive_display.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4967865515794_send%20to%20interactive%20display.jpg)**
   ***La opción para Enviar a pantalla interactiva en la aplicación móvil***
3. Ingresa el código de sincronización único que ves en la pantalla interactiva. Esto enviará el tablero desde tu dispositivo móvil a la pantalla.
   ![enter_code.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4967892004114_enter%20code.jpg)
   *La opción para ingresar el código*

:::tip
Una vez que finalice la sesión, recuerda cerrar sesión en la pantalla para proteger tus datos. Si lo olvidas, se cerrará automáticamente después de 15 minutos de inactividad.
:::

## Resolución de problemas

Si no ves la pantalla de Enviar a pantalla en la aplicación de escritorio de Windows, prueba los pasos de resolución de problemas que se indican a continuación.

1. Instala la [app de Miro para escritorio](https://miro.com/apps/).
2. Haz clic con el botón derecho en el icono de la app de escritorio de Miro, selecciona **Propiedades**.
   ![properties.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4949111804946_properties.jpg)*Propiedades de la app de Miro*
3. Cambia a la pestaña **Acceso directo** y agrega el siguiente flag a los argumentos de la CLI en el campo **Objetivo** y haz clic en OK para aplicar los cambios.

   ```
   --public-device
   ```

   ![target_field.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4949083211538_target%20field.jpg)*La pestaña de Acceso directo en las propiedades de Miro*
4. Ahora la opción Enviar a pantalla se mostrará de forma predeterminada cada vez que inicies la aplicación.

:::tip
Aprende más sobre [qué pantallas son compatibles con Miro](07-interactive-displays.md) y [lee sobre cómo seleccionar la pantalla adecuada para la colaboración híbrida](09-selecting-the-right-interactive-display-for-hybrid-collaboration.md).
:::
