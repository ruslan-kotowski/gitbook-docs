---
title: Plugin de Miro para Sketch
article_id: 360017731173
translation_id: 360017731173
locale: es
sidebar_position: 13
created_at: '2019-02-11T10:13:46Z'
updated_at: '2025-02-26T12:15:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

El plugin de Miro para Sketch ofrece una manera fácil y rápida de pasar imágenes de Sketch directamente al tablero. Envía tus mesas de trabajo a Miro y actualízalas fácilmente con un solo clic. Sincroniza todas tus imágenes cada vez que hagas un cambio, sin volver a cargarlas.

### Cómo habilitar el plugin

1. 1. Descarga el plugin de Sketch desde GitHub: sigue [este enlace](https://github.com/miroapp/sketch_plugin) > **Código** > **Descargar ZIP**:

Download_from_Github.jpg

2. 2. Extrae el contenido del archivo zip > haz doble clic en el paquete de RealtimeBoard.sketchplugin para instalar el plugin.

plugin_installed.jpg
El plugin de Miro para Sketch está instalado

3. 3. Para encenderlo, abre Sketch, ve a **Plugins >** **Administrar plugins** y marca la casilla **Miro por Miro**.

Miro_plugin_in_Sketch.jpg
El plugin de Miro se activa en Sketch

4. 4. Después de eso, deberás autenticarte con tus credenciales de Miro. Para ello, haz clic en **Plugins -** **Miro:** **Entra en Miro, Sal de Miro**.

Log_in_to_Miro_in_Sketch.jpg
Iniciar sesión en Miro

5. 5. Escribe tu email y contraseña o haz clic en **Use company credentials** (Usar credenciales de empresa) si inicias sesión mediante SSO.

Miro_login.jpg
Ventana de autenticación para iniciar sesión en Miro

### Cómo añadir mesas de trabajo de Sketch a Miro

Para añadir una mesa de trabajo de Sketch a Miro, ve a **Plugins:** **Miro -** **Sincroniza todas las mesas de trabajo con Miro**.

La ventana de diálogo te dará la opción de elegir entre los tableros en los que tienes el rol de editor por medio de una invitación por correo electrónico o por medio del acceso a [proyectos](../../using-miro/sharing-boards/16-projects.md) por equipos.

> *⚠️ Ten en cuenta que los tableros en los que tengas el rol de [visitante](../../using-miro/sharing-boards/08-collaboration-with-visitors.md) no estarán disponibles.*

Selecciona un tablero a) haciendo clic en una de las sugerencias del menú desplegable o b) introduciendo el nombre del tablero. Después haz clic para añadir **todas** o **solo algunas mesas de trabajo**. Marca la casilla si quieres **abrir Miro después de la sincronización**:

select_a_board.jpg
Cómo seleccionar un tablero para la sincronización

Haz clic en **Sincronizar**, y las mesas de trabajo aparecerán en tu tablero.

artiboards_in_Miro.jpg
**Ten en cuenta que solo puedes enviar mesa de trabajo a tableros de Miro existentes**

:::warning
Ten en cuenta que copiar y pegar mesas de trabajo directamente solo está disponible para la versión de *navegador* de Miro.
:::

### Cómo sincronizar mesas de trabajo de Sketch con Miro

Para sincronizar las mesas de trabajo que ya fueron añadidas a Miro y después alteradas en Sketch, ve a **Plugins -** **Miro:** **Sincroniza todas las mesas de trabajo con Miro**. El tablero con el que hayas sincronizado previamente las mesas de trabajo se seleccionará automáticamente en la ventana de diálogo. Simplemente elige si quieres sincronizar **todas** las mesas de trabajo o **solo algunas**. Marca la casilla si quieres **abrir Miro después de la sincronización**:

syncing_boards.jpg
Cómo sincronizar mesas de trabajo con Miro

### Cómo deshabilitar el plugin

Para detener la sincronización entre Sketch y Miro, ve a **Plugins >** **Administrar plugins** y desmarca la casilla **Miro by Miro**.

disable_Miro_sync.jpg
El plugin de Miro se deshabilitará en Sketch

### Posibles dificultades y cómo resolverlas

|  |  |  |
| --- | --- | --- |
| **Mensaje de error/dificultad** | **Posibles causas** | **Solución** |
| 1. Se ha producido un error. Hubo un error durante la sincronización. Vuelve a intentarlo" | 1. 1. Estás usando una versión obsoleta de Sketch./span>  2. 2. Tu mesa de trabajo de Sketch es enorme (hay una imagen muy grande en la mesa de trabajo de Sketch). | 1. 1. Actualiza la versión más reciente del plugin de Sketch.  2. 2. Verifica el tamaño de la imagen y redúcelo si es necesario. |
| 2. Error de conexión Algo salió mal" | 1. 1. El plugin no se puede conectar con la API de Miro.  2. 2. La tarifa está limitada por la API de Miro.  3. 3. Hay otros problemas posibles con la red. | Cierra tu sesión y vuelve a entrar en tu perfil de Miro dentro de Sketch, e intenta sincronizar la mesa de trabajo de nuevo. |
| 3. Hubo un error durante la sincronización. Vuelve a intentarlo" | El problema puede estar siendo causado por cambios en los ajustes de tu red. | Registra las entradas de la consola y[envía un informe de error al Equipo de soporte de Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md). |
| 4. 4. El plugin de Sketch se congela y funciona de forma inesperada cuando intento sincronizar múltiples mesas de trabajo con Miro | Esto sucede cuando tienes un tablero de Miro enorme e intentas sincronizar múltiples mesas de trabajo mediante el plugin de Sketch. | Crea un nuevo tablero de Miro en Miro y sincroniza una mesa de trabajo a la vez con él. |
| 5. 5. Los tableros no me aparecen en los resultados de búsqueda de Sketch | Esto ocurre cuando un tablero fue trasladado a otro [proyecto](../../using-miro/sharing-boards/16-projects.md) en Miro o si no tienes un asiento en el proyecto donde se encuentra el tablero | 1. 1. Verifica si el tablero que no aparece en la lista de sincronización de Sketch se trasladó a otro proyecto dentro de Miro.  2. 2. Verifica si tienes un asiento en alguno de los proyectos donde se encuentra el tablero. |
| 6. 6. Sketch no reemplaza mesas de trabajo existentes en un tablero de Miro - se duplican en el lienzo en lugar de ser reemplazadas | Esto ocurre cuando un tablero que está sincronizado con Sketch ha sido [trasladado](../../using-miro/managing-boards/04-how-to-move-a-board.md) [a otro equipo de Miro](../../using-miro/managing-boards/04-how-to-move-a-board.md).  En este caso, las imágenes se duplicarán en la primera sincronización. Más adelante, serán reemplazadas. | Elimina las mesas de trabajo anteriores del tablero de Miro. Los duplicados serán reemplazados de nuevo. |

#### Cómo grabar registros de Sketch para Soporte de Miro

1. Abre Spotlight Search/span>(haz clic en el icono de lupa ubicado en la esquina superior derecha de la pantalla) >Console:

spotlight_search.jpg
Búsqueda de Spotlight

2. 2. Introduce s**ketch-rtb-error**en el campo de búsqueda de la consola y busca por mensaje/cualquiera:

search_in_Sketch.jpg
Buscar en la consola

3. 3. Haz clic en la línea con el mensaje en la sección inferior de la consola, toma una captura de pantalla y compártela con nosotros.

error_message.jpg
Mensaje de error de la consola
