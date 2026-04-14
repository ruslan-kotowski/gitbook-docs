---
title: "C\xF3mo deshabilitar la ventana emergente de la aplicaci\xF3n de escritorio\
  \ de Miro en tu navegador"
article_id: 360019244239
translation_id: 360019244239
locale: es
sidebar_position: 5
created_at: '2021-01-29T12:48:31Z'
updated_at: '2026-03-06T13:37:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Si tienes la [aplicación de escritorio de Miro](../../../getting-started/apps-for-devices/05-desktop-app.md) instalada en tu dispositivo, cuando abras un tablero de Miro en un navegador, podrás ver la ventana emergente que sugiere que abras el tablero en la aplicación.

ventana_emergente_navegador.jpg
La ventana emergente del navegador que lleva a la aplicación de escritorio de Miro

Si quieres deshabilitar la ventana emergente, sigue las instrucciones a continuación.

- Para usuarios de Mac
- Para usuarios de Windows
- Navegador Safari

### Para usuarios de Mac

**Paso 1.** Elimina (desinstala) la app Escritorio de tu ordenador.

**Paso 2.** Anula la configuración "Abrir siempre la URL en la app Miro" en tu navegador. Así es cómo puedes hacerlo en Chrome y en Firefox.

*Para Chrome:*

1. Cierra todas las ventanas de Chrome + Miro antes de empezar (usa **C****md + Q** para salir del navegador).
2. Abre Finder en tu Mac > presiona **Command + Shift + G** > ingresa la siguiente ruta en el cuadro de búsqueda: **~/Biblioteca/Asistencia de aplicaciones/Google/Chrome**. Abre tu carpeta de perfil de Chrome, busca Preferencias.

   Puede haber varias carpetas con el archivo, prueba estas sugerencias:

   - Abre y busca **Preferencias**dentro de la carpeta **Predeterminada**, si tienes solo un perfil en Google Chrome.
   - Si tienes varios perfiles en Google Chrome, abre y busca **Preferencias**dentro de la carpeta **Perfil X**, en el que **X**  es un número de la lista de perfiles.
   - Abre y busca **Preferencias** dentro de cada carpeta (**Predeterminada, Perfil de invitado, Perfil X**), si existen.
3. Abre **Preferencias** en un editor de texto.
4. Busca **`https://miro.com":\{"miroapp":true\}`** .
5. Elimina **`https://miro.com":\{"miroapp":true\}`** .
6. Guarda los cambios.
7. Reinicia el navegador Chrome.

Si usas varios perfiles de Google, tendrás que editar las Preferencias en todos los catálogos. Para esto, en el paso 2, tendrás que abrir **~/Biblioteca/Asistencia de aplicaciones/Google/Chrome** y cambiar **las Preferencias** en las carpetas **Perfil 1, Perfil 2**, etc.

*Para Firefox:*

1. Abre los ajustes del navegador.
2. En la sección **General** desplázate hacia abajo hasta **Aplicaciones.**
3. Busca **miroapp** y cambia **Use Miro** (Usar Miro) (predeterminado) a **Always ask** (Preguntar siempre); para ello, selecciona la opción en el menú desplegable.

### Para usuarios de Windows

**Paso 1.** Elimina (desinstala) la app Escritorio de tu ordenador.

**Paso 2.** Utiliza el script disponible en [este enlace](https://desktop.miro.com/platforms/Miro_DeleteAppSchema.reg) para borrar el valor del registro de Windows*. Una vez que se haya hecho esto, la notificación no debería aparecer en tu navegador. Si la ventana emergente sigue apareciendo, sigue el paso 3.*

**Paso 3.** Anula la configuración "Abrir siempre la URL en la app Miro" en tu navegador. Así es cómo puedes hacerlo en Chrome y en Firefox.

*Para Chrome:*

1. Cierra todas las ventanas de Chrome + Miro antes de empezar.
2. *V*e a **PC** > **Usuarios > \{current_user\} > Datos de aplicaciones > Local > Google > Chrome > Datos de usuario > Predeterminado > Preferencias.**
3. Abre **Preferencias** en un editor de texto.
4. Busca **`https://miro.com":\{"miroapp":true\}`** .
5. Elimina **`https://miro.com":\{"miroapp":true\}`** .
6. Guarda los cambios.
7. Reinicia el navegador Chrome.

Si usas varios perfiles de Google, tendrás que editar las Preferencias en todos los catálogos. Para esto, ve a **PC** > **Usuarios > \{current_user\} > Datos de aplicaciones > Local > Google > Chrome > Datos de usuario** y cambia **las Preferencias** en las carpetas **Perfil 1, Perfil 2**, etc.

*Para Firefox:*

1. Abre los ajustes del navegador.
2. En la sección **General** desplázate hacia abajo hasta **Aplicaciones.**
3. Busca **miroapp** y cambia **Use Miro** (Usar Miro) (predeterminado) a **Always ask** (Preguntar siempre); para ello, selecciona la opción en el menú desplegable.

### Navegador Safari

Si tienes que deshabilitar la ventana emergente en Safari, elimina la aplicación de escritorio de Miro de tu dispositivo.
