---
title: Planificador para Azure DevOps
article_id: 15280547945618
translation_id: 15280547945618
locale: es
sidebar_position: 10
created_at: '2023-11-23T14:12:19Z'
updated_at: '2025-11-25T15:39:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: program-board-widget
availability:
  notes: 'Disponible para: plan Education, plan Enterprise, plan Business'
---

Durante los eventos de planificación del equipo y de la empresa, como los incrementos de programa (PI), Big Room, Roadmapping y Sprints, los equipos de desarrollo debaten y se ponen de acuerdo entre sí.

Con el Planificador para Azure, los moderadores y equipos pueden ejecutar y participar en eventos de planificación en un tablero de Miro, a la vez que sincronizan las actualizaciones con su tablero de Azure en tiempo real, ahorrando horas de trabajo manual.

## Cómo crear un Planificador para Azure DevOps

:::note
Para utilizar el Planificador para Azure DevOps, configura primero [tu integración en Azure](03-azure-cards.md).
:::

1. Navega hasta la barra de herramientas de creación situada a la izquierda de tu tablero.
2. Haz clic en ****Más aplicaciones**** (+) y busca "Planificador".
3. Haz clic en **Planificador.**
4. Aparecerá un cursor en el tablero.  Haz clic en cualquier lugar para colocar un Planificador en blanco.
5. La fuente de datos de tu Planificador será por defecto la integración que hayas autorizado. Si aún no has autorizado una integración, por defecto será Jira. Puedes cambiarlo fácilmente a Azure **DevOps** haciendo clic en el menú desplegable etiquetado **Jira** y seleccionando **Azure DevOps**.
6. Si aún no has autorizado tu cuenta de Azure DevOps en Miro, se te instruirá para que iniciar sesión.
7. Una vez que hayas iniciado sesión, haz clic en el menú desplegable **del proyecto Azure** y selecciona un proyecto para conectarlo al Planificador.
8. A continuación, haz clic en el menú desplegable **Equipos** y selecciona un equipo.
9. El primer **campo**, *Columnas*, es el tipo de columna. La **iteración** se selecciona automáticamente. Pronto habrá más campos Azure.
10. Utiliza el segundo desplegable **Columnas** para afinar aún más qué iteraciones quieres mostrar.

## Cómo trabajar con el Planificador

Arrastra las tarjetas Azure por las columnas para actualizarlas. Por ejemplo, si arrastras una tarjeta Azure de la Iteración 1 a la Iteración 2 en el Planificador, se actualizará tanto en Miro como en Azure.

Los participantes pueden comentar las tarjetas Azure para hacer un seguimiento de las discusiones y notas en curso.

![Comentario-sobre-un-Azure-Planificador.png](../../../../../../docs/integrations-apps/microsoft/images/21016020674450_Comment-on-an-Azure-Planner.png)*Comentario sobre el Planificador*

## Sincronización del Planificador

### De Miro a Azure

Cuando arrastras una tarjeta entre campos personalizados en Miro, Azure se actualiza automáticamente. Esto puede tardar unos segundos.

### De Azure a Miro

Para asegurarte de que tu Planificador se mantiene actualizado con los cambios que hagas en Azure, selecciona el Planificador y haz clic en el botón **Sincronizar** del menú contextual.

![Sincronizar el planificador con Azure.png](../../../../../../docs/integrations-apps/microsoft/images/21016020674962_Syncying-the-planner-with-Azure.png)*Sincronizar el Planificador con Azure*

Los campos compatibles con Azure actualmente son:

- Iteración (también conocido como sprint).
- Asignado a
- Todos los demás campos que se ajusten a los siguientes criterios:
  - Editable (es decir, no de sólo lectura).
  - Valores de cadena (texto).
  - Una lista de valores predefinidos que se pueden establecer (es decir, no texto de flujo libre).
  - Válido para los elementos de trabajo de Azure (algunos campos de Azure tienen otros usos).

# ¿No ves los sprints de tu equipo?

Asegúrate de que tus iteraciones en Azure están mapeadas en tu equipo para que puedas visualizarlas en el Planificador.

1. Ve a tu **Proyecto** en Azure.
2. En la parte inferior del menú lateral derecho, haz clic en el icono **Configuración del proyecto** .
3. Ve a la sección **Tableros** y haz clic en **Configuración del equipo**.
4. Haz clic en la pestaña **Iteraciones**, en la parte superior de la pantalla.
5. Haz clic en **+ Seleccionar iteración**. Asegúrate de haber añadido todas las iteraciones relacionadas con tu equipo.

![Añadir-iteraciones-Azure-Devops.png](../../../../../../docs/integrations-apps/microsoft/images/21016020675858_Adding-iterations-Azure-Devops.png)*Añadir iteraciones a Azure*

## Creación de mapas de dependencias

Los participantes pueden mapear visualmente las dependencias entre tareas en el planificador. Más información sobre [Dependencias para Azure](../../using-miro/facilitation-tools/08-dependencies-for-azure-devops.md).
