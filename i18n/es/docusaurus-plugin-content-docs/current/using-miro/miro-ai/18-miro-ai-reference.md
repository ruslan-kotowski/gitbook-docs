---
title: Referencia de Miro AI
article_id: 20970362792210
translation_id: 20970362792210
locale: es
sidebar_position: 18
created_at: '2024-08-26T09:34:26Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: comments
availability:
  notes: 'Quién puede hacerlo: Todos los usuarios Qué planes: Free, Starter, Business,
    Enterprise, Education Qué plataformas: Navegador, Escritorio, Móvil'
---

Este artículo de referencia describe la funcionalidad de Miro AI.

## Modelos de IA de Miro

Los modelos generalmente están alojados en la infraestructura de los proveedores, o en el servicio Microsoft Azure AI o AWS Bedrock. Para los clientes que adquieren Miro a través de AWS Marketplace, todos los modelos están alojados en AWS Bedrock.

### Creación e iteración impulsada por IA

| **Función de Miro AI** | **Descripción** | **Modelo** |
| --- | --- | --- |
| Resúmenes de conversación | Genera un resumen de hilos de comentarios extensos en tu tablero de Miro. | GPT 4o-mini |
| Crear diagrama - Flujograma | Crea un flujograma a partir de una instrucción del usuario y contenido seleccionado del tablero. | GPT-4o |
| Editar diagrama - Diagrama de flujo | Edita un diagrama de flujo a partir de una instrucción del usuario y el contenido del tablero seleccionado. | GPT-4o |
| Crear diagrama - Mapa mental | Crea un mapa mental a partir de una instrucción del usuario y el contenido del tablero seleccionado. | GPT 4o-mini |
| Editar diagrama - Mapa mental | Edita un mapa mental a partir de una instrucción del usuario y el contenido del tablero seleccionado. | GPT-4o |
| Crear diagrama - ERD | Crea un diagrama de relación de entidades (ERD) a partir de una instrucción del usuario. Una opción **Crear con IA** . | GPT 4o-mini |
| Editar diagrama - DER | Edita un DER a partir de una instrucción del usuario y el contenido del tablero seleccionado. | GPT-4o |
| Digitalizar diagrama | Transforma imágenes de diagramas dibujados a mano en diagramas totalmente editables en Miro. | Claude 3.7 Sonnet (AWS Bedrock) |
| Crear documento | Crea un documento de Miro a partir de una instrucción del usuario y el contenido del tablero seleccionado. Una opción de **Crear con IA**. | GPT-4o |
| Editar documento | Edita un documento de Miro a partir de una instrucción del usuario y el contenido del tablero seleccionado. | GPT-4o |
| Crear imagen | Crea una imagen a partir de una instrucción del usuario, incluyendo objetos del tablero para contexto. Una opción de **Crear con IA** . | Segmind Stable Diffusion 1B (SSD-1B) + StabilityAI Diffusion XL Refiner 1.0 |
| Editar imagen | Edita una imagen a partir de una instrucción del usuario, incluyendo objetos del tablero para contexto. Una opción de **Crear con IA**. | GPT-4o |
| Convertir imagen a prototipo | Convierte una imagen de boceto o prototipo en un prototipo editable de Miro. | Modelo patentado de Miro + Claude 3.7 Sonnet |
| Texto alternativo de imagen | Genera texto alternativo para una imagen. No consume créditos de IA. | Modelo propio de Miro |
| Crear notas adhesivas | Crea notas adhesivas a partir de una instrucción de usuario y el contenido del tablero seleccionado. | GPT-4o |
| Editar notas adhesivas | Edita notas adhesivas de Miro a partir de un tablero de usuario y el contenido del tablero seleccionado. | GPT-4o |
| Captura de notas adhesivas | Convierte una imagen de notas adhesivas físicas en notas adhesivas de Miro. | Modelo propio de Miro |
| Crear Prototipo | Crea un Prototipo de Miro a partir de una instrucción del usuario y el contenido del tablero seleccionado. | GPT-4o + Claude 4.5 Sonnet + GPT 4o-mini + Gemini 2.5 Flash Image (nano-banana) |
| Editar pantalla del Prototipo | Edita una pantalla del Prototipo de Miro a partir de una instrucción del usuario y el contenido del tablero seleccionado. | Claude 4.5 Sonnet + Gemini 2.5 Flash Image (nano-banana) |
| Eliminar fondo | Elimina el fondo de una imagen. | Modelo propio de Miro |
| Dibujos inteligentes | Convierte un dibujo a lápiz en una línea, forma o nota adhesiva. | Modelo propio de Miro |
| Crear tabla | Crea una tabla de Miro a partir de una instrucción del usuario y el contenido del tablero seleccionado. | Claude 3.7 Sonnet |
| Editar tabla | Edita una tabla de Miro a partir de una instrucción del usuario y el contenido del tablero seleccionado. | Claude 3.7 Sonnet |

### Compañeros impulsados por IA

|  |  |  |
| --- | --- | --- |
| **Función de Miro AI** | **Descripción** | **Modelo** |
| Compañero de IA - Instructor Agile | Identifica los temas clave en una retrospectiva y sugiere próximos pasos. | GPT-4o |
| Compañeros de IA - Líder de producto | Ofrece comentarios y sugerencias como comentario en marcos, notas adhesivas o texto. También proporciona ideas de solución como notas adhesivas. | GPT-4o |
| Compañeros de IA - Alianza de marketing de producto | Ofrece comentarios y sugerencias como comentario en marcos, notas adhesivas o texto. | GPT-4o |

### Agrupación impulsada por IA

| **Función de Miro AI** | **Descripción** | **Modelo** |
| --- | --- | --- |
| Agrupación de notas adhesivas por palabras clave | Agrupa notas adhesivas por palabras clave, asignando un título a cada grupo. | Claude 3.5 Haiku + Amazon Nova Micro |
| Agrupación de notas adhesivas por sentimiento | Agrupa notas adhesivas por sentimiento, como opiniones y puntos de vista, en grupos positivos, neutrales y negativos. | Claude 3.5 Haiku |

### Edición de texto impulsada por IA

La siguiente tabla muestra la edición de texto impulsada por Miro AI:

|  |  |  |
| --- | --- | --- |
| **Función de Miro AI** | **Descripción** | **Modelo** |
| Cambiar tono | Modifica el tono del texto seleccionado para transmitir un estilo amigable, profesional, empresarial o divertido. | GPT-5 nano |
| Corregir gramática y ortografía | Corrige la ortografía y la gramática del texto seleccionado. | GPT-5 |
| Reescribir para mayor claridad | Vuelve a escribir el texto seleccionado para mayor claridad. | GPT-5 Chat |
| Acortar texto | Reformula el texto seleccionado en una versión más corta sin perder claridad ni legibilidad. | GPT-5 mini |
| Traducir | Traduce el texto seleccionado a inglés, español, alemán, francés, japonés, portugués, coreano, polaco, italiano, turco, árabe, ruso, danés, finlandés, noruego, neerlandés, sueco o tailandés. Puedes traducir uno o varios objetos simultáneamente. | GPT-5 mini |

### Mapas mentales impulsados por IA

| **Función de Miro AI** | **Descripción** | **Modelo** |
| --- | --- | --- |
| Generar mapa mental | Genera un mapa mental a partir de un nodo raíz seleccionado. | GPT 4o-mini |
| Mapa mental - Ampliar con ideas | Genera ideas a partir de un nodo raíz o un nodo hijo seleccionado. | GPT 4o-mini |
| Mapa mental - Expandir con temas | Genera temas a partir de un nodo raíz o nodo hijo seleccionado. | GPT 4o-mini |
| Mapa mental - Expandir con preguntas | Genera una pregunta a partir de un nodo raíz o nodo hijo seleccionado. | GPT 4o-mini |

### Diapositivas impulsadas por IA

Miro Diapositivas usa los siguientes modelos:

- Amazon Titan
- Claude 4 Sonnet
- Claude 3.7 Sonnet
- Claude 3.5 Sonnet
- GPT-5
- GPT-4o
- Stable Diffusion 3.5 Large
- Stability Image Core

### Miro Insights

Para sintetizar opiniones de clientes, [Miro Insights](https://help.miro.com/hc/articles/25438311770770) usa GPT-4o.

### Clientes de AWS Marketplace

**Modelos de AWS Marketplace**

| **Función de Miro AI** | **Modelo** |
| --- | --- |
| Resúmenes de conversación | Claude Haiku 3.7 (AWS Bedrock) |
| Crear diagrama – Diagrama de flujo | Claude Sonnet 3.7 (AWS Bedrock) |
| Editar diagrama – Diagrama de flujo | Claude Sonnet 3.7 (AWS Bedrock) |
| Crear diagrama – Mapa mental | Claude Sonnet 3.7 (AWS Bedrock) |
| Editar diagrama – Mapa mental | Claude Sonnet 3.7 (AWS Bedrock) |
| Crear diagrama – DER | Claude Sonnet 3.7 (AWS Bedrock) |
| Editar diagrama – ERD | Claude Sonnet 3.7 (AWS Bedrock) |
| Crear documento | Claude Sonnet 3.7 (AWS Bedrock) |
| Editar documento | Claude Sonnet 3.7 (AWS Bedrock) |
| Crear notas adhesivas | Claude Sonnet 3.7 (AWS Bedrock) |
| Editar notas adhesivas | Claude Sonnet 3.7 (AWS Bedrock) |
| Captura de notas adhesivas | Claude Sonnet 3.7 (AWS Bedrock) + modelo propietario de Miro |
| Crear imagen | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| Editar imagen | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| Texto alternativo de la imagen | Claude Sonnet 3.7 (AWS Bedrock) |
| Crear prototipo | Claude Sonnet 3.7 (AWS Bedrock) + Núcleo de Imagen de Estabilidad de Bedrock |
| Editar pantalla de prototipo | Claude Sonnet 3.7 (AWS Bedrock) + Núcleo de Imagen de Estabilidad de Bedrock |
| Convertir imagen en prototipo | Claude Sonnet 3.7 + modelo propietario de Miro |
| Crear tabla | Claude Sonnet 3.7 (AWS Bedrock) |
| Editar tabla | Claude Sonnet 3.7 (AWS Bedrock) |
| Digitalizar diagrama | Claude Sonnet 3.7 (AWS Bedrock) |
| Agrupación de notas adhesivas por palabras clave | Claude Sonnet 3.7 (AWS Bedrock) + modelo propio de Miro |
| Agrupación de notas adhesivas por sentimiento | Modelo propio de Miro |
| Compañeros de IA | Claude Sonnet 3.7 (AWS Bedrock) |
| Edición de texto impulsada por IA | Claude Sonnet 3.7 (AWS Bedrock) |
| Mapas mentales impulsados por IA | Claude Sonnet 3.7 (AWS Bedrock) |

## Selecciona tu propio modelo

Las siguientes listas muestran qué modelos están disponibles con [Selecciona tu propio modelo](10-select-your-own-model-beta.md), disponible para [flujos](04-flows-overview.md) y compañeros de IA.

### Modelos de lenguaje grande

**Claude**

- Claude 3.7 Sonnet
- Claude Sonnet 4

**OpenAI**

- GPT-4o
- GPT-4o mini
- OpenAI o4-mini
- GPT-5
- GPT-5 mini
- GPT-4.1
- GPT-4.1 mini

### Modelos de imagen

**Stability AI**

- Stable Image Core
- Stable Image Ultra
- Stable Diffusion 3.5 Large

**Amazon**

- Generador de Imágenes Amazon Titan
- Lienzo Amazon Nova

**Google**

- Gemini 2.5 Flash Image (Nano Banana)
- Vertex AI Imagegen 3
- Vertex AI Imagegen 3 Rápido
- Vertex AI Imagegen 4

## Créditos de IA y complemento de Miro

Miro asigna un número determinado de créditos de IA a tu cuenta cada mes. La cantidad de créditos asignados depende de tu plan. Tu asignación se restablece el primer día de cada mes calendario.

Por cada acción de IA que realices, consumes créditos de IA. La mayoría de las acciones de IA consumen un (1) crédito por acción, sin embargo, algunas funciones pueden consumir más.

Para aumentar tu asignación de créditos de IA, puedes optar por comprar una suscripción adicional de créditos de Miro AI. Para más información, consulta [Créditos de Miro AI y complemento de IA](../../plans-billing/billing-and-payments/03-miro-ai-credits.md).

## Privacidad y seguridad de Miro AI

A partir del 3 de febrero de 2025, Miro recopilará datos de interacción de IA de usuarios del plan Free para mejorar funciones de Miro AI como resúmenes inteligentes, diagramas y compañeros de IA.

Para saber más sobre cómo Miro utiliza las interacciones de IA para mejorar Miro AI, y cómo puedes controlar tus preferencias de datos, consulta [Mejoras de calidad de Miro AI](19-miro-ai-quality-improvements.md).
