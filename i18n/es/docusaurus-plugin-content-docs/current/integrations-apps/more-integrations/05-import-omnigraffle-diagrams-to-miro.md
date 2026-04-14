---
title: Importar diagramas de OmniGraffle a Miro
article_id: 33541520646674
translation_id: 33541520646674
locale: es
sidebar_position: 11
created_at: '2026-02-23T15:00:35Z'
updated_at: '2026-02-26T09:55:26Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: diagramming
---

Importa fácilmente tus diagramas desde OmniGraffle a Miro y comienza a colaborar en una herramienta unificada. Dado que OmniGraffle y Miro utilizan diferentes modelos de objetos y sistemas de estilo, es posible que los tableros importados no se vean exactamente como los archivos originales. Puede que necesites revisar y ajustar el formato después de importarlos. Para más información, consulta las secciones [Entender el mapeo de objetos OmniGraffle en Miro](#h_omni_mapping) y [Limitaciones conocidas](#h_omni_known_limitations).

## Antes de comenzar

- Asegúrate de poder crear tableros en Miro.
- Usa OmniGraffle 7.25.1 (septiembre 2025) o posterior. Para verificar tu versión, ve a **OmniGraffle > Acerca de OmniGraffle**.
- Revisa el contenido oculto y las capas antes de la importación. Los elementos ocultos y en capas también se importan y aparecerán en el tablero. Si los elementos se superponen, reorganicenlos después de la importación.
- Convierte los rellenos degradados a colores sólidos antes de exportar. Los degradados no son compatibles.

## Importar un archivo de OmniGraffle a un tablero de Miro

1. Abre OmniGraffle, exporta el diagrama en el formato **.graffle Single File (Zipped)** y guarda el archivo en tu dispositivo.

   **Nota:** Solo admitimos el formato **Single File (Zipped)**. Los formatos **Package** y **Legacy** no son compatibles. Si tienes un archivo exportado no compatible guardado anteriormente, puedes abrir el archivo en OmniGraffle y luego exportarlo en el formato **.graffle Single File (Zipped)**.
2. Abre el tablero de Miro en el que quieras agregar el diagrama.
3. Arrastra y suelta el archivo en formato **.graffle Single File (Zipped)** en el tablero de Miro.

## Importación masiva de múltiples archivos de OmniGraffle al panel de Miro

1. Abre tu panel de Miro.
2. Haz clic en **+ Crear nuevo** en la esquina superior derecha.
3. Haz clic en **Importar** > **Importar desde OmniGraffle**.
4. En el cuadro de diálogo de importación, bajo **Importar a**, selecciona el espacio donde desees crear los tableros de Miro para tus archivos importados de OmniGraffle.
5. Suelta tus archivos **.graffle** en el área de carga, o haz clic en **explorar** para seleccionar archivos de tu computadora.

   **Nota:** Solo admitimos el formato **Archivo único (Zipped)**. Los formatos **Paquete** y **Legacy** no son compatibles. Si tienes un archivo exportado no compatible guardado anteriormente, puedes abrirlo en OmniGraffle y luego exportar al formato **.graffle Archivo único (Zipped)**.
6. Haz clic en **Importar [X] archivos**, donde **[X]** es el número real de archivos que estás importando.
7. Cuando veas el mensaje **Estamos importando tus tableros**, haz clic en **Volver al panel**.

### Después de iniciar la importación

- La importación se ejecuta en segundo plano.
- Los nuevos tableros aparecen en el espacio que seleccionaste durante el proceso de importación una vez que finaliza el procesamiento.
- Recibirás una notificación por correo electrónico una vez que se creen los tableros, incluyendo un enlace directo al espacio para que puedas acceder rápidamente.

## Verificar contenido importado

Después de que se complete la importación, verifica lo siguiente:

- Se creó el número esperado de tableros.
- El contenido es legible y está correctamente posicionado.
- Los conectores están correctamente unidos.
- El formato del texto aparece como se espera.
- Las secciones visuales clave están intactas.

Para diagramas que evolucionarán con el tiempo, considera reconstruir áreas muy complejas usando objetos nativos de Miro para una mejor capacidad de edición a largo plazo.

## Preguntas frecuentes (FAQ)

¿Puedo importar múltiples archivos a la vez?

Sí. Puedes importar múltiples archivos en formato **.graffle Single File (Zipped)** a la vez. Para más información, consulta [Importación masiva de múltiples archivos de OmniGraffle al panel de Miro](#h_omni_bulk_import).

¿Dónde están los tableros de mi importación masiva?

Los tableros de tu importación masiva se crean en el espacio que seleccionaste durante el [proceso de importación](#h_omni_bulk_import). También puedes hacer clic en el enlace del correo electrónico que recibiste cuando se crearon los tableros para acceder rápidamente a ellos. Por último, si no especificaste el espacio durante el proceso de importación y no tienes el correo electrónico a mano, puedes buscar tus tableros en el espacio **Archivos importados**.

¿Mi diagrama se verá exactamente igual después de la importación?

La mayoría de las veces sí, pero no siempre. Las fuentes, los conectores y el formato complejo pueden cambiar durante la importación. Para más información, consulta las secciones [Limitaciones conocidas](#h_omni_known_limitations) y [Entender el mapeo de objetos de OmniGraffle en Miro](#h_omni_mapping).

¿Cuánto tiempo tarda la importación?

El tiempo de procesamiento depende del tamaño y la complejidad del archivo. Recibirás un correo electrónico una vez que se hayan creado tus tableros, incluyendo un enlace directo al espacio para que puedas acceder rápidamente a los tableros.

¿Cómo sé si mi importación masiva tuvo éxito o falló?

**Si tu importación masiva tuvo éxito**, recibirás una notificación por correo una vez que los tableros estén creados, incluyendo un enlace directo al espacio para que puedas acceder a ellos rápidamente.

**Si tu importación masiva falló**, recibirás un correo informándote sobre los archivos para los cuales hubo errores de importación.

Próximos pasos:

- Contacta a tu admin de Miro o al equipo de soporte de Miro e infórmales sobre este error.
- Si es posible, proporciona una versión **redactada** del archivo de OmniGraffle a tu admin de Miro, ya que esto ayudará a solucionar tu error de importación.

¿Puedo deshacer una importación?

No es posible deshacer una importación. Puedes eliminar los tableros creados, si es necesario.

## Resolución de problemas

No veo la opción de Importar desde OmniGraffle en el menú de Importación

- Confirma que tienes permiso para crear tableros en Miro.
- Borra el caché, actualiza tu navegador y vuelve a intentarlo.
- Contacta a tu admin de empresa para confirmar que la función está habilitada para tu organización.

Mi archivo no se carga

- Asegúrate de exportar el archivo de OmniGraffle en formato **.graffle Single File (Zipped)**.

  **Nota:** Solo admitimos el formato **Single File (Zipped)**. Los formatos **Package** y **Legacy** no son compatibles. Si tienes un archivo exportado no compatible guardado anteriormente, puedes abrir el archivo en OmniGraffle y luego exportar al formato **.graffle Single File (Zipped)**.
- Intenta cargar un solo archivo en lugar de varios archivos a la vez.
- Divide los diagramas más grandes de OmniGraffle en elementos más pequeños.

No recibí un correo

- [Revisa el spam o los buzones filtrados.](../../using-miro/tools/troubleshooting/02-allowlist-miro-mailers.md)
- Revisa el espacio seleccionado para tableros recién creados.

El diseño se ve incorrecto

- Vuelve a aplicar las fuentes si hubo sustituciones.
- Reconecta manualmente los conectores o líneas.
- Edita las secciones críticas utilizando formas nativas de Miro si es necesario.

## Entender el mapeo de objetos de OmniGraffle en Miro

| Función de forma nativa de Miro | Disponible para formas importadas de OmniGraffle |
| --- | --- |
| **Estilizar formas**  Puedes personalizar el aspecto de tus formas usando varias opciones de estilo para adaptarlas a tus necesidades y añadir un toque personal a tus tableros. Selecciona una forma para cambiar su estilo, color y transparencia. Puedes seleccionar varias formas al mismo tiempo y estilizar todas. También puedes estilizar los bordes eligiendo el color, transparencia, grosor, radio de las esquinas redondeadas, y tipo. | Espesor ✅  Opacidad/transparencia ✅  Color ✅  Funciones de selección múltiple (excepto) transparencia ❌  (Se puede establecer transparencia en la selección múltiple)  Color del borde ✅  Transparencia del borde ✅  Espesor del borde ✅  Tipo de borde ✅ (punteado)  Radio de las esquinas redondeadas ❌ |
| **Cambiar tamaño o rotación de la forma**  Usa los nodos blancos para cambiar las dimensiones de una forma. Arrastra el icono de la flecha para rotar la forma. | ✅ |
| **Convertir formas**  Puedes convertir una forma en una tarjeta, cuadro de texto, nota adhesiva o cualquier otra forma. | ❌ |
| **Enviar forma hacia atrás o traer al frente**  Envía la forma atrás o tráela al frente; haz clic en los tres puntos que se encuentran en el menú contextual y elige una opción. O utiliza los atajos **Pg Up** y **Pg Dn** (para Windows)/**fn + ↑** y **fn + ↓** (para Mac). | ✅ |
| **Añadir texto a las formas**  Para añadir texto a una forma, selecciónala y comienza a escribir. Las formas tienen un límite de 6000 símbolos. Siéntete libre de usar distintas opciones de formato de texto: puedes cambiar el tamaño del texto, la fuente, el estilo, la alineación, el color y resaltar el texto.  **Nota:** Las viñetas no son compatibles con las formas. Usa texto en su lugar. | 🟠  No puedes añadir nuevo texto a las formas importadas desde OmniGraffle. Sin embargo, si una forma importada ya contiene texto, puedes editar ese texto como de costumbre (fuente, tamaño, color, alineación y resaltado). |
| **Crea diagramas con rapidez**  Tan pronto como selecciones una forma, una nota adhesiva o una tarjeta y desplaces el cursor sobre un punto azul cerca del objeto, se mostrará dónde se creará la nueva forma o la línea de conexión. Haz clic sobre el punto para crear la línea o el objeto. Si deseas conectar el objeto con uno diferente de los sugeridos, arrastra el punto y dibuja una línea de conexión. | ✅  Replica la misma forma |
| **Dimensiones de los objetos**  Usa dimensiones de los objetos para crear formas del mismo tamaño en tu tablero con precisión. Puedes habilitar dimensiones de los objetos en la configuración de tu tablero. | ✅ |

## Limitaciones conocidas

En esta versión, al importar archivos de OmniGraffle a Miro, puedes notar diferencias en la estructura, el estilo o el comportamiento debido a diferencias entre las dos plataformas.

### Mapeo de formas y geometría

**Limitaciones**

- Las formas de OmniGraffle se importan en Miro como SVG o formas personalizadas, las cuales no admiten la función de cambio de forma de Miro. Si una forma no puede ser reconocida y no existe una geometría de reserva, se convierte por defecto en un rectángulo.

**Soluciones alternativas**

- Reemplaza las formas críticas con formas nativas de Miro después de la importación para restaurar el soporte completo de edición y QDC.
- Intenta usar las bibliotecas integradas de formas y prototipos de Miro con cientos de formas para una variedad de casos de uso.
- Revisa los diagramas complejos después de la importación y ajusta manualmente las formas que se convirtieron en rectángulos.

### Fidelidad visual y estilo

**Limitaciones**

- Los gradientes no son compatibles. Los rellenos de gradiente se aplanan durante la importación.
- Las sombras no son compatibles y se eliminan durante la importación.
- Las fuentes no compatibles se reemplazan por una fuente del sistema.

**Soluciones alternativas**

- Usa colores sólidos en lugar de gradientes antes de exportar.
- Elimina los efectos de sombra en OmniGraffle antes de exportar si la precisión visual es crítica.
- Usa fuentes del sistema ampliamente compatibles para reducir la sustitución de fuentes.
- Revisa la tipografía y el espaciado después de la importación y ajusta los estilos directamente en Miro.

### Conectores y anotaciones

**Limitaciones**

- Las leyendas de las líneas pueden no detectarse o posicionarse correctamente después de la importación.
- Las líneas pueden aparecer divididas, ligeramente desalineadas o pasar a través de las formas.
- Las flechas direccionales dentro de formas agrupadas pueden perderse ocasionalmente durante la conversión.

**Soluciones**

- Reposiciona manualmente las etiquetas de texto en las líneas de conexión después de la importación.
- Reconecta o redirige los conectores de Miro si ocurren problemas de alineación.

### Formatos de archivo

**Limitaciones**

- Solo admitimos el formato **Single File (Zipped)**. Los formatos **Package** y **Legacy** no son compatibles.
- Las exportaciones en PNG se importan como imágenes planas no editables.

**Soluciones alternativas**

- Utiliza el formato de exportación **Single File (Zipped)** para obtener los mejores resultados.
- Si tienes un archivo de exportación no compatible que guardaste anteriormente, puedes abrir el archivo en OmniGraffle y luego exportarlo al formato **.graffle Single File (Zipped)**.
- Evita las exportaciones en PNG si necesitas objetos editables.

### Comportamiento de importación masiva

**Limitaciones**

- Las notificaciones por correo electrónico para las importaciones masivas pueden fallar ocasionalmente debido a rebotes duros.
- Después de completar una importación masiva, es posible que el contenido importado no aparezca inmediatamente en el tablero.

**Soluciones alternativas**

- Verifica las reglas de spam o filtro de correo si no se reciben las notificaciones.
- Refresca tu navegador después de la finalización de la importación masiva.
