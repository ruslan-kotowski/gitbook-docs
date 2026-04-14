---
title: Selecciona tu propio modelo (Beta)
article_id: 29484232754578
translation_id: 29484232754578
locale: es
sidebar_position: 10
created_at: '2025-09-15T12:50:30Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ai-sidekicks
availability:
  notes: '¿Quién puede hacerlo?: Miembros del equipo ¿Cuáles planes?: Free, Starter,
    Business, Enterprise ¿Cuáles plataformas?: Navegador, Escritorio, Móvil'
---

Cuando realizas acciones de IA con Miro [flujos](04-flows-overview.md) y compañeros de IA, Selecciona Tu Propio Modelo te permite especificar el modelo de lenguaje grande (LLM) más apropiado para la tarea.

Por ejemplo, para la generación de imágenes puedes decidir si usar Stable Diffusion 3.5 Large o Gemini 2.5 Flash Image (Nano Banana).

Tu elección puede depender de la complejidad o especificidad de tu tarea.

:::tip
Los flujos y compañeros de IA de Miro incluyen un LLM predeterminado preseleccionado para cada tarea. Cuando no estés seguro de qué modelo seleccionar, usar el modelo predeterminado es la mejor opción. El modelo predeterminado se muestra con una etiqueta de Recomendado.
:::

El selector de modelos está disponible solo como parte de flujos y compañeros de IA para lo siguiente:

- Documentos y formatos de imágenes en compañeros de IA y flujos
- Lógica principal de compañeros de IA
- Bloque de instrucciones en flujos

Este artículo explica cómo seleccionar tu propio modelo para flujos y compañeros de IA, y proporciona información para ayudarte a elegir un LLM para tareas comunes.

## Seleccionar tu propio modelo

### Flujos

Los documentos, imágenes y Bloques de Instrucciones en un flujo tienen cada uno una caja de instrucción donde puedes seleccionar tu propio modelo.

Sigue estos pasos:

1. Añade un documento, imagen o Bloque de Instrucción al lienzo.
2. Para acceder a la lista de modelos disponibles, en la esquina superior derecha de la caja de instrucción, haz clic en el nombre del modelo por defecto. Por ejemplo, `AWS | Claude 3.5`.
3. Selecciona un modelo.

Para aprender más sobre cómo crear flujos y la experiencia de usuario de Flujos, consulta [Flujos](05-flows.md).

### Compañeros de IA

Al crear o editar compañeros de IA, verás la sección **Modelo (avanzado)**, y puedes seleccionar qué modelo deseas usar para el procesamiento del compañero de IA, la generación de imágenes y la generación de documentos.

Para obtener más información sobre los compañeros de IA, consulta la [documentación de compañeros de IA](08-ai-sidekicks.md).

## ¿Cómo difieren los modelos

Un modelo de lenguaje grande (LLM) suele ser miembro de una familia de modelos que incluye modelos capaces pero que consumen muchos recursos, modelos óptimos y los modelos más rápidos pero menos capaces.

Por ejemplo, la familia GPT-5 incluye GPT-5, GPT-5-mini y GPT-5-nano.

Los modelos más rápidos pero menos capaces son ideales para menor latencia.

### Con razonamiento y sin razonamiento

Un diferenciador principal entre los LLMs son los modelos de razonamiento frente a los de no razonamiento.

*Razonamiento* significa que el modelo toma más tiempo para proporcionar una respuesta de mayor calidad.

:::note
El *razonamiento* no siempre significa el resultado más preciso. Si requieres muchas iteraciones de salida, un alto razonamiento puede no ser lo más eficiente.
:::

Para tareas complejas, como la creación de documentos orientados al cliente, la priorización, y las tareas que requieren procesar un gran volumen de información, un modelo de razonamiento es la mejor opción.

Para tareas simples, como la revisión gramatical, traducción o reformateo de texto, un modelo de no razonamiento es la opción más eficiente.

La siguiente tabla muestra algunos modelos de razonamiento y de no razonamiento.

| Capacidad de razonamiento | Modelos |
| --- | --- |
| Razonamiento | GPT-5, GPT-5-mini, GPT-5-nano, Claude Sonnet 4, Claude Sonnet 4.5, Gemini 2.5, Gemini 2.5 Flash, o3, o4-mini |
| No razonamiento | GPT 4o, GPT-4o-mini, GPT-4.1, GPT-4.1-mini, Claude Sonnet 3.7, Claude Sonnet 3.5, Gemini 2.5 Flash Lite |

### Estilo

Cada LLM tiene un "estilo" único. A medida que experimentas con diferentes modelos, puedes notar que un estilo de salida particular coincide con tus necesidades, ya sea para la marca, el ambiente o la preferencia.

:::tip
Los modelos más antiguos tienen un estilo más distintivo, especialmente para resultados creativos e innovadores.
:::

## Seleccionar tu modelo de IA por tarea

| Tarea | Modelos | Descripción |
| --- | --- | --- |
| Lluvia de ideas | GPT-4o, o3, o4-mini, Sonnet 3.7 | Ideales para el pensamiento divergente, generación de ideas para funciones, tono lúdico y "toque creativo". Úsalos para generar textos, como titulares alternativos y variantes de microcopias, por ejemplo. |
| Priorización y puntuación | GPT-5, Claude Sonnet 4.5, Gemini 2.5 | Los mejores modelos de razonamiento para puntuaciones consistentes y argumentos claros. Por ejemplo, RICE/MoSCoW en tareas pendientes, evaluaciones de compensaciones y niveles en el roadmap. |
| Síntesis e investigación | GPT-5, GPT-5-mini, Claude Sonnet 4.5, GPT-4.1, Claude Sonnet 3.7, Gemini 2.5 Flash | Úsalo para tareas de complejidad media a alta. Por ejemplo, generar perfiles a partir de notas y obtener conclusiones de bases de datos y conocimiento. |
| Esquema y transformación | GPT-5-mini, GPT-5-nano, GPT-4.1, Sonnet 3.7, Gemini 2.5 Flash, Gemini 2.5 Flash Lite | El cambio de formato generalmente no requiere razonamiento complejo, por lo que las versiones optimizadas ofrecerán resultados más rápidos. Sin embargo, utiliza modelos de familias más recientes para asegurar consistencia cuando trabajes con grandes contextos. notas → documentos, documento → tabla, especificación → diagrama) |
| Ediciones rápidas de texto | GPT-4o-mini, Gemini 2.5 Flash Lite, GPT-5-nano, Claude 3.7 | Opciones más rápidas. Ideales para ediciones de texto simples, como gramática, traducción y reescrituras para mejorar la claridad. |

## Seleccionando modelos para generación de imágenes

Todos los modelos de lenguaje grande (LLM) que Miro soporta pueden procesar texto e imágenes. Sin embargo, la mayoría no puede generar imágenes.

Para la generación de imágenes, Gemini 2.5 Flash Image (Nano Banana) es excepcionalmente hábil para convertir tus instrucciones generales en una imagen.

La mayoría de los LLM esperan una descripción de imagen y no instrucciones específicas. Por ejemplo, "una pintura de un perro con un sombrero divertido" como descripción, versus "crear una imagen divertida de un perro" como instrucción. Nano Banana puede generar imágenes basadas en instrucciones específicas.

:::note
Usa Nano Banana para ediciones específicas en una imagen existente. Otros modelos pueden usar una imagen existente como referencia de estilo.
:::

En cuanto a velocidad o calidad de salida, hay poca diferencia entre los LLM. Como con cada caso de uso, puedes experimentar con diferentes modelos para encontrar el que mejor se adapte a tus preferencias.
