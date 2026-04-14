---
title: "C\xF3mo solucionar problemas e informar de un error"
article_id: 360017731413
translation_id: 360017731413
locale: es
sidebar_position: 7
created_at: '2019-02-11T10:14:28Z'
updated_at: '2025-11-25T16:03:12Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Si estás experimentando problemas de rendimiento o no puedes usar Miro, aquí te contamos cómo informar del error al servicio de soporte de Miro.

## Antes de informar de un error

1. Consulta la [página de estado de Miro](https://status.miro.com/) para ver si hay informes de degradación potencial del rendimiento
2. Comprueba si el problema se reproduce en modo [incógnito](https://support.google.com/chrome/answer/95464)  **(privado)** y en un **navegador diferente**
3. [Deshabilitar las extensiones del navegador](https://support.box.com/hc/articles/360044196613-How-To-Disable-Plugins-Add-Ons-Extensions-In-Multiple-Browsers). A veces chocan con los procesos de Miro (por ejemplo, gramaticalmente con los widgets del texto).
4. Si trabajas en la aplicación de Escritorio, [reinicia los datos de la aplicación](../../../getting-started/apps-for-devices/05-desktop-app.md)
5. Si experimentas problemas de rendimiento en un tablero específico, prueba [a duplicarlo](../../managing-boards/03-how-to-duplicate-a-board.md) y observa si el problema persiste en el tablero copiado
6. Consulta nuestras guías de resolución de problemas:

- [Problemas de rendimiento y carga del tablero](../../tools/troubleshooting/04-board-performance-and-loading-issues.md)
- [No puedo iniciar sesión](../../tools/troubleshooting/09-i-can't-log-in.md)
- [No puedo acceder o editar un tablero de Miro](../../tools/troubleshooting/08-i-can't-access-or-edit-a-miro-board.md)
- [Problemas con la exportación de tableros](../../tools/troubleshooting/03-board-export-issues.md)
- [Perdí mi tablero o mi contenido](../../tools/troubleshooting/11-i-lost-my-board-or-content.md)
- Otras guías

## Cómo enviar un error

Proporciona tantos detalles como sea posible: esto nos ayudará a entender tu problema de inmediato para que podamos ayudarte mejor.

1. Incluye una descripción del problema y envía capturas de pantalla, GIF o un [video corto](https://chrome.google.com/webstore/detail/openvid-screen-recorder-c/liecbddmkiiihnedobmlmillhodjkdmb).  Además,

- si el problema ocurre en un tablero específico, [comparte el tablero](../../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) con [support@help.miro.com](mailto:support@help.miro.com), de ser posible con derecho a editar
- Si el problema está relacionado con un archivo subido específico, envíanos el archivo

2. Especifica tu dispositivo, sistema operativo y versión de navegador
3. Proporciona tu consola de navegador y registros de red o registros de tus aplicaciones de escritorio

### Cómo grabar registros de consola

**Cómo grabar registros de la consola de navegador**

1. Desde el tablero de Miro, **haz clic en la barra de direcciones** de tu navegador (usa este paso si el problema se repite en uno de tableros en lugar de hacerlo en la página de ajustes o en el panel de control)mceclip1.png
2. Presiona **F12**o **fn + F12** para abrir las herramientas de desarrollador del navegador
3. Elige **la pestaña Red** y marca la casilla **Preservar registros**
4. Vuelve a cargar la página
5. Intenta reproducir el problema de nuevo
6. Haz clic en Download Arrow (flecha para descargar) para **Exportar** los registros HAR de la red
   registros_de_consola_de_red.jpg
7. Cambia a la pestaña **Console (consola)**, haz clic con el botón derecho en los registros y elige **Save as (guardar como)**save_console_logs.jpg
8. Envíanos los  archivos .log y .har. Si el archivo no se adjunta a tu ticket debido a su tamaño, súbelo a cualquier espacio de almacenamiento en la nube y envíanos el enlace (permite que cualquier persona con el enlace pueda descargar los archivos).

**Cómo grabar registros de la aplicación de escritorio en Mac**

Si experimentas un error en la aplicación de escritorio en Mac, envíanos el detalle de los registros.

1. Desde la aplicación de escritorio, haz clic en **Ayuda** en la esquina superior izquierda.  Selecciona **Abrir herramientas de desarrollo para pestañas**​​​​​​​​
   open_developer_tools_for_tabs.jpg
2. ​Cambia a la pestaña **Red**.​​​ Marca la casilla **Conservar registros**
3. Abre el tablero donde deseas solucionar el problema (omite el paso si no puedes acceder a tableros)
4. Vuelve a cargar la página con el acceso directo **Ctrl + R**
5. Reproduce el problema
6. Haz clic en Download Arrow (flecha para descargar) para Exportar los registros HAR de la red
   preserve_logs.jpg
7. Cambia a la pestaña **Console (consola)**, haz clic con el botón derecho en los registros y elige Save as (guardar como)save_as_.jpg
8. Vuelve a hacer clic en **Ayuda** > selecciona **Abrir herramientas de desarrollo** y repite los pasos del 2 al 7. Esto recopilaría otro tipo de registro que nos proporcionaría un conjunto diferente de datos, para investigar el problema más a fondo para ti
9. Envíanos los  archivos .log y .har. Si el archivo no se adjunta a tu ticket debido a su tamaño, súbelo a cualquier espacio de almacenamiento en la nube y envíanos el enlace (permite que cualquier persona con el enlace pueda descargar los archivos).

**Cómo grabar registros de la aplicación de escritorio en Windows**

Si experimentas un error en la aplicación de escritorio en Windows, envíanos el detalle de los registros.

1. Mientras estás en la app de escritorio pulsa **Alt** > pulsa **Ayuda** > **Abrir para pestañas![open_developer_tools_for_tabs_on_Windows.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020264830994_open%20developer%20tools%20for%20tabs%20on%20Windows.jpg)**
2. ​Cambia a la pestaña **Red**.​​​ Marca la casilla **Conservar registros**
3. Abre el tablero que en el que deseas solucionar el problema (omite este paso si no puedes acceder a tableros)
4. Presiona **Ctrl + R** para volver a cargar la página C**trl + R**
5. Reproduce el problema
6. Haz clic en el icono Descargar para exportar los registros HAR de la red
   preserve_logs.jpg
7. Cambia a la pestaña **Console (consola)**, haz clic con el botón derecho en los registros y elige Save as (guardar como)
   save_as_.jpg
8. Vuelve a abrir la **Ayuda** > elige **Abrir herramientas de desarrollo** y repite los pasos del 2 al 7. Esto recopilaría otro tipo de registro que nos proporcionaría un conjunto diferente de datos, para investigar el problema más a fondo para ti
9. Envíanos los  archivos .log y .har. Si el archivo no se adjunta a tu ticket debido a su tamaño, súbelo a cualquier espacio de almacenamiento en la nube y envíanos el enlace (permite que cualquier persona con el enlace pueda descargar los archivos).

### Cómo recopilar un informe del navegador

Cuando informas de problemas de carga o de rendimiento, compartir la información ampliada de la versión del navegador ayuda al Soporte de Miro a diagnosticar el problema. Puedes encontrar esta información introduciendo un comando específico en la **barra de direcciones** de tu navegador. A continuación, encontrarás cómo acceder a esta información en distintos navegadores.

- **Chrome**: chrome://version
- **Microsoft Edge**: edge://versión
- **Firefox**: about:Soporte (o about:versión en algunas versiones)
- **Opera**: opera://acerca de
- **Navegador Yandex**: browser://version

> **✏️** Mira [Cómo contactar al equipo de soporte de Miro.](../../tools/troubleshooting/06-contacting-miro-support.md)
