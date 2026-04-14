---
title: Dependencias para Azure DevOps
article_id: 15556757538450
translation_id: 15556757538450
locale: es
sidebar_position: 6
created_at: '2023-12-05T11:50:18Z'
updated_at: '2025-11-25T15:39:53Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

Asigna dependencias entre tarjetas Azure en tu [Planificador](../../integrations-apps/microsoft/09-planner-for-azure-devops.md), o en cualquier lugar de tu tablero de Miro. Con la app Dependencias puedes identificar, visualizar, debatir y registrar dependencias entre equipos en tiempo real durante los ejercicios de planificación.

:::note
Para utilizar las dependencias para Azure DevOps, configura primero [tu integración de Azure](../../integrations-apps/microsoft/03-azure-cards.md).
:::

## Cómo funcionan las dependencias

Las dependencias aparecen como una capa de líneas de conexión, y muestran las relaciones entre las tarjetas Azure.

Sólo son visibles cuando abres dependencias en el tablero. Los participantes pueden filtrar diferentes tipos de dependencias para debatir obstáculos y relaciones.

![Mapa-dependencias-Azure.pngMapa de](../../../../../../docs/using-miro/facilitation-tools/images/15603398527890_Mapping-dependencies-Azure.png)
*dependencias en Azure*

## Cómo ver y filtrar dependencias

:::note
Sólo puedes ver y filtrar las relaciones que ya has creado en Azure. Pronto podrás crear y editar dependencias entre tarjetas Azure directamente en Miro.
:::

1. Ve a la barra de herramientas de creación, en la parte izquierda del tablero.
2. Haz clic en el **ícono** Dependencias. Si el icono de Dependencias no está en tu barra de herramientas de creación, tendrás que añadirlo desde **Herramientas, Medios e integraciones****(+**).
3. Se abrirá el panel Dependencias, y las dependencias existentes aparecerán como líneas en el tablero.
4. Haz clic en el ícono **Filtrar** en la parte superior del panel de Dependencias.
5. Utiliza los conmutadores para filtrar por **Tipo de dependencia**, representado por diferentes colores de línea.
6. Utiliza el desplegable **Mostrar líneas** para controlar cuándo se muestran las dependencias. Selecciona **Siempre** para ver todas las dependencias activas. Elige **En selección** para ver las dependencias sólo cuando hagas clic en una tarjeta Azure específica o en un tipo de dependencia.

![Mapear-dependencias-Azure-y-Jira.pngFiltrar](../../../../../../docs/using-miro/facilitation-tools/images/15603699800338_Mapping-dependencies-Azure-and-Jira.png)
*dependencias mapeadas*

## Tarjetas de Jira y Azure en el mismo tablero

Si tu equipo utiliza Azure DevOps y Jira, y has configurado ambas integraciones en Miro, puedes gestionar tarjetas y dependencias de ambos sistemas en un tablero.

Las dependencias enlazan dos tarjetas de Jira o dos tarjetas de Azure. Cuando abras la app Dependencias en un tablero con tarjetas de Azure y de Jira que tengan dependencias, mostraremos todos los enlaces existentes entre estas tarjetas.

Para filtrar las dependencias de un solo sistema, utiliza los conmutadores **Guardado en Jira** y **Guardado en Azure**.

![Dependencies-mapped-between-Jira-and-Azure-cards.pngDependencias](../../../../../../docs/using-miro/facilitation-tools/images/15603628660626_Dependencies-mapped-between-Jira-and-Azure-cards.png)
*tanto de Jira como de Azure en un único tablero de Miro*
