---
title: Verificador de accesibilidad de Miro
article_id: 19479150111378
translation_id: 19479150111378
locale: es
sidebar_position: 3
created_at: '2024-06-11T13:49:03Z'
updated_at: '2025-07-30T17:01:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: accessibility
---

Garantizar la accesibilidad para todos es una parte central de la misión de Miro. Miro ha desarrollado herramientas para ayudarte a crear experiencias en las que todos puedan participar. El Verificador de accesibilidad de Miro está diseñado para ayudarte a asegurar que tus tableros de Miro sean tan inclusivos y accesibles como sea posible.

## ¿Qué es el Verificador de accesibilidad de Miro?

El Verificador de accesibilidad de Miro es una herramienta innovadora diseñada para empoderar a todos los usuarios a colaborar eficazmente, sin las limitaciones impuestas por las barreras de accesibilidad. Realiza una variedad de verificaciones en tus tableros de Miro para identificar áreas que pueden no cumplir con los estándares de accesibilidad, proporcionándote insights prácticos sobre cómo mejorar tu contenido para todos los usuarios.

## ¿Por qué usar el Verificador de accesibilidad de Miro?

Crear una experiencia accesible no se trata solo de cumplimiento. El Verificador de accesibilidad de Miro te guía para crear contenido más inclusivo, asegurando que cada participante, independientemente de sus necesidades de acceso, tenga una experiencia fluida y atractiva.

## Para usar el Verificador de accesibilidad de Miro:

1. Navega hasta el menú **tres puntos verticales** (![icon-main.svg](../../../../../../../docs/getting-started/start-here/your-first-board/images/28438530164626_icon-main.svg)) > **Accesibilidad** > **Verificador de accesibilidad**.![new-accessibility-checker.png](../../../../../../../docs/getting-started/start-here/your-first-board/images/28438515675410_new-accessibility-checker.png)
   *El Verificador de accesibilidad se encuentra en el menú principal de la barra de herramientas del tablero > Accesibilidad > Verificador de accesibilidad*
2. El Verificador de accesibilidad de Miro escaneará automáticamente tu tablero en busca de posibles incidencias de accesibilidad. Esto incluye verificaciones de contraste de color, descripciones de imágenes y títulos de marcos, asegurando que tu contenido sea perceptible para todos.
3. Una vez que se complete el escaneo, el verificador presentará un informe detallado de sus hallazgos. Este informe incluye recomendaciones específicas sobre cómo abordar cualquier incidencia identificada. El informe dividirá las incidencias en dos categorías: Descripciones y contraste de color.
   ![Accessibility checker shows 4 accessibility issues found on the board](../../../../../../../docs/getting-started/start-here/your-first-board/images/19479175122578_f4530230-4f9f-4155-b801-1554c1393a56.png)*El Verificador de accesibilidad muestra que se encontraron 4 incidencias de accesibilidad en el tablero*
4. Sigue las recomendaciones del verificador para modificar tu tablero. Esto podría implicar ajustar colores o añadir descripciones a los objetos.
5. Activar en una incidencia seleccionada te llevará a esa incidencia en el tablero, facilitando realizar un cambio.
   ![Un objeto de texto con contraste insuficiente está seleccionado en el tablero](../../../../../../../docs/getting-started/start-here/your-first-board/images/19479175123346_8f32a246-8d3d-4558-8a3d-d5adf1167df7.png)
   *Un objeto de texto con contraste insuficiente está seleccionado en el tablero*
6. Después de realizar los ajustes sugeridos, puedes ejecutar el verificador nuevamente para asegurarte de que todas las incidencias han sido resueltas.![Accessibility checker shows no issues](../../../../../../../docs/getting-started/start-here/your-first-board/images/19479175124114_4522a346-c8de-44a5-b79f-60f8ce5cc9cc.png)
   *El verificador de accesibilidad no muestra incidencias*

## Verificaciones de accesibilidad

Actualmente, se admiten cuatro verificaciones de accesibilidad en un tablero de Miro.

### Contraste de color

El contraste de color se define como la diferencia en luminosidad o brillo entre dos colores. Si la proporción es demasiado baja, puede ser difícil o imposible distinguir entre los dos colores. Esto puede dificultar que algunos usuarios perciban texto o formas en un tablero de Miro. La orientación actual de W3C WCAG 2.2 AA es la siguiente:

- El texto debe tener al menos un contraste de 4,5:1 contra el fondo![Text with insufficient contrast saying Future is accessible and marked Fail, same text with sufficient contrast marked Pass](../../../../../../../docs/getting-started/start-here/your-first-board/images/19479175125522_ff02eeb3-c357-41b9-8c15-f8e17f7affa5.png)
  *Texto con contraste insuficiente que dice “El futuro es accesible” y está marcado como “Fallo”, el mismo texto con suficiente contraste marcado como “Aprobado”*
- Los elementos gráficos deben tener al menos una relación de contraste de 3:1 contra el fondo![An arrow with insufficient contrast marked Fail, same arrow with sufficient contrast marked Pass](../../../../../../../docs/getting-started/start-here/your-first-board/images/19479175127314_88063df8-8a9d-4191-ac09-6e18f6cb9e74.png)
  *Una flecha con contraste insuficiente marcada como “Falló”, la misma flecha con suficiente contraste marcada como “Aprobada”*

### Descripciones de imágenes

- Las descripciones de las imágenes proporcionan a las tecnologías de accesibilidad, como los lectores de pantalla y el control por voz, información que se puede comunicar a los usuarios.

![Diálogo de descripción de imagen. Selecciona una imagen en el tablero, presiona Ctrl+Intro para mover el foco al menú contextual, presiona la flecha derecha hasta llegar al botón de Descripción](../../../../../../../docs/getting-started/start-here/your-first-board/images/19479175127954_618517d6-3d09-40f9-a9a1-40542fb9181c.png)
*Diálogo de descripción de la imagen. Selecciona una imagen en el tablero, pulsa Ctrl+Intro para mover el foco al menú contextual, presiona la flecha derecha hasta llegar al botón de Descripción*

### Títulos de marcos

- Proporcionar títulos de los marcos facilita que los usuarios naveguen por un tablero de Miro.

![Marco sin nombre marcado como Fallo, mismo marco etiquetado como Intro marcado como Aprobado](../../../../../../../docs/getting-started/start-here/your-first-board/images/19479175129106_89f69207-a0ac-4bfd-b3ee-1255b23e6c1d.png)

*Marco sin nombre marcado “Fallido”, el mismo marco etiquetado “Intro” marcado “Aprobado”*

## Categorización de incidencias

Las incidencias en el Verificador de accesibilidad de Miro se clasifican en dos niveles distintos de importancia:

- Crítico: Incidencias que tendrán un impacto bloqueante en el tablero, haciendo imposible que algunos usuarios lo utilicen eficazmente.
- Grave Incidencias que pueden tener un impacto negativo en la experiencia de usuario para los usuarios que utilizan tecnologías de accesibilidad.

Ten en cuenta que el uso del Verificador de accesibilidad de Miro no detectará todas las incidencias de accesibilidad, y podría ser necesario realizar algunos pasos adicionales para que tu tablero de Miro sea accesible para todos. Para obtener más información, consulta la guía sobre cómo crear experiencias Miro accesibles e inclusivas.

## Objetos compatibles

- notas adhesivas
- Texto
- forma
- líneas de lápiz
- Líneas de conexión
