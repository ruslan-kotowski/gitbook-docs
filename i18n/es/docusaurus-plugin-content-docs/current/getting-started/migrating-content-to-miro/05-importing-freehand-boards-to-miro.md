---
title: Importar tableros de Freehand a Miro
article_id: 18580556555538
translation_id: 18580556555538
locale: es
sidebar_position: 9
created_at: '2024-04-26T16:34:28Z'
updated_at: '2025-11-25T15:42:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Personas: Todos los usuarios con planes elegibles Planes: Starter, Business,
    Education, Enterprise Plataformas: Navegador, Escritorio, Móvil (para acceder
    a Miro e iniciar la importación)'
---

Este artículo explica cómo importar tableros de Freehand a Miro, incluyendo cómo preparar tus tableros de Freehand, para importaciones individuales y en bloque.

:::note
Las ediciones que hagas a contenido importado en Miro no se sincronizan con su contenido original en Freehand.
:::

:::note
Solo puedes importar tableros de Freehand que están bajo licencias Free o Limitadas.
:::

## Importar un solo tablero de Freehand a Miro

Puedes importar fácilmente tableros individuales de Freehand a Miro exportándolos en el formato de archivo `.RTB` de Miro. Mira cómo hacerlo:

1. Accede al tablero de Freehand que deseas exportar a Miro.
2. Descarga el archivo en .RTB, el formato propietario de Miro, directamente desde Freehand. Ve al menú **Herramientas** y selecciona **Exportar a tablero de Miro**. El archivo se guardará en tu carpeta de descargas predeterminada. Freehand te avisará cuando se haya completado la descarga.
3. Abre tu panel de Miro.
4. En el área superior derecha del panel de Miro, haz clic en el botón **+ Crear nuevo**, haz clic en **Importar**, y luego haz clic en **Importar copia de seguridad**.
5. Elige el archivo `.RTB` previamente descargado de tu sistema.
6. Todo el contenido se importa ahora a un nuevo tablero de Miro en un formato editable.
7. Aunque la mayoría del contenido pasará sin problemas, puede que sea necesario realizar pequeños ajustes debido a las variaciones en las opciones de estilo y formato entre Freehand y Miro. Consulta Entender la creación de mapas de objetos de Freehand en Miro para obtener orientación sobre posibles diferencias.

## Importación masiva de varios archivos de Freehand a Miro

Para migrar varios tableros de Freehand a la vez, Miro ofrece un proceso de importación en bloque. Primero, asegúrate de que tus tableros de Freehand estén preparados correctamente.

**Requisitos previos: Prepara tus tableros de Freehand para la importación masiva**

Sigue estos pasos en Freehand para preparar tus tableros:

1. En Freehand, en la barra de menú del panel izquierdo, selecciona **Documentos**. Se abre un menú desplegable.
2. Selecciona **Todos los Documentos** o **Creados por Mí**, y especifica el periodo para los tableros que quieres importar a Miro.
3. Para cada tablero que quieras importar, selecciona los tres puntos (**...**) y elige **Select**.
4. En el diálogo en la parte inferior de tu pantalla, selecciona **Mover**.
5. Selecciona un espacio para mover tus tableros. Esto los consolida para facilitar el procesamiento por la herramienta de importación masiva.

   Has preparado con éxito varios archivos para la importación masiva a Miro.

Para realizar la importación masiva de tus tableros de Freehand preparados a Miro, sigue las instrucciones proporcionadas en la siguiente guía del tablero Miro incrustado:

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="460" scrolling="no" src="https://miro.com/app/embed/uXjVKB1IT00=/?pres=1&amp;frameId=3458764590689727256&amp;embedId=507813406404&amp;&amp;autoplay=yep" width="100%"></iframe>

:::note
Notas importantes para la importación masiva:
- El token de Freehand utilizado para la migración masiva es válido solo por dos semanas desde la fecha en que lo recibiste.
- A partir del 31 de diciembre de 2024 a las 11:59 PM EST, Freehand y todos los tokens de migración asociados serán descontinuados e invalidados. Los usuarios ya no podrán generar nuevos tokens ni acceder a Freehand para la migración.
:::

## Revisar las prácticas recomendadas

Para una experiencia de migración fluida, es importante entender las mejores prácticas y consideraciones clave al mover tu contenido de Freehand a Miro. Por favor, revisa la guía detallada en el tablero insertado de Miro a continuación:

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="460" scrolling="no" src="https://miro.com/app/embed/uXjVKB1FWSM=/?pres=1&amp;frameId=3458764590691451227&amp;embedId=480338444592&amp;autoplay=yep" width="100%"></iframe>

## Mapeo de objetos en Miro

Esta tabla proporciona una comparación exhaustiva de cómo los objetos de Freehand se suelen importar y representar en Miro, junto con notas sobre cualquier ajuste manual que pueda ser necesario:

|  |  |  |
| --- | --- | --- |
| **Freehand** | **Miro** | **Retoques necesarios** |
| Tableros | Kanban | Ninguna |
| Tarjetas | Tarjetas | Las tarjetas de Jira en Freehand se importarán como tarjetas de Jira en Miro. Sin embargo, no se conectarán a la instancia existente, ya que los usuarios tendrán que volver a autenticar sus cuentas de Jira en Miro.    Las tarjetas de ADO, Trello y Asana no son compatibles. |
| Colaboradores y uso compartido | Se puede recrear manualmente | Ninguno |
| Comentarios | Se puede recrear manualmente | Ninguno |
| Conectores/Líneas | Conectores/Líneas | Ninguno |
| Dibujos/Diagramas/Formas | Formas, texto y conectores | Ninguno |
| Tablas de datos dinámicas | CSV | El contenido puede descargarse y editarse como archivo .CSV desde el tablero de Miro. |
| Inserciones    Google y Microsoft Documentos, YouTube, Spotify, Loom | Nombre de la fuente (por ejemplo, Google, YouTube) y la URL para la incrustación | Si los usuarios desean volver a insertar un documento, pueden [cargarlo a través de URL](../../using-miro/import-and-export/import/05-uploading-files-to-boards.md). |
| Reacciones de emojis | Se puede recrear manualmente | Ninguno |
| Marcos | Marcos | Ninguno |
| Cuadrículas (tablas) | Tablas | Ninguno |
| Objetos agrupados | Objetos no agrupados | Para reagrupar objetos, selecciona todos los objetos relevantes y pulsa **Cmd/Ctrl + G**, o haz clic en **Agrupar objetos** en el menú contextual. |
| Imágenes | Imágenes | Ninguno |
| Páginas | Documento incrustado | El contenido puede descargarse y editarse como archivo .docx desde el tablero de Miro. |
| Prototipos | Nombre de la fuente (InVision) y la URL de la incrustación | Si los usuarios desean volver a incrustar un documento, pueden cargarlo a través de la URL para volver a incrustarlo. |
| Widgets inteligentes:    Tarjeta giratoria, Encuesta, Esto o Aquello, Gráficos, Contador, Tabla de clasificación, Ruleta, Zumbador, Personas, Puntos de historia, Tallas de camiseta, Temporizador, Botones de acción | Se crea un PNG del widget inteligente en el momento de la importación | El contenido no es editable. |
| Notas adhesivas | Notas adhesivas | Es posible que haya que ajustar el tamaño del texto de las notas adhesivas. |
| Línea de tiempo (Gantt) | CSV | El contenido puede descargarse y editarse como archivo .CSV desde el tablero de Miro. |
| Esquemas de página | Esquemas de página | Puede que haya que volver a dibujar algunos objetos. |

## Limitaciones clave

Ten en cuenta las siguientes limitaciones y diferencias estructurales al migrar tu contenido de Freehand a Miro para garantizar una transición más fluida:

- Los cuadros de texto de Miro pueden contener hasta 6000 caracteres, incluidos los espacios. Cualquier texto adicional se recortará.
- Las notas adhesivas de Miro no admiten ajustes de la paleta de colores ni viñetas de texto de la misma forma que Freehand; algunos formatos pueden diferir.
- Los widgets inteligentes de Freehand se importan como imágenes estáticas (PNG) y no son editables en Miro.
- Los comentarios, reacciones con emojis y prototipos de Freehand no se migran a Miro.
- El token de Freehand requerido para la importación masiva es válido solo por dos semanas desde la fecha en que lo recibiste.
- A partir del 31 de diciembre de 2024 a las 11:59 PM EST, Freehand y todos los tokens de migración asociados serán descontinuados e invalidados. Los usuarios ya no podrán generar nuevos tokens ni acceder a Freehand.

### Compara la estructura organizativa entre Freehand y Miro

Para planificar tu migración de manera efectiva, es importante comprender cómo las estructuras organizativas en Freehand corresponden a las de Miro:

**Capas organizativas de Freehand**

- Equipos: Cada subdominio al que tienes acceso en InVision se considera un Equipo. Si solo tienes acceso a un subdominio, tienes un equipo.
- Grupos: Carpetas de documentos que ayudan a agrupar y compartir documentos en tu equipo.
- Espacios: Una capa adicional de organización dentro de los grupos para tus documentos.

:::note
Si tu equipo utilizó la función de visión general del Espacio en Freehand, necesitarás migrar manualmente este contenido a Miro. Recomendamos copiar el contenido de la visión general del espacio a un tablero de Miro.
:::

**Capas organizativas de Miro**

- Organizaciones: Normalmente solo tienes acceso a una sola organización en Miro.
- Equipos: Espacios de trabajo compartidos donde los usuarios colaboran en tableros y proyectos (anteriormente conocidos como Espacios en algunos contextos, ten en cuenta la evolución de la terminología de Miro; generalmente, los equipos son el espacio de trabajo colaborativo principal).
- Proyectos: colecciones de tableros dentro de un equipo, lo que facilita la organización, recuperación y uso compartido de tableros.

Considera que tus Grupos InVision son aproximadamente equivalentes a los Proyectos de Miro (o lo que podría haber sido conceptualmente similar a carpetas/espacios para organizar tableros dentro de un equipo). Para cada grupo de InVision que planees migrar, te recomendamos crear un proyecto de Miro con el mismo nombre. Por ejemplo, si tuvieras un grupo de InVision llamado "Acme Corp Relaunch Project", te sugerimos crear un Proyecto de Miro con el mismo nombre, "Acme Corp Relaunch Project", dentro del Equipo de Miro correspondiente.

:::tip
Si tienes más preguntas sobre la migración a Freehand, ponte en contacto con [el equipo de Soporte de Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) o directamente con tu gerente de Customer Success de Miro.
:::
