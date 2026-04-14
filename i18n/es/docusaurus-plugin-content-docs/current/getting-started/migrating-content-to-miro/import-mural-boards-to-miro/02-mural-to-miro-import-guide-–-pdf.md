---
title: Guía de importación de Mural a Miro – PDF
article_id: 22856050009362
translation_id: 22856050009362
locale: es
sidebar_position: 2
created_at: '2024-11-25T14:36:20Z'
updated_at: '2026-01-19T14:43:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Usuarios: Usuarios con acceso de edición Planes: Business, Education, Enterprise,
    Starter Plataformas: Navegador, Escritorio'
---

Puedes importar tus tableros de Mural existentes en Miro exportándolos de Mural como archivos PDF y luego importando esos PDFs en Miro. Este artículo proporciona orientación para lograr los mejores resultados con las importaciones de PDF, explica el procedimiento de importación y describe qué puedes esperar cuando se importan varios elementos de Mural a Miro utilizando este método.

El método de importación de PDF es particularmente efectivo para contenido que puede no transferirse bien a través de copiado-pegado o importaciones basadas en API. El importador de PDF de Miro analiza las formas y sus coordenadas dentro del PDF de Mural e intenta reconstruir el diseño original. Por ejemplo, puede interpretar líneas que se cruzan como una estructura de tabla.

Ten en cuenta que algunos objetos pueden aparecer de manera diferente en Miro después de la importación, y el estilo o diseño preciso puede requerir ajustes o recreación manual en Miro. En general, el contenido más simple con un estilo menos complejo tiende a ofrecer resultados de importación más precisos.

## Directrices para importar desde Mural

Para lograr los mejores resultados al importar contenido de Mural como PDFs, es útil entender cómo funciona el importador y qué contenido se transfiere más eficazmente. El importador de PDF empareja principalmente formas básicas y líneas.

:::note
**Nota:** Para importar contenido a Miro, tu contenido de Mural debe estar bajo una licencia gratuita limitada o completa en Mural.
:::

El espacio claro entre elementos en tu Mural permite al importador de Miro analizar el contenido con mayor precisión. Un tablero de Mural con muchos elementos muy juntos puede producir resultados de importación mixtos o menos precisos.

Para lograr la importación con la mayor fidelidad posible, asegúrate de que tu contenido de Mural **no** contenga los siguientes atributos, ya que pueden no transferirse bien vía PDF:

- Fuentes personalizadas
- Estilos complejos que transforman formas básicas (por ejemplo, esquinas muy redondeadas en rectángulos, flechas con curvas únicas)
- Numerosas formas y líneas superpuestas
- Elementos rotados

:::tip
**Consejo:** Si necesitas preservar estilos exactos, diseños complejos o coordenadas precisas de tu contenido de Mural, el método más fiable es exportar el contenido de Mural como una imagen estática (por ejemplo, PNG, JPG) y luego importar esa imagen en tu tablero de Miro.
:::

## Importar tableros de Mural a Miro como PDFs

Esta sección explica cómo importar tu contenido de Mural en Miro utilizando la función de importación de PDFs.

### Requisitos previos para la importación de PDFs

Antes de comenzar el proceso de importación, asegúrate de cumplir con los siguientes requisitos previos:

- Debes tener acceso de edición al tablero fuente en Mural (para exportarlo como un PDF).
- Debes tener acceso de edición al tablero de destino en Miro donde pretendes importar el contenido.
- Necesitas haber descargado previamente tus tableros de Mural como archivos PDF.

**Más información:** Para obtener instrucciones sobre cómo exportar desde Mural, consulta la documentación de Mural sobre [cómo exportar y descargar el contenido de tu mural](https://support.mural.co/s/article/export-and-download-your-mural-s-content) (enlace externo).

### Importa el PDF

Sigue estos pasos para importar tus archivos PDF de Mural a Miro:

1. Desde tu panel de Miro, haz clic en el botón **+ Crear nuevo**.
2. En el menú desplegable, selecciona **Importar** y luego elige **Importar desde Mural**.
   Se abrirá el cuadro de diálogo modal **Importar tableros desde Mural**.
3. Sigue las instrucciones en pantalla dentro del modal. Se te pedirá que cargues tus archivos PDF de Mural.
   Opcionalmente, puedes elegir agregar tu contenido importado a un Espacio específico de Miro. Si no especificas un Espacio, el contenido importado se agregará a tu área principal del equipo.
4. Una vez que hayas cargado tus archivos y configurado las opciones, selecciona **Importar tableros**.
   El proceso de importación comenzará. Recibirás una notificación por correo electrónico de Miro cuando la importación se haya completado.

Ahora has importado exitosamente tu contenido de Mural en Miro a través de PDF.

## Resultados esperados

Cuando los objetos de Mural se importan a Miro a través de PDF, se esperan algunas variaciones en el estilo y formato debido a las diferencias entre las plataformas y la naturaleza de la conversión a PDF. Esta sección describe los resultados típicos de importación para objetos comunes de Mural y ofrece algunas mejores prácticas.

### Áreas

El área más externa en tu exportación de Mural generalmente se importará como un marco en Miro. Otras áreas interiores suelen importarse como formas regulares en Miro.

:::note
**Nota:** Las áreas anidadas (áreas dentro de otras áreas) a veces pueden ser identificadas o estructuradas incorrectamente durante la importación. El importador de PDF se basa en las coordenadas visuales para determinar las relaciones padre-hijo de los widgets, lo que puede ser ambiguo con anidaciones complejas.
:::

### Conectores

El importador de PDF reconoce y recrea principalmente conectores de línea continua. Los conectores de línea punteada o discontinua pueden no importarse como se espera.

Si un conector en Mural incluye texto insertado directamente en la línea, el importador de PDF puede interpretarlo como dos líneas separadas con el objeto de texto cerca, en lugar de un solo conector con texto.

![A connector with text that the PDF importer breaks into two lines.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Un conector con texto que el importador de PDF "divide" en dos líneas.*

### Dibujos

Los elementos dibujados a mano de Mural generalmente se importan como una colección de líneas o curvas en Miro.

Para los dibujos complejos, el importador de PDF a veces puede vincular incorrectamente partes del dibujo a objetos cercanos o superpuestos, interpretándolos como conectores donde no estaban previstos.

![A drawing may import as linked to a nearby or overlapping object.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Un dibujo puede importarse como vinculado a un objeto cercano o superpuesto.*

### GIFs

El importador de PDF reconocerá los GIFs de Mural pero los importará como imágenes estáticas (típicamente el primer cuadro del GIF).

:::note
**Nota:** El formato de archivo PDF en sí no soporta GIFs animados. Esta es una limitación del PDF, no del importador de Miro.
:::

### Imágenes

Las imágenes de tu tablero de Mural se importarán como imágenes en Miro. Sin embargo, su posición exacta en el tablero podría cambiar ligeramente debido a las diferencias en los sistemas de coordenadas entre Mural y Miro, y el proceso de conversión a PDF.

### Listas

Las listas (tanto numeradas como con viñetas) de Mural generalmente se importan como listas en Miro. Para obtener mejores resultados, asegúrate de que tus listas en Mural usen marcadores predeterminados (números estándar para listas ordenadas y viñetas básicas para listas no ordenadas).

![A numbered list, and a bulleted list, with default markers, numerals and bullets respectively.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Una lista numerada y una lista con viñetas, con marcadores predeterminados, números y viñetas respectivamente.*

### Mapas mentales

El método de importación PDF funciona mejor para mapas mentales de Mural que tienen un solo nodo raíz y bordes visibles en todos los nodos. Los mapas mentales complejos con múltiples raíces o bordes ocultos pueden no importarse con precisión.

![A basic Mind map is easier to import as PDF.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Un mapa mental básico es más fácil de importar como PDF*

El importador de PDFs puede tener dificultades para interpretar con precisión los mapas mentales debido a que a menudo contienen muchas líneas y objetos en proximidad cercana. Si tu mapa mental en PDF se importa de manera deficiente, considera intentar copiar y pegar el contenido del mapa mental directamente de Mural a Miro. Aunque el método de copiar y pegar puede requerir ajustes manuales de estilo y escala en Miro, la fidelidad estructural general podría ser mayor para algunos mapas mentales.

### Formas

El importador de PDFs está diseñado para importar formas básicas de Mural (por ejemplo, rectángulos, óvalos, triángulos) como formas editables en Miro.

![Only basic shapes import as editable content.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Solo las formas básicas se importan como contenido editable*

Las formas avanzadas, personalizadas o con mucho estilo de Mural, así como las formas rotadas, pueden importarse como imágenes estáticas en lugar de como formas editables de Miro.

### Notas adhesivas

Las notas adhesivas estándar de Mural generalmente se importan como notas adhesivas de Miro. Para obtener la mayor fidelidad, utiliza notas adhesivas de Mural con relaciones de aspecto predeterminadas (por ejemplo, tamaños comunes de 3x3 o 5x3).

![Sticky notes with the default size can be easily imported.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Las notas adhesivas con el tamaño predeterminado pueden importarse fácilmente*

:::note
**Nota:** Las notas adhesivas redondas de Mural se importarán como formas regulares en Miro, ya que Miro no tiene un objeto nativo de nota adhesiva redonda.
:::

Las notas adhesivas superpuestas o rotadas pueden no importarse con alta fidelidad y podrían requerir un reajuste o reposicionamiento manual en Miro.

![Import results vary for rotated sticky notes, and sticky notes that overlap.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Los resultados de la importación varían para las notas adhesivas rotadas y para las que se superponen.*

### Tablas

Las tablas simples de Mural con líneas de cuadrícula claras generalmente se importan con alta fidelidad como tablas de Miro o como una colección de formas y líneas que forman una estructura de tabla.

Las tablas con geometría compleja pueden importarse como una serie de líneas y cuadros de texto desconectados. Para obtener los mejores resultados al importar tablas, asegúrate de que las tablas en tu exportación de Mural **no** tengan los siguientes atributos:

- Celdas combinadas
- Bordes invisibles u ocultos
- Esquinas redondeadas en las celdas o en el borde de la tabla

![Complex tables do not import with high fidelity.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Las tablas complejas no se importan con alta fidelidad.*

### Texto

Los objetos de texto de Mural generalmente se importan como texto editable en Miro, a menudo dentro de un solo bloque de texto o forma que corresponde al cuadro de texto original de Mural.

Para importar texto de la manera más fiel posible, utiliza fuentes predeterminadas y márgenes estándar en Mural.

:::note
**Nota:** El tamaño de la fuente puede variar después de la importación, y puede que necesites ajustarlo manualmente en Miro.
:::

El importador de PDF puede separar el texto que usa fuentes personalizadas o tiene un estilo complejo (por ejemplo, varios estilos dentro de un solo cuadro de texto) en varios bloques de texto más pequeños.
