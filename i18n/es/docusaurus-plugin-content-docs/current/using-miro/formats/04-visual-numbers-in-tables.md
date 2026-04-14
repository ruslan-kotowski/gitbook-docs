---
title: Números visuales en tablas (BETA)
article_id: 31356870414610
translation_id: 31356870414610
locale: es
sidebar_position: 18
created_at: '2025-11-25T19:40:55Z'
updated_at: '2026-03-13T12:26:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: tables
availability:
  notes: '¿Quién puede hacerlo?: Editores de tableros ¿Qué planes?: Business, Enterprise
    ¿En qué plataformas?: Navegador, Escritorio, Móvil'
---

Visual Numbers permite a los usuarios convertir números en barras de progreso visuales. Los usuarios pueden establecer reglas de formato condicional con colores personalizados y configurar rangos mínimos/máximos para una mejor visualización de datos. Visual Numbers también permite el formato como porcentajes o monedas.

## Formatear números visualmente

El formato visual de números transforma los datos numéricos en barras de progreso, haciendo más fácil detectar tendencias y seguir el progreso de un vistazo. Puedes mostrar los números como porcentajes o monedas, establecer rangos personalizados y aplicar reglas de formato condicional.

Aplica formato visual a un campo numérico:

1. Pasa el cursor sobre un campo de número o fórmula para mostrar el icono de **tres puntos** (**...**).
2. Haz clic en el icono de **tres puntos** (**...**) y selecciona **Editar campo**.
3. En la sección **Visualización** del diálogo, haz clic en **Barra**.
   Los números se mostrarán como barras de progreso.
4. Elige tu formato:
   1. Porcentaje (%): Ideal para tasas de finalización, seguimiento de progreso.
   2. Moneda: Selecciona entre principales monedas ($, €, £, ¥, y más).
5. Establece el rango de **Mín** y **Máx** para tus barras de progreso. Para porcentajes, utiliza típicamente 0-100. Para moneda, establece valores mínimos y máximos apropiados para tus datos.
6. Elige un color de barra del selector de colores.
7. Alterna las etiquetas numéricas entre encendidas o apagadas:
   1. Encendidas: Muestra el valor numérico junto a la barra de progreso.
   2. Apagadas: Muestra solo la barra de progreso para una vista más limpia.
8. Haz clic en **Guardar**.

## Aplica formato condicional

El formato condicional colorea automáticamente tus barras de progreso de acuerdo con reglas que defines, ayudándote a identificar rápidamente los valores que necesitan atención.

1. Abre la **configuración de campo** para un campo numérico o de fórmula.
2. Activa **colores condicionales**.
3. Haz clic en **Agregar regla**.
4. Define tu regla:
   1. Selecciona una condición (es igual a, no es igual a, es mayor que, es menor que, es mayor o igual a, es menor o igual a, está vacío, no está vacío).
   2. Ingresa el valor para comparar (si corresponde).
   3. Elige un color para los valores que coincidan con esta regla.
5. Agrega varias reglas según sea necesario. Arrastra y suelta las reglas para establecer su prioridad. Las reglas en la parte superior tienen prioridad.
6. Haz clic en **Guardar**.

El formato condicional aparece tanto en la vista de tablas como en el panel lateral al ver registros individuales.

El formato visual de números está disponible actualmente solo en la vista de tabla y el panel lateral.

Las vistas de Cronograma, Kanban y Tarjetas mostrarán el formato numérico estándar.
