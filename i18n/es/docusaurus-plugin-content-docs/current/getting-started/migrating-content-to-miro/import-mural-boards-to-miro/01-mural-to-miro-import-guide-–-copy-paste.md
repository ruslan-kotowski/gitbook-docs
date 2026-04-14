---
title: Guía de importación de Mural a Miro – Copiar y pegar
article_id: 22957521683986
translation_id: 22957521683986
locale: es
sidebar_position: 1
created_at: '2024-11-29T13:36:36Z'
updated_at: '2025-11-25T15:49:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Personas: Usuarios con acceso de edición Planes: Free, Starter, Business,
    Enterprise y Education Plataformas: Navegador, Escritorio, Móvil'
---

Puedes transferir contenido de tus tableros de Mural a Miro utilizando el método de copiar y pegar. Esta guía proporciona las mejores prácticas para este método de importación, explica el proceso paso a paso y detalla lo que puedes esperar respecto a la apariencia y el comportamiento de varios objetos una vez que son pegados en Miro.

## Directrices para importar desde Mural

Seguir estas directrices te ayudará a lograr los mejores resultados al transferir contenido de Mural a Miro.

Para datos estructurados, como los mapas mentales de Mural, el método de copiar y pegar es generalmente la mejor opción para evitar romper las conexiones entre los elementos.

:::note
Para importar contenido a Miro usando este método, el contenido de Mural debe estar bajo una licencia completa o una licencia gratuita limitada en Mural.
:::

El método de copiar y pegar también se recomienda para importar widgets individuales que no son compatibles con la [guía de importación de Mural a Miro (PDF)](02-mural-to-miro-import-guide-–-pdf.md), o para widgets que no se importan con alta fidelidad usando el método PDF.

Ten en cuenta algunas limitaciones del método de copiar y pegar: ciertos atributos de estilo y cualquier imagen que se haya cargado originalmente en Mural (en lugar de enlazada a través de URL) no se copiarán en tu portapapeles y, por lo tanto, no se transferirán a Miro.

## Copiar y pegar contenido de Mural a Miro

El siguiente procedimiento explica cómo copiar contenido de un tablero de Mural y pegarlo en un tablero de Miro.

**Requisitos previos**

Asegúrate de tener acceso de edición tanto al tablero de origen en Mural como al tablero de destino en Miro.

Para copiar contenido de un tablero de Mural y pegarlo en un tablero de Miro:

1. En Mural, selecciona los objetos que quieres copiar.
   > 💡 Para seleccionar todos los objetos en el tablero de Mural, usa el atajo de teclado **Ctrl+A** (Windows) o **Cmd+A** (Mac).
2. Para copiar los objetos seleccionados, utiliza el atajo de teclado **Ctrl+C** (Windows) o **Cmd+C** (Mac).
   Tus objetos de Mural se han copiado a tu portapapeles.
3. En Miro, abre el tablero donde quieras pegar el contenido. Usa el atajo de teclado **Ctrl+V** (Windows) o **Cmd+V** (Mac) para pegar.

   Has copiado y pegado contenido correctamente de Mural a Miro.
   > ✏️ El contenido pegado desde Mural puede requerir algún ajuste manual en Miro. Ciertos aspectos de estilo y formato pueden aparecer de manera diferente después de pegar.

## Apariencia del objeto después de pegar

Los objetos de Mural generalmente se copian y pegan en Miro con algunas variaciones respecto a su estado original. Esta sección describe los resultados esperados para algunos objetos comunes y proporciona prácticas recomendadas cuando sea aplicable.

### Áreas

Las áreas de Mural se copian y pegan como marcos y formas en Miro.

Un área de Mural con 100% de transparencia mostrará un borde transparente pero visible cuando se pegue en Miro. Si el área de Mural tiene un título, este título aparece y se comporta en Miro como un título del marco.

![Área del mural con título, y fondo y borde 100% transparentes.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Un área libre de Mural con título y fondo y borde 100% transparentes*

![Un área pegada de Mural a Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Un área pegada de Mural a Miro*

### Conectores

Los conectores de Mural se copian y pegan como conectores de Miro.

Para etiquetas de conectores, las posiciones verticales y horizontales se pegarán a Miro como centradas. Miro solo admite una posición centrada para las etiquetas de los conectores.

Con respecto a los tipos de conectores, Miro admite líneas *sólidas*, *punteadas* y *discontinuas*. Mural además incluye un tipo de conector *ligeramente punteado*. Miro conecta los tipos de líneas pegadas desde Mural de la siguiente manera: *línea sólida* se mantiene como *línea sólida*, y el tipo de línea *línea débilmente discontinua* de Mural se convierte en el tipo *línea discontinua* de Miro. Otras coincidencias directas (como de punto a punto) también se preservan.

Miro admite cada tipo de curva conectora de Mural, aunque su apariencia en Miro podría diferir ligeramente.

![Una curva de conector de Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Curva del conector de Mural*

![Una curva de conector de Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Curva del conector de Miro*

### GIFs e imágenes

Los GIFs e imágenes que se añadieron originalmente a Mural desde una URL se pueden copiar y pegar en Miro.

:::note
Un GIF o imagen en Mural que fue cargado directamente desde un dispositivo o agregado desde la barra de herramientas de Mural no puede ser copiado y pegado a Miro usando este método.
:::

### Mapas mentales

Mapas mentales de Mural se pueden copiar y pegar como mapas mentales de Miro, incluyendo el nodo raíz, cada nodo hijo y su texto.

El estilo del nodo raíz se conserva en su mayoría. Sin embargo, es posible que el radio de las formas difiera y que el tamaño de la fuente del texto no se conserve al pasar de Mural a Miro.

Los nodos hijos de Mural se pegan como nodos de texto en Miro, y su estilo no se conserva.

El color y el grosor del conector en el mapa mental también pueden diferir.

![Un mapa mental copiado en Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)
*Mapa mental copiado en Mural*

![Un mapa mental copiado de Mural a Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mapa mental copiado a Miro*

Para los mapas mentales de Mural que tienen múltiples niveles de nodos, el orden de los nodos puede cambiar al pegarse en Miro.

![Un mapa mental en Mural con múltiples niveles de nodos.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mapa mental en Mural con múltiples niveles de nodos*

![Un mapa mental con múltiples niveles de nodos copiados de Mural a Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mapa mental con múltiples niveles de nodos copiados de Mural a Miro*

:::tip
Los mapas mentales copiados de Mural a Miro pueden perder su escala original. Para redimensionar el mapa mental después de pegarlo, puedes estirarlo manualmente en el tablero de Miro.
:::

### formas

Las formas de Mural generalmente se pegan como formas de Miro. Miro admite la mayoría de las formas de Mural directamente.

Sin embargo, Mural incluye 16 formas específicas que no tienen un equivalente directo en Miro. Estas formas se pegarán en Miro como rectángulos.

![Las 16 formas que se copian y pegan de Mural a Miro como rectángulos.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Las 16 formas que se copian y pegan de Mural a Miro como rectángulos*

### Notas adhesivas

Las notas adhesivas de Mural se pegan como notas adhesivas de Miro.

Miro asignará el color y el nivel de opacidad de la nota adhesiva a las coincidencias más cercanas disponibles en Miro.

También pueden aparecer las siguientes diferencias cuando copias y pegas notas adhesivas de Mural a Miro:

- Las notas adhesivas circulares de Mural se pegarán en Miro como notas adhesivas cuadradas.
- Las listas dentro de las notas adhesivas no se conservan como listas interactivas, aunque los elementos individuales aparecerán en líneas separadas dentro de la nota adhesiva de Miro.
- El tamaño de la fuente no se conserva, ya que las notas adhesivas de Miro establecen automáticamente el tamaño de la fuente según el contenido y el tamaño de la nota adhesiva.
- La rotación aplicada a las notas adhesivas en Mural no se conserva al pegar.

![Notas adhesivas copiadas en Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Notas adhesivas copiadas en Mural*

![Notas adhesivas copiadas de Mural a Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Notas adhesivas copiadas y pegadas a Miro*

### tablas

Las tablas de Mural se pegan como tablas de Miro.

Pueden aparecer las siguientes diferencias cuando copias y pegas tablas de Mural a Miro. Para cada uno de estos elementos, normalmente puedes restaurar tus preferencias manualmente en Miro después de pegar:

- Las tablas posicionadas encima de otros objetos en Mural (como áreas, formas o imágenes) pueden quedar parcialmente ocultas detrás de esos objetos cuando se pegan en Miro. Puede que necesites ajustar su capa (traer al frente).
- El color de borde se ignora; los bordes se pegarán en gris.
- La opacidad del fondo se ignora. Las celdas transparentes en Mural se pegarán como celdas blancas en Miro. Sin embargo, el color de fondo en sí (si no es transparente) generalmente se conserva.
- La familia de fuentes de texto se ignora; el texto se pegará utilizando la fuente de tabla predeterminada de Miro (RobertPro).
- El formato de texto en línea, como negritas e itálicas, se ignora dentro de las celdas de la tabla.

![Una tabla con formato mixto copiada en Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Tabla con formato mixto copiada en Mural*

![Tabla con formato mixto copiada y pegada de Mural a Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Tabla con formato mixto copiado y pegado en Miro*

### Texto

Los objetos de texto de Mural se pegan como objetos de texto en Miro. Las familias tipográficas originales de Mural no se conservan. Miro asigna la familia de fuentes de Mural a la fuente más cercana disponible en Miro y ajusta el texto pegado para obtener resultados óptimos en el tablero de Miro.
