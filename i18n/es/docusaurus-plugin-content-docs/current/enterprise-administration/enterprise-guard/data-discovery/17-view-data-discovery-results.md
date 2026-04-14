---
title: Ver los resultados del descubrimiento de datos
article_id: 15794382139154
translation_id: 15794382139154
locale: es
sidebar_position: 16
created_at: '2023-12-15T15:47:29Z'
updated_at: '2025-11-25T15:40:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

El ciclo de Descubrimiento de Datos se ejecuta al menos una vez cada hora y escanea todas las actualizaciones de los tableros en busca de información relacionada con la privacidad. Esto incluye tableros que ya fueron escaneados en el ciclo anterior de descubrimiento de datos.

:::note
Para ver los resultados del descubrimiento de datos, debes tener el [rol de admin de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de contenido sensible, ponte en contacto con el admin de empresa.
:::

*![privacidad_relacionada_dd.png](images/24937502955410_privacy_related_dd.png)
Figura 1: Resultados del descubrimiento de datos*

Aunque trabajamos continuamente con nuestro socio tecnológico y nuestros clientes para mejorar el sistema de detección de contenido sensible, no podemos garantizar que encuentre y marque el 100% de los datos sensibles de tus tableros. Nuestro sistema de detección de contenido sensible utiliza patrones y otros criterios para determinar la probabilidad de una coincidencia. Puede haber ocasiones en las que el sistema marque incorrectamente los datos de tus tableros como probablemente sensibles (un falso positivo) o no marque los datos como sensibles (un falso negativo). Varios factores contribuyen a que esto ocurra, como la proximidad de términos relacionados o el formato de los datos sensibles.

Para más información sobre cómo puedes suprimir las coincidencias de falsos positivos, consulta [Suprimir una coincidencia de contenido sensible](11-suppress-a-sensitive-content-match.md).

## Ver información sobre la última exploración de descubrimiento de datos completada

La sección **Resultados** del descubrimiento de datos muestra cuándo se completó el último escaneado de descubrimiento de datos, representado en un formato de fecha Mes Día, Año, y una Hora:Minuto AM/PM, con un formato de hora de especificación de zona horaria (GMT+offset). Por ejemplo, 14 de diciembre de 2023, 22:15 h GMT+1 (Figura 1) .

## Ver los resultados del descubrimiento de datos

La sección **Resultados del** descubrimiento de datos muestra información, como el nombre de la normativa, una breve descripción, la etiqueta asociada y el recuento de tableros con contenido potencialmente sensible que podrían estar dentro del alcance de la normativa (Figura 1).

Para explorar los tableros con datos altamente sensibles, haz clic en el enlace Recuento de tableros. Aparece el explorador de contenido con la lista de tableros. Para más información, consulta [Revisar tableros con datos sensibles](16-review-boards-with-privacy-related-information.md).
