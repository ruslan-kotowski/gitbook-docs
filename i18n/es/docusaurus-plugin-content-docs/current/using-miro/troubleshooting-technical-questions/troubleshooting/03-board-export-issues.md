---
title: "Problemas con la exportaci\xF3n de tableros"
article_id: 360020567820
translation_id: 360020567820
locale: es
sidebar_position: 3
created_at: '2021-03-18T12:15:46Z'
updated_at: '2025-11-05T13:45:32Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Puedes [exportar tu tablero de Miro](../../import-and-export/export/03-how-to-export-your-board.md) como imagen, PDF o archivo CSV. Si tienes problemas para exportar tu tablero de Miro, revisa las posibles soluciones a continuación.

## No puedo exportar el tablero

**El botón de exportación no aparece en mi tablero**

El botón de exportación se encuentra en el menú de **tres puntos** (**...**), luego en el submenú de **Tablero**.

No hay opción de exportar en el [menú del tablero](../../../getting-started/start-here/your-first-board/05-toolbars.md):

1. Verifica que el propietario o el copropietario del tablero haya permitido la exportación del tablero para los usuarios en la configuración del contenido del tablero.

   Para averiguar el nombre del propietario del tablero, haz clic en el nombre del tablero en la esquina superior izquierda para abrir la tarjeta de información del tablero. Si no tienes permiso para ver esta información, puedes verificar el nombre del usuario que te invitó al tablero en el correo de invitación.

   Comunícate con el propietario del tablero y pídele que habilite la opción para ti en la ventana de **Compartir** > **Configuración de uso compartido** > **Permisos**. El propietario/copropietario necesita seleccionar qué categoría de usuarios puede [copiar el contenido del tablero](../../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md).
   ![.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044218642_.gif.png)
   *Configurando quién puede copiar el tablero*
2. Asegúrate de que tu navegador, plan y dispositivo sean compatibles con la exportación. Puedes consultar la disponibilidad a continuación. Si tu navegador, plan o dispositivo no son compatibles con la opción de exportación, recomendamos cambiar a otro navegador o dispositivo o [mejorar tu equipo](../../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md).

   |  |  |  |  |  |  |
   | --- | --- | --- | --- | --- | --- |
   |  | Plan Free | | Planes Starter, Business, Enterprise y Education | | Exportar a CSV (todos los planes) |
   |  | Baja resolución | Alta resolución sin marca de agua | Baja  resolución | Alta resolución  sin marca de agua |
   | Google Chrome | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Safari | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Firefox | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Opera | ✔ | ✘ | ✔ | ✔ | ✘ |
   | Edge < 79 | ✘ | ✘ | ✘ | ✔ | ✘ |
   | [Aplicación de escritorio](../../../getting-started/apps-for-devices/05-desktop-app.md) | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Tableta | ✔ | ✘ | ✔ | ✔ | ✘ |
   | Móvil | ✘ | ✘ | ✘ | ✘ | ✘ |

**Para exportaciones de baja calidad**

Para solucionar problemas, cierra las pestañas del navegador y las pestañas de fondo. También puedes intentar cambiar de navegador.

Para exportaciones de alta calidad, haz lo siguiente:

- Oculta los marcos que no desees exportar. El contenido en los marcos ocultos no se exporta.
- Divide el tablero en tableros más pequeños para exportarlos.

**Consejos generales**

- Pon todo lo que quieras exportar en marcos, ya que solo se exportan los widgets dentro de los marcos.
- Evita PDF en PDF. Si tienes un PDF en un tablero que deseas exportar como PDF, reemplaza el PDF en el tablero con imágenes de baja calidad.
- Convierte imágenes de alta resolución a JPEG o redúcelas con una herramienta externa.
- Revisa la página de estado de Miro para conocer los incidentes pertinentes.
- Divide el tablero en marcos y exporta cada marco por separado. Los PDFs separados se pueden volver a unir con una herramienta externa.
- Divide tableros grandes en tableros más pequeños y usa [espacios](../../spaces/01-spaces.md) para ayudarte a mantenerte organizado y agrupar tableros que pertenezcan juntos.

**“Lo sentimos, ocurrió un error durante la generación del documento PDF”**

Prueba a dividir el tablero en marcos y exporta los marcos por separado, ya que el problema podría deberse al tamaño del tablero.

Si eso no ayuda, revisa [los registros de consola de tu navegador](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md). Si los registros contienen el siguiente mensaje:

```
ERR_CONNECTION_ABORTED
```

*donde:*

La exportación está bloqueada por un software de seguridad en tu dispositivo o un firewall dentro de tu red.

Tú o tu administrador del sistema deben configurar los ajustes de tu programa de antivirus y/o firewall para permitir que Miro realice el procedimiento de exportación.

En caso de duda, [contacta al soporte de Miro](../../tools/troubleshooting/06-contacting-miro-support.md).

**No pasa nada cuando intento exportar un tablero a PDF, y Miro no muestra ningún error**

Este es un problema conocido que ocurre principalmente en el navegador Safari, cuando las ventanas emergentes están deshabilitadas. Para resolver el problema en Safari, [sigue estos pasos](https://support.apple.com/en-gb/guide/safari/sfri40696/mac). Asegúrate de habilitar las ventanas emergentes para miro.com o para todos los sitios web. Vuelve a Miro e intenta nuevamente exportar tu tablero.

Para Chrome, [sigue estos pasos](https://support.google.com/chrome/answer/95472?hl=en&co=GENIE.Platform%3DDesktop).

## Tengo problemas con los archivos exportados (PDF, imágenes, CSV)

**Las imágenes o los archivos PDF aparecen borrosos en el documento exportado**

Realiza esto si las imágenes cargadas o los archivos PDF están borrosos en tu archivo guardado:

1. Establece el zoom del tablero en 100% y deja que las imágenes o los archivos PDF se rendericen antes de exportar el tablero.
2. La imagen cargada o el archivo PDF pueden ser demasiado complejos o grandes como para exportarlos. Para reducir el tamaño del archivo, conviértelo a formato PNG y reemplázalo en el tablero. Luego, vuelve a exportar el tablero.

El plan Free solo es compatible con la exportación en baja calidad. Si necesitas exportar tu tablero en alta calidad, te recomendamos [moverlo a un equipo de pago](../../managing-boards/04-how-to-move-a-board.md) o [mejorar tu plan](../../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md).

**El orden de las páginas no es el mismo que el orden de los marcos en el tablero**

El orden de los marcos exportados a PDF es el mismo que en el panel de marcos. Para cambiar el orden de los marcos:

1. Abre la descripción general del tablero en la esquina inferior izquierda
2. Arrastra los marcos para cambiar su posición en la lista. También puedes usar [Magic organize](../../essential-tools/07-frames.md) para organizar rápidamente tus marcos en el orden en el que se encuentran en el tablero
   ![move_frames.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057584914_move%20frames.gif)
   *Cambiando el orden de los marcos*

**El archivo exportado se corta**

Si **exportas el tablero como una imagen**, asegúrate de incluir todo el contenido que quieres exportar en el área exportada seleccionada.

![save_as_image.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057583890_save%20as%20image.gif)
*Exportar un tablero como imagen*

Si **exportas el tablero como PDF**, asegúrate de crear un marco que incluya todo el contenido que deseas exportar. Luego [exporta el marco](../../import-and-export/export/03-how-to-export-your-board.md).

**El archivo PDF exportado no contiene los nombres de los marcos**

Cuando exportas tu tablero como un archivo PDF, los títulos de los marcos no están incluidos en la exportación. Puedes reemplazar los títulos de los marcos usando la [herramienta de texto](../../essential-tools/16-text.md) y poner el texto en los marcos. Los títulos aparecerán en tu archivo PDF.

**Los datos en un archivo CSV exportado no están estructurados**

Por el momento, la exportación en CSV no mantiene la estructura ni las relaciones del tablero. Sin embargo, si exportas [tablas](../../advanced-tools/05-grid.md) como un archivo CSV, la estructura queda guardada.

Si necesitas exportar un [mapa mental](../../advanced-tools/03-mind-map.md) como un archivo con datos inteligentes, utiliza el [descargador de Mapas Mentales](https://miro.com/marketplace/mindmapdownloader/?backUrl=%2Fmarketplace%2F).

**Las fuentes en el tablero son diferentes a las fuentes en el archivo exportado**

La exportación de Miro usa las fuentes instaladas en el sistema operativo de tu dispositivo. Si la fuente no está presente en tu sistema operativo, se usará en su lugar una fuente similar de tu sistema. Si necesitas la misma fuente que en tu tablero de Miro, elige una fuente diferente en el tablero o instala la fuente deseada en tu dispositivo.

## No puedo encontrar el archivo exportado

**No encuentro el archivo exportado en mi dispositivo**

**Si usas Miro en un navegador**

Los archivos se almacenarán en la carpeta en la que las descargas del navegador se guardan de forma predeterminada. Puedes consultar las opciones de descarga en la configuración del navegador.

**Si usas la aplicación de escritorio de Miro o la aplicación para tabletas**

Revisa la carpeta Descargas en tu dispositivo. También puedes buscar en tus archivos mediante el nombre del tablero.

**Miro crea una carpeta nueva cada vez que exporto un tablero**

> **Relevante para**: [aplicación de escritorio de Windows](../../../getting-started/apps-for-devices/05-desktop-app.md)

Es posible que la ruta se haya guardado en la configuración de la app de Miro. Para eliminar la ruta:

1. Elimina la aplicación de escritorio de Miro
2. En la parte inferior izquierda de Windows (barra de búsqueda), escribe **%AppData%** y abre la carpeta **Local,** luego elimina la carpeta **RealTimeBoard**
3. Abre **%AppData%** de nuevo, navega a la carpeta **Roaming,** y elimina la carpeta **RealTimeBoard**

Reinstala la última [aplicación de Miro](https://miro.com/apps/).

Si ninguna de las soluciones funciona, [contacta al soporte de Miro](../../tools/troubleshooting/06-contacting-miro-support.md).
