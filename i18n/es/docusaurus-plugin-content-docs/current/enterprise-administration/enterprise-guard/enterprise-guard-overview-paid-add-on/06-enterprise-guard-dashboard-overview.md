---
title: Vista general del panel de Enterprise Guard
article_id: 26707467343890
translation_id: 26707467343890
locale: es
sidebar_position: 4
created_at: '2025-05-14T13:14:06Z'
updated_at: '2025-11-25T15:51:12Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: admin-analytics
---

## Vista centralizada de seguridad y gobernanza

El panel de Enterprise Guard ofrece una vista centralizada y de alto nivel de los conocimientos de seguridad y gobernanza de información de tu organización en una única vista unificada. Diseñado para los administradores de Enterprise Guard, este panel reúne métricas clave a través de dominios centrales, incluyendo el descubrimiento de datos, la clasificación, el ciclo de vida del contenido y el eDiscovery, en una única interfaz consolidada. Permite una visibilidad rápida de la exposición actual, la cobertura de políticas y la preparación legal, lo que empodera a los administradores para detectar riesgos potenciales temprano, tomar medidas proactivas y oportunas, y abordar cualquier área que requiera atención.

## Métricas prácticas en tiempo real

Cada métrica en el panel de Enterprise Guard refleja datos en tiempo real, actualizados diariamente. Todos los datos son accionables y están vinculados directamente a sus respectivos paneles, lo que permite a los administradores explorar insights detallados y configurar la configuración según sea necesario. Ya sea que estés monitoreando la sensibilidad del tablero, el estado de clasificación, las políticas de retención o las retenciones legales, este panel ofrece un punto de partida centralizado. Este enfoque en capas garantiza la consistencia en todo el producto Enterprise Guard y simplifica la navegación para los administradores ocupados.

## Soporte para gobernanza a gran escala

El panel de Enterprise Guard es especialmente útil para los admins de Enterprise Guard que gestionan despliegues a gran escala en el plan Enterprise. Aporta claridad a configuraciones complejas de gobernanza de la información y apoya la toma de decisiones informadas al consolidar las señales más importantes en un solo lugar. Como parte de nuestro compromiso con una experiencia Enterprise Guard más intuitiva, el panel de Enterprise Guard ayuda a los admins no solo a entender lo que está sucediendo, sino también a saber qué hacer a continuación, con enlaces para tomar acciones directamente desde los datos. Ya sea que estés informando a la dirección o gestionando la gobernanza de datos diaria, este panel garantiza que puedas acceder a información relevante rápidamente, priorizar acciones y demostrar el valor de la estrategia de seguridad y cumplimiento de tu organización.

## Paneles relacionados específicos del dominio

Además del panel de Enterprise Guard, los administradores pueden explorar un paquete de paneles específicos de dominio diseñados para proporcionar un mayor entendimiento y control en áreas clave de gobernanza. Cada uno de estos paneles permite una toma de decisiones enfocada dentro de su área respectiva mientras mantiene la alineación con el marco más amplio de Enterprise Guard. Entre estos se incluyen:

- **Panel de descubrimiento de datos:** explorar y analizar dónde reside la información sensible en tus tableros.
- **Panel de clasificación:** rastrear y gestionar la cobertura de clasificación a nivel de tablero y las etiquetas de sensibilidad.
- **Panel del ciclo de vida del contenido:** monitorear las políticas de retención de datos y automatizar las acciones de gestión del ciclo de vida.
- **Panel de eDiscovery:** obtener visibilidad sobre las retenciones legales y optimizar los flujos de trabajo de preparación de eDiscovery.

## Comprender las métricas del panel

Los paneles de Enterprise Guard incluyen dos tipos de métricas: métricas actuales y métricas históricas. Para asegurar claridad y consistencia, cada métrica presentada en los paneles de Enterprise Guard está definida en la [documentación de métricas del panel de Enterprise Guard](07-enterprise-guard-dashboard-metrics-reference.md).

:::note
Notas sobre métricas:

- Todas las métricas en Enterprise Guard excluyen tableros de equipos en la papelera y tableros bajo retención legal.
- Todas las métricas de clasificación excluyen las plantillas y los tableros en la papelera.
:::

## Comprender los errores, los estados vacíos y los cambios históricos

Comprender cómo interpretar los estados vacíos y los mensajes de error es esencial para leer con precisión las métricas del panel de Enterprise Guard.

### Comprender el comportamiento de los datos históricos cuando la configuración cambia

Si una función, como la clasificación, se deshabilita después de haber recopilado datos, las métricas históricas seguirán mostrando valores del período activo. Por ejemplo, si deshabilitas la clasificación en mayo y la clasificación estaba activa en abril con 20 tableros clasificados:

- Los valores de abril seguirán apareciendo en el panel.
- El gráfico de mayo mostrará **no hay datos disponibles**, ya que la recopilación de datos se ha detenido.
