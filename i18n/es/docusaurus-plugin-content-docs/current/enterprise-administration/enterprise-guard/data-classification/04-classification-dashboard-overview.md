---
title: "Vista general del panel de clasificaci\xF3n"
article_id: 26886219054354
translation_id: 26886219054354
locale: es
sidebar_position: 3
created_at: '2025-05-22T11:26:15Z'
updated_at: '2025-08-18T09:36:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

El panel de clasificación ofrece una vista centralizada para que los administradores rastreen y gestionen la clasificación de los tableros en toda su organización. El panel ofrece un desglose claro de los tableros clasificados y no clasificados, ayudando a asegurar una cobertura completa e identificar áreas que necesitan atención.

Los administradores también pueden controlar el método de clasificación utilizado, ya sea manual, automático o no clasificado, para entender cómo se están categorizando los tableros. Además, el historial del método de clasificación visualiza los cambios a lo largo del tiempo, ofreciendo información sobre las tendencias y la eficacia de la clasificación de tableros en curso.

:::note
Notas sobre las métricas:

- Todas las métricas en Enterprise Guard excluyen los tableros de equipos en la papelera y los tableros bajo retención legal.
- Todos los métricos de clasificación excluyen plantillas y tableros en la papelera.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Título** | **Descripción** | **Dominio** | **Aparece en el panel de vista general** | **Tiene métricas históricas** |
| Número total de tableros que están clasificados | Número de tableros que tienen una etiqueta de clasificación asignada | Clasificación | ✅ | ❌ |
| Número de tableros por clasificación | Número de tableros por etiqueta de clasificación (nombre de la etiqueta) | Clasificación | ✅ | ❌ |
| Número de tableros no clasificados | Número de tableros que no tienen una etiqueta de clasificación asignada | Clasificación | ✅ | ✅ |
| Número de tableros clasificados manualmente | Número de tableros que tienen una etiqueta de clasificación asignada manualmente (lee: no por clasificación automática) | Clasificación | ❌ | ✅ |
| Número de tableros clasificados automáticamente | Número de tableros que tienen una etiqueta de clasificación asignada automáticamente por la clasificación automática | Clasificación | ❌ | ✅ |

## Comprender los errores, los estados vacíos y los cambios históricos

Comprender cómo interpretar los estados vacíos y los mensajes de error es esencial para leer con precisión las métricas del panel de Enterprise Guard.

### Comprender el comportamiento de los datos históricos cuando la configuración cambia

Si una función, como la clasificación, se deshabilita después de haber recopilado datos, las métricas históricas aún mostrarán valores del período activo. Por ejemplo, si deshabilitas la clasificación en mayo y la clasificación estaba activa en abril con 20 tableros clasificados:

- Los valores de abril seguirán apareciendo en el panel.
- El gráfico de mayo mostrará **no hay datos disponibles**, ya que la recopilación de datos se ha detenido.
