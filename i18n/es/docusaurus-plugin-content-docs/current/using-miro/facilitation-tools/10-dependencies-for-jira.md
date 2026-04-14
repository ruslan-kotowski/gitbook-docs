---
title: Dependencias para Jira
article_id: 10649083010834
translation_id: 10649083010834
locale: es
sidebar_position: 7
created_at: '2023-03-22T10:22:08Z'
updated_at: '2025-11-25T16:22:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

Mapa las dependencias existentes o crea nuevas entre las tarjetas de Jira en tu [planificador](../../integrations-apps/atlassian/21-planner-for-jira.md) o en cualquier lugar en tu tablero de Miro,  y se sincronizarán instantáneamente en Jira. Con la app Dependencias puedes identificar, visualizar, debatir y registrar dependencias entre equipos en tiempo real durante los ejercicios de planificación.

> ****💡**** Esta función ya está disponible para [Azure DevOps](08-dependencies-for-azure-devops.md).

> **Disponible para:** planes Business y Enterprise
>
> **Disponible en:** navegador de escritorio, aplicación de escritorio

## Cómo funcionan las dependencias

Las dependencias aparecen como una capa de líneas de conexión y muestran relaciones entre tarjetas de Jira.

Solo son visibles cuando abres dependencias en el tablero. Los participantes pueden filtrar diferentes tipos de dependencias para debatir obstáculos y relaciones.

![Dependencies-app.png](../../../../../../docs/using-miro/facilitation-tools/images/13244544218258_Dependencies-app.png)
*Dependencias mapeadas entre tarjetas de Jira en un widget de Planificador*

## Cómo crear una nueva dependencia

1. Ve a la barra de herramientas de creación en el lado izquierdo del tablero.
2. Haz clic en el icono de **Dependencias**. Si el icono de Dependencias no está en tu barra de herramientas de creación, tendrás que añadirlo desde **Herramientas, Medios e Integraciones** (**+**).
3. Se abrirá el panel Dependencias.
4. Haz clic en **Nueva dependencia**.
5. Haz clic en **Primera tarjeta** y selecciona una incidencia de Jira desde el menú desplegable o mediante la búsqueda.
6. Selecciona el **tipo de dependencia** según las opciones disponibles en tu instancia de Jira (por ejemplo, bloques, clones, duplicados o relacionados con).
7. Haz clic en **Segunda tarjeta** y selecciona una incidencia de Jira desde el menú desplegable o mediante la búsqueda.
8. Haz clic en **Guardar borrador**, o en **Guardar en Jira**directamente.

:::tip
Los borradores de dependencias se guardan solo en Miro. Puedes crear borradores de dependencias como sugerencias para otros participantes y equipos durante los ejercicios de planificación. Una vez que las hayan revisado y debatido, puedes guardarlas en Jira o eliminarlas.
:::

![dependencies-entry-point.png](../../../../../../docs/using-miro/facilitation-tools/images/21537435953426_dependencies-entry-point.png)
*Creando una nueva dependencia y guardándola en Jira*

## Cómo ver y filtrar dependencias

1. Ve a la barra de herramientas de creación en el lado izquierdo del tablero.
2. Haz clic en el ícono **Dependencias**. Si el ícono de Dependencias no está ya en tu barra de herramientas de creación, necesitas añadirlo desde **Herramientas, Medios e Integraciones** (**+**).
3. Se abrirá el panel de Dependencias y todas las dependencias existentes aparecerán como líneas en el tablero.
4. Haz clic en el ícono **Filtrar** en la parte superior del panel de Dependencias.
5. Usa los interruptores para filtrar por **tipo de dependencia** y **estado de sincronización**.
6. Utiliza el desplegable **Mostrar líneas** para controlar cuándo se muestran las dependencias. Selecciona **Siempre** para ver todas las dependencias activas. Elige **Al seleccionar** para ver dependencias solo cuando haces clic en una tarjeta de Azure específica o tipo de dependencia.

Las líneas de puntos muestran borradores de dependencias y las líneas continuas muestran dependencias que ya se sincronizaron con Jira. El color de la línea representa el tipo de dependencia.

![Filtering-dependencies.gif](../../../../../../docs/using-miro/facilitation-tools/images/13245295619730_Filtering-dependencies.gif)
*Filtrando la vista de la dependencia* *en el widget Planificador*

## Cómo editar, guardar, revertir o eliminar una dependencia

1. Ve a la barra de herramientas de creación en el lado izquierdo del tablero.
2. Haz clic en el **icono de Dependencias**.
3. Se abrirá el panel Dependencias.
4. Haz clic en el **icono de Editar** junto a una dependencia.

![The_option_to_edit_a_Dependency.jpg](../../../../../../docs/using-miro/facilitation-tools/images/10866625733778_The%20option%20to%20edit%20a%20Dependency.jpg)
*Editar una dependencia*

Puedes cambiar la **Primera tarjeta** y la **Segunda tarjeta** de una dependencia, así como el **tipo de dependencia.**

*![Editing_a_dependency.gif](../../../../../../docs/using-miro/facilitation-tools/images/10866808392722_Editing%20a%20dependency.gif)**Cambiando la Primera tarjeta y el Tipo de dependencia*

Haz clic en **Guardar en Jira** para guardar y sincronizar un borrador de dependencia en Jira.

![Save_to_Jira.png](../../../../../../docs/using-miro/facilitation-tools/images/10868740630034_Save%20to%20Jira.png)
*Guardar un borrador de dependencia en Jira*

Haz clic en **Revertir a borrador** para convertir una dependencia sincronizada de nuevo en borrador.

![Revert_to_draft.png](../../../../../../docs/using-miro/facilitation-tools/images/10868741500690_Revert%20to%20draft.png)
*Revertir una dependencia sincronizada en Jira a borrador*

Haz clic en el icono de **Papelera** para eliminar una dependencia.
![Delete_dependency.png](../../../../../../docs/using-miro/facilitation-tools/images/10868804195986_Delete%20dependency.png)*Eliminando una dependencia*
