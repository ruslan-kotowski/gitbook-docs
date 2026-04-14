---
title: Flujos
article_id: 29687970855442
translation_id: 29687970855442
locale: es
sidebar_position: 5
created_at: '2025-09-23T12:18:02Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: template-picker
availability:
  notes: 'Quién puede hacerlo: Miembros del equipo Cuáles planes: Free, Starter, Business,
    Enterprise, Education Cuáles plataformas: Navegador, Escritorio, Móvil'
---

Los flujos te permiten encadenar formatos en el lienzo para crear flujos de trabajo impulsados por IA. Cada formato actúa como entrada para el siguiente, convirtiendo procesos complejos de varios pasos, como la planificación de sprints, escribir informes o aprovechar datos de clientes, en flujos automatizados.

Para saber qué formatos son compatibles con los flujos, consulta Formatos compatibles.

Este artículo explica cómo utilizar los flujos. Para obtener información general sobre los flujos, consulta [descripción general de los flujos](04-flows-overview.md).

:::tip
Obtén plantillas de Flujos prefabricadas en el [seleccionador de plantillas](../../getting-started/start-here/your-first-board/04-templates.md).
:::

## Crear y ejecutar un flujo

El siguiente procedimiento utiliza elementos básicos de UX de Flujos para crear un flujo desde cero. Para asegúrate de que puedas comenzar a crear flujos rápidamente, consulta elementos de UX de Flujos.

Sigue estos pasos:

1. Agrega un Formato compatible o un bloque de Instrucción de IA al lienzo.
2. (Opcional) Conecta cualquier formato o bloque de instrucciones existente al formato que acabas de agregar. Usa los conectores de IA en forma de diamante para conectar tu flujo.
3. Encima del Formato, haz clic en la barra **TASK**.
   La barra **TASK** se expande en un cuadro donde puedes especificar tu instrucción para esa posición en tu flujo.
4. En el cuadro **TASK**, añade tu instrucción. Por ejemplo, en un documento puedes generar un Documento de Requisitos del Producto (PRD). Puedes usar la salida de cualquier Formato o bloque de instrucción de IA conectados.

   > 💡 El cuadro **TASK** te permite seleccionar un modelo de lenguaje extenso (LLM), proveedor de conocimientos, o búsqueda web. En la esquina inferior izquierda, selecciona un modelo de IA, una base de conocimientos o busca en la web. Las opciones varían dependiendo del Formato.
5. (Opcional) Para crear una nueva salida, a la derecha haz clic en el conector de IA con forma de diamante.
   Se abre el menú **Crear nueva salida**.
6. (Opcional) Para crear una nueva entrada, a la izquierda haz clic en el conector de Miro AI en forma de diamante.
   Se abrirá el menú de **Crear nueva entrada**.
7. Para completar tu flujo, repite los pasos 1-6 según sea necesario.
8. Para ejecutar tu flujo, en la barra **TASK** haz clic en **Ejecutar**.
   ![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png)*El menú de contexto **Flujo seleccionado** te muestra cuántos pasos incluye el flujo.*

## Usar Conocimiento con Flujos

El conocimiento se integra con proveedores como Glean, búsqueda en la web y Miro Insights, para recuperar todo lo que tu empresa sabe, usando fuentes internas y externas.

Para cualquier formato en tu flujo, haz clic en la barra de **TAREAS**. La barra de **TAREAS** se expande. En la parte inferior izquierda, selecciona y conecta tu base de conocimiento.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Especifica una base de conocimiento interna para tu flujo*

Puedes convertir datos de tus propios recursos de conocimiento en formatos como documentos, tablas, notas adhesivas y diapositivas. Luego conecta cada formato para usar tus datos como entrada o salida de un flujo.

**Más información:** Consulta [Knowledge](09-knowledge.md).

## Revertir salida en un flujo

Puedes revertir la salida de cualquier formato en tu flujo. Por ejemplo, ejecutas un flujo accidentalmente y sobrescribes un documento.

Para revertir un formato en tu flujo a un estado anterior, haz clic en la **barra de TAREA** del formato. La **barra de TAREA** se expandirá. En la parte inferior derecha, haz clic en el icono de sentido contrario a las agujas del reloj. Selecciona cualquier versión de las últimas 24 horas para restaurar.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *La función de Revertir te permite restaurar cualquier versión de tu formato de las últimas 24 horas.*

## Elementos de UX de los flujos

Comprender los siguientes elementos de UX de los flujos te ayudará a comenzar a crear flujos más rápidamente.

### Conector Miro AI

Formatos admitidos y Bloques de instrucción tienen un conector de Miro AI con forma de diamante a la izquierda que te permite conectar la entrada, y a la derecha que conecta la salida.

Haz clic en el conector de Miro AI en cualquiera de los lados para abrir los menús de **Crear nueva entrada** o **Crear nueva salida**.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png)

*Haz clic en el conector de Miro AI para abrir los menús de entrada y salida.*

:::tip
También puedes arrastrar el conector de Miro AI hacia el contenido existente.
:::

### Resaltado de conector inteligente

Haz clic en cualquier objeto en tu flujo para ver solo esas conexiones resaltadas.

### Ocultar conectores de flujo

Para flujos complejos con muchas conexiones, puedes ocultar todos los conectores de flujo para simplificar tu vista.

En la barra del [tablero](../working-on-the-board/02-miro's-new-simplified-user-interface.md), haz clic en los tres puntos verticales. Luego selecciona **Ver**. Cambia **Mostrar/Ocultar conectores de flujo** a la posición de apagado. Para mostrar todos los conectores de flujo, cámbialo a la posición de encendido.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Mostrar u ocultar todos los conectores de flujo en tu tablero.*

:::note
**Mostrar/Ocultar conectores de flujo** solo afecta tu vista del tablero. Los colaboradores pueden ajustar su propio interruptor.
:::

### Instrucción en el formato

Puedes dar una instrucción a cualquier formato o bloque de instrucciones en tu flujo, lo que garantiza que cada formato en la cadena pueda realizar una tarea especializada de flujo.

Haz clic en la barra de **TAREAS** sobre cualquier formato en tu flujo. La barra de **TAREAS** se expandirá. Añade tu instrucción y describe cómo deseas que el formato lea el contenido de entrada, o cualquier contenido en el tablero, y especifica reglas y salida para el siguiente formato en tu flujo.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *El cuadro de instrucción en formato aparece en la barra de **TAREAS** sobre cada formato en tu flujo.*

### Bloque de instrucciones de IA

Puedes seleccionar un modelo de lenguaje amplio (LLM) o cualquier [proveedor de conocimiento](09-knowledge.md) disponible para ejecutar una instrucción en un bloque independiente, en cualquier parte de tu flujo.

Para un determinado formato, haz clic en el conector de diamante de Miro AI. En el menú de entrada o salida, selecciona **IA** **Instrucción**.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Los Bloques de Instrucción te permiten encadenar instrucciones, aceptar entrada y pasar salida al siguiente formato.*

### Botón de ejecución global

Puedes iniciar tu ejecución desde cualquier formato o bloque de instrucción IA en tu flujo. Haz clic para seleccionar el formato o bloque. El menú de contexto **Flujo seleccionado** aparece junto a la barra de colaboración.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *El menú de contexto de flujo seleccionado*

El menú **Flujo seleccionado** muestra cuántos pasos faltan por ejecutar. Para ejecutar el flujo, haz clic en **Ejecutar**.

## Formatos compatibles

Los flujos son compatibles con los siguientes formatos de Miro.

- Diagramas
- Documentos
- Imágenes
- Insertar código iFrame
- Kanban
- Prototipos
- Diapositivas
- Tablas
- Cronograma
