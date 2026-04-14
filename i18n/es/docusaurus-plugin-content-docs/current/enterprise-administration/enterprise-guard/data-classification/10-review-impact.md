---
title: Revisar el impacto
article_id: 16494764223378
translation_id: 16494764223378
locale: es
sidebar_position: 10
created_at: '2024-01-19T19:02:16Z'
updated_at: '2025-08-18T09:36:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
id: 10-review-impact
---

Este es el último paso del flujo de configuración de la autoclasificación y las barreras de protección. En este paso del flujo, debes revisar el impacto de las actualizaciones de la clasificación o de la configuración de las barreras de protección. En este paso del flujo, debes revisar el impacto de los cambios que estás realizando en la configuración de la clasificación o de las barreras de protección. Las siguientes secciones describen la información disponible en la página de revisión del impacto y varias acciones que puedes llevar a cabo.

## Distribución de los niveles de clasificación

Esta sección te permite revisar el impacto de tu configuración actualizada en términos de los cambios para cada nivel de clasificación de tableros.

La sección **Distribución de los niveles de clasificación** es plegable, lo que te permite desplazarte por la lista de actualizaciones de forma más eficaz (véase la Figura 1).

![Sección colapsable Distribución de los niveles de clasificación](images/24937148905874_Collapsible_Distribution_of_classification.png)

Figura 1: Sección colapsable Distribución de los niveles de clasificación

La interfaz de usuario basada en columnas simplifica el proceso de comparación y revisión de las actualizaciones de la clasificación de los tableros. Hemos proporcionado columnas distintas que muestran el número de tableros añadidos, el número de tableros eliminados y el total actualizado para cada nivel de clasificación (Figura 2).

![Interfaz de usuario basada en columnas que muestra el número de tableros añadidos, el número de tableros eliminados y el total actualizado para cada nivel de clasificación.](images/24937148908178_columnview.png)

*Figura 2: Interfaz de usuario basada en columnas que muestra el número de tableros añadidos, el número de tableros eliminados y el total actualizado para cada nivel de clasificación.*

La función de desglose ofrece una visión completa (Figura 3) de los siguientes detalles:
- Etiquetas de autoclasificación añadidas o eliminadas.
- Barreras de protección añadidas o eliminadas.
- Número de tableros que cambiaron a un nivel de clasificación específico.
- Número de tableros no afectados por los cambios de configuración que has realizado.

![Función de desglose con una visión completa de las actualizaciones](images/24937158572050_drilldown_feature_classification.png)

*Figura 3: Función de desglose con una visión completa de las actualizaciones*

## Impacto de las barreras de protección

Esta sección muestra las barreras de protección que se aplicarán en función del nivel de clasificación de un tablero, el número total de tableros que tendrán cada barrera de protección específica. El número entre paréntesis indica el número de tableros para los que se añade o suprime la barandilla tras la publicación de la nueva configuración. Además, esta sección también muestra el número de tableros que están sin clasificar (Figura 4).

Para actualizar la configuración de las barreras de protección, haz clic en **Anterior**.
*![Configurar la clasificación Revisar el impacto](images/24937158573202_guardrails.png)
Figura 4: Configurar la clasificación > Revisar el impacto*

## Actualizar la configuración de la autoclasificación

Para realizar actualizaciones después de revisar el impacto de las actualizaciones que has hecho en la configuración de autoclasificación y barreras de protección, haz clic en el botón **Anterior**, realiza las actualizaciones en la configuración y, a continuación, vuelve a revisar el impacto.

## Publicar configuración

Después de revisar el impacto de la clasificación o la configuración de las barreras de protección que has realizado, haz clic en **Publicar**.

:::note
**Notas** :
- La configuración del nivel de clasificación se aplica inmediatamente.
- La configuración de las barreras de protección se aplica inmediatamente.
- Cuando se añaden nuevos tableros con datos sensibles, estos tableros se autoclasifican una vez finalizado el siguiente ciclo de Descubrimiento de Datos.
- Cuando se actualiza el contenido de los tableros (eliminación o adición de contenido sensible), estos tableros se autoclasifican una vez finalizado el siguiente ciclo de Descubrimiento de Datos.
:::
