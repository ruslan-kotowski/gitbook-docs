---
title: Vista general del panel de descubrimiento de datos
article_id: 26806897106834
translation_id: 26806897106834
locale: es
sidebar_position: 1
created_at: '2025-05-19T11:10:19Z'
updated_at: '2025-11-25T15:51:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

El panel de descubrimiento de datos ofrece una vista centralizada de la información sensible detectada en los tableros de tu organización. Permite a los admins monitorear, clasificar y gestionar los riesgos de datos mediante la identificación del contenido relacionado con la privacidad o sensible de la empresa. El panel de descubrimiento de datos incluye las siguientes métricas:

> Todas las métricas de Enterprise Guard excluyen los tableros de equipos eliminados y los tableros bajo retención legal.

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Título** | **Descripción** | **Dominio** | **Aparece en el panel de vista general** | **Tiene métricas históricas** |
| Número de tableros sensibles | Número de tableros que tienen al menos una etiqueta integrada, una etiqueta de palabra clave o una etiqueta de privacidad asignada | Descubrimiento de datos | ✅ | ❌ |
| Número de tableros que contienen elementos sensibles de la empresa | Número de tableros que tienen al menos una etiqueta integrada o una etiqueta de palabra clave asignada | Descubrimiento de datos | ✅ | ✅ |
| Número de tableros que tienen elementos sensibles relacionados con la privacidad | Número de tableros que tienen asignada al menos una etiqueta de privacidad | Descubrimiento de datos | ✅ | ✅ |
| Número de tableros que tienen una etiqueta asignada por etiqueta | Para cada etiqueta individual en las tres categorías (integradas, de palabras clave o de privacidad), cuenta el número de tableros que tienen esa etiqueta asignada. | Descubrimiento de datos | ❌ | ❌ |
| Recuento de etiquetas habilitadas relacionadas con la privacidad | Recuento de etiquetas habilitadas relacionadas con la privacidad | Descubrimiento de datos | ❌ | ❌ |
| Recuento de etiquetas de palabras clave habilitadas | Recuento de etiquetas de palabras clave habilitadas | Descubrimiento de datos | ❌ | ❌ |
| Recuento de etiquetas sensibles de la empresa habilitadas | Recuento de etiquetas sensibles de la empresa habilitadas | Descubrimiento de datos | ❌ | ❌ |

## Comprender los errores, los estados vacíos y los cambios históricos

Comprender cómo interpretar los estados vacíos y los mensajes de error es esencial para leer con precisión las métricas del panel de Enterprise Guard.

### Comprender el comportamiento de los datos históricos cuando la configuración cambia

Si el descubrimiento de datos se deshabilita después de haber recopilado datos, las métricas históricas aún mostrarán valores del período activo. Por ejemplo, si deshabilitas el descubrimiento de datos en mayo y el descubrimiento de datos estaba activo en abril:

- Los valores de abril seguirán apareciendo en el panel.
- El gráfico de mayo mostrará **no hay datos disponibles**, ya que la recopilación de datos se ha detenido.

## Ver resultados del descubrimiento de datos

El ciclo de descubrimiento de datos se ejecuta al menos una vez cada hora y escanea todas las actualizaciones de los tableros en busca de información relacionada con la privacidad, sensible de la empresa o personalizada según la configuración de descubrimiento de datos. Esto incluye tableros que ya fueron escaneados en el ciclo anterior de descubrimiento de datos.

Los resultados del descubrimiento de datos aparecen debajo de los gráficos de métricas. Puedes ver información como el nombre de la etiqueta, estado, tipo, clasificación, número de tableros, y así sucesivamente.

Para más información sobre cómo revisar tableros con documentación relacionada con la privacidad, [consulta este artículo](16-review-boards-with-privacy-related-information.md).

Para obtener más información sobre cómo revisar tableros con datos sensibles de la empresa y datos sensibles personalizados, [consulta este artículo](14-review-boards-with-business-sensitive-and-custom-business-sensitive-information-beta.md).

Para obtener más información sobre la revisión de tableros con etiquetas personalizadas y sensibles de la empresa, [consulta este artículo](15-review-custom-business-sensitive-labels-and-data-discovery-results.md).

:::note
- Para ver los resultados del descubrimiento de datos, debes tener el [rol de admin de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de contenido sensible, ponte en contacto con el admin de empresa.

Aunque estamos trabajando continuamente con nuestro socio tecnológico y clientes para mejorar el sistema de detección de contenido sensible, no podemos garantizar que encontrará y marcará el 100% de los datos sensibles en tus tableros. Nuestro sistema de detección de contenido sensible utiliza patrones y otros criterios para determinar la probabilidad de una coincidencia. Puede haber momentos en que el sistema marque incorrectamente datos en tus tableros como probablemente sensibles (un falso positivo) o no logre marcar datos como sensibles (un falso negativo). Varios factores contribuyen a estas ocurrencias, incluyendo la proximidad de términos relacionados o el formato de datos sensibles.

Para más información sobre cómo puedes suprimir coincidencias de falsos positivos, consulta [Suprimir una coincidencia de contenido sensible](11-suppress-a-sensitive-content-match.md).
:::

##

##
