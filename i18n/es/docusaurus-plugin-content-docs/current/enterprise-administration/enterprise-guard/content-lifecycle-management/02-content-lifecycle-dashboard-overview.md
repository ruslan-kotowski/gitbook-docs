---
title: Vista general del panel del ciclo de vida del contenido
article_id: 26894063726482
translation_id: 26894063726482
locale: es
sidebar_position: 2
created_at: '2025-05-22T16:02:58Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

El panel del ciclo de vida del contenido proporciona una vista centralizada para que los administradores supervisen y gestionen el ciclo de vida completo de los tableros, desde la creación hasta la eliminación, mientras se alinean con las políticas de retención de datos de la organización. Proporciona visibilidad sobre la etapa actual del ciclo de vida de cada tablero, ayudando a garantizar un manejo adecuado del contenido.

Los administradores también pueden rastrear los tableros gobernados por políticas de retención y eliminación, y ver las tendencias históricas de la aplicación de políticas. El panel incluye una previsión de eliminación, permitiendo una planificación proactiva para las próximas acciones automatizadas del ciclo de vida. Esto habilita la gobernanza de contenido consistente y basada en políticas en toda la organización.

:::note
Todas las métricas en Enterprise Guard excluyen tableros de equipos eliminados y tableros bajo retención legal.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Título** | **Descripción** | **Dominio** | **Aparece en el panel de vista general** | **Tiene métricas históricas** |
| Número total de tableros | Número total de tableros en todos los estados del ciclo de vida (activo, en la papelera, retenido) | Gestión del ciclo de vida del contenido | ✅ | ❌ |
| Número de tableros activos. Esto NO es la actividad del tablero, sino tableros que están en el estado de ciclo de vida activo | Número total de tableros en estado de ciclo de vida activo | Gestión del ciclo de vida del contenido | ✅ | ✅ |
| Número de tableros en la papelera | Número total de tableros en estado de ciclo de vida eliminado | Gestión del ciclo de vida del contenido | ✅ | ✅ |
| Número de tableros retenidos | Número total de tableros en estado de ciclo de vida retenido | Gestión del ciclo de vida del contenido | ✅ | ✅ |
| Número de tableros bajo retención | Número total de tableros que tienen asignada al menos una política de retención no expirada | Gestión del ciclo de vida del contenido | ❌ | ✅ |
| Número de tableros afectados por la eliminación | Número total de tableros que tienen asignada al menos una política de eliminación no expirada | Gestión del ciclo de vida del contenido | ❌ | ❌ |
| Número de tableros bajo una política de retención, agrupados por política | Número de tableros en cualquier estado del ciclo de vida que tienen asignada al menos una política de retención por política | Gestión del ciclo de vida del contenido | ✅ | ❌ |
| Número de tableros bajo una política de eliminación, agrupados por política | Número de tableros en cualquier estado del ciclo de vida que tienen al menos una política de eliminación asignada por política | Gestión del ciclo de vida del contenido | ✅ | ❌ |
| Número de tableros creados este día/semana/mes | Número de tableros creados esta semana | Gestión del ciclo de vida del contenido | ❌ | ✅ |
| Número de tableros eliminados (movidos a la papelera) este día/semana/mes | Número de tableros eliminados (movidos a la papelera) esta semana | Gestión del ciclo de vida del contenido | ❌ | ✅ |
| Número de tableros bajo políticas de eliminación, agrupados por la fecha de vigencia de la política de eliminación por mes |  | Gestión del ciclo de vida del contenido | ❌ | ❌ |

## Comprender los errores, los estados vacíos y los cambios históricos

Comprender cómo interpretar los estados vacíos y los mensajes de error es esencial para leer con precisión las métricas del panel de Enterprise Guard.

### Comprender el comportamiento de los datos históricos cuando la configuración cambia

Si el descubrimiento de datos se deshabilita después de haber recopilado datos, las métricas históricas aún mostrarán valores del período activo. Por ejemplo, si deshabilitas el descubrimiento de datos en mayo y el descubrimiento de datos estaba activo en abril:

- Los valores de abril seguirán apareciendo en el panel.
- El gráfico de mayo mostrará **no hay datos disponibles**, ya que la recopilación de datos se ha detenido.

###
