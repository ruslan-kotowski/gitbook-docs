---
title: "Referencia de m\xE9tricas del panel de Enterprise Guard"
article_id: 26718144750610
translation_id: 26718144750610
locale: es
sidebar_position: 5
created_at: '2025-05-15T00:17:54Z'
updated_at: '2025-07-22T20:38:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: admin-analytics
---

:::note
Notas sobre métricas:

- Todas las métricas de Enterprise Guard excluyen los tableros de equipos en la papelera.
- Todos los métricas de clasificación excluyen plantillas y tableros en la papelera.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Título** | **Descripción** | **Dominio** | **Aparece en el panel de vista general** | **Tiene métricas históricas** |
| Número total de tableros que están clasificados | Número de tableros que tienen una etiqueta de clasificación asignada | Clasificación | ✅ | ❌ |
| Número de tableros por clasificación | Número de tableros por etiqueta de clasificación (nombre de la etiqueta) | Clasificación | ✅ | ❌ |
| Número de tableros no clasificados | Número de tableros que no tienen una etiqueta de clasificación asignada | Clasificación | ✅ | ✅ |
| Número de tableros clasificados manualmente | Número de tableros que tienen una etiqueta de clasificación asignada manualmente (no por clasificación automática) | Clasificación | ❌ | ✅ |
| Número de tableros clasificados automáticamente | Número de tableros que tienen una etiqueta de clasificación asignada automáticamente por la clasificación automática | Clasificación | ❌ | ✅ |
| Número de tableros sensibles | Número de tableros que tienen al menos una etiqueta integrada, una etiqueta de palabra clave o una etiqueta de privacidad asignada | Descubrimiento de datos | ✅ | ❌ |
| Número de tableros que contienen información sensible de la empresa | Número de tableros que tienen al menos una etiqueta integrada o una etiqueta de palabra clave asignada | Descubrimiento de datos | ✅ | ✅ |
| Número de tableros que tienen elementos sensibles relacionados con la privacidad | Número de tableros que tienen asignada al menos una etiqueta de privacidad | Descubrimiento de datos | ✅ | ✅ |
| Número de tableros que tienen una etiqueta asignada por categoría de etiqueta | Número de tableros para cada categoría de etiqueta (incorporada, palabra clave o privacidad) | Descubrimiento de datos | ❌ | ❌ |
| Recuento de etiquetas habilitadas relacionadas con la privacidad | Número de etiquetas relacionadas con la privacidad habilitadas | Descubrimiento de datos | ❌ | ❌ |
| Recuento de etiquetas de palabras clave habilitadas | Número de etiquetas de palabras clave habilitadas | Descubrimiento de datos | ❌ | ❌ |
| Recuento de etiquetas sensibles de la empresa habilitadas | Número de etiquetas sensibles de la empresa habilitadas | Descubrimiento de datos | ❌ | ❌ |
| Número total de tableros | Número total de tableros en todos los estados del ciclo de vida (activo, en la papelera, retenido) | Gestión del ciclo de vida del contenido | ✅ | ❌ |
| Número de tableros activos. Esto NO es la actividad del tablero, sino tableros que están en el estado de ciclo de vida activo | Número total de tableros en estado de ciclo de vida activo | Gestión del ciclo de vida del contenido | ✅ | ✅ |
| Número de tableros en la papelera | Número total de tableros en estado de ciclo de vida eliminado | Gestión del ciclo de vida del contenido | ✅ | ✅ |
| Número de tableros retenidos | Número total de tableros en estado de ciclo de vida retenido | Gestión del ciclo de vida del contenido | ✅ | ✅ |
| Número de tableros bajo retención | Número total de tableros que tienen asignada al menos una política de retención no expirada | Gestión del ciclo de vida del contenido | ❌ | ✅ |
| Número de tableros afectados por la eliminación | Número total de tableros que tienen asignada al menos una política de eliminación no expirada | Gestión del ciclo de vida del contenido | ❌ | ❌ |
| Número de tableros bajo una política de retención, agrupados por política | Número de tableros en cualquier estado del ciclo de vida que tienen al menos una política de retención asignada | Gestión del ciclo de vida del contenido | ✅ | ❌ |
| Número de tableros bajo una política de eliminación, agrupados por política | Número de tableros en cualquier estado del ciclo de vida que tienen al menos una política de eliminación asignada | Gestión del ciclo de vida del contenido | ✅ | ❌ |
| Número de tableros creados este día/semana/mes | Número de tableros creados esta semana | Gestión del ciclo de vida del contenido | ❌ | ✅ |
| Número de tableros eliminados (movidos a la papelera) este día/semana/mes | Número de tableros eliminados (movidos a la papelera) esta semana | Gestión del ciclo de vida del contenido | ❌ | ✅ |
| Número de tableros bajo políticas de eliminación, agrupados por la fecha de vigencia de la política de eliminación por mes |  | Gestión del ciclo de vida del contenido | ❌ | ❌ |
| Número de casos | Número total de casos | eDiscovery | ✅ | ❌ |
| Número de retenciones legales | Número total de retenciones legales | eDiscovery | ✅ | ❌ |
| Número de retenciones legales para un caso específico | Número total de retenciones legales para un caso específico | eDiscovery | ❌ | ❌ |
| Número de tableros bajo retención legal | Número total de tableros que están en retención en todas las retenciones legales | eDiscovery | ❌ | ❌ |
| Usuarios bajo retención legal y el número total de sus tableros | Lista a los usuarios bajo retención legal y el número total de sus tableros | eDiscovery | ❌ | ❌ |
