---
title: Planificador para Jira
article_id: 10648975837970
translation_id: 13241218459794
locale: es
sidebar_position: 22
created_at: '2023-08-23T08:45:49Z'
updated_at: '2026-02-09T13:21:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Con el planificador para Jira, los facilitadores y los equipos pueden realizar y participar en eventos de planificación en un tablero de Miro, mientras sincronizan en tiempo real las actualizaciones con su tablero de Jira, ahorrando horas de trabajo manual.

> **Disponible para:** planes Business, Enterprise

Durante los eventos de planificación del equipo y de la empresa, como los incrementos de programa (PI), Big Room, roadmap y sprints, los equipos de desarrollo debaten y se alinean entre sí.

:::tip
El planificador ahora está disponible para [Azure DevOps](https://help.miro.com/hc/articles/15280547945618).
:::

## Cómo crear un planificador para Jira

1. Ve a la [barra de herramientas de creación](https://help.miro.com/hc/articles/360017730553-Toolbars) del lado izquierdo del tablero.
2. Haz clic en **Más aplicaciones** (**+**) y busca 'Planificador'.
3. Haz clic en **Planificador** para iniciar la aplicación.
4. Aparecerá un cursor en el tablero. Haz clic en cualquier lugar para colocar un planificador en blanco.
5. Haz clic en el menú desplegable **Tablero de Jira** y selecciona un tablero para conectarlo al planificador. Si aún no has autorizado tu cuenta de Jira en Miro, se te pedirá que inicies sesión.
6. El primer campo de **Columnas** es tu *tipo de columna*. Después de seleccionar el tablero de Jira, el tipo de columna predeterminado será **Estado**, y mostrará hasta 3 columnas. Haz clic en el primer campo de **Columnas** para seleccionar un tipo de columna diferente desde el menú desplegable (puedes elegir Sprint, Estado, Prioridad, Versiones de corrección, Componentes o un campo personalizado).
7. Usa el segundo campo de **Columnas** para refinar tu Planificador. Por ejemplo, si elegiste 'Sprint' como tu campo de columna, puedes seleccionar qué sprints mostrar.
8. Agrega **Swimlanes** a tu planificador, además de columnas, para organizar aún más las tareas en función de un segundo campo de Jira (puedes elegir entre Sprint, Estado, Prioridad, Versión de corrección, Componentes, o un campo personalizado).

:::note
Actualmente el planificador solo admite un tablero de Jira. Sin embargo, puedes crear múltiples planificadores en un solo tablero de Miro.
:::

![Creating-a-planner-widget.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696033042_Creating-a-planner-widget.gif)*Creando un planificador*

## Cómo trabajar con el planificador

Arrastra tarjetas de Jira por las columnas para actualizarlas. Por ejemplo, arrastrar una tarjeta de Jira desde el backlog a un sprint en el planificador la actualizará tanto en Miro como en Jira.

![Dragging-stories-between-columns-planning-widget.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696028306_Dragging-stories-between-columns-planning-widget.gif)*Moviendo tarjetas de Jira entre sprints*

Elige un campo para **carriles** para dividir tu trabajo en filas y columnas. Si mueves tarjetas entre carriles, se actualizarán los campos *de columna* y *carril* de la incidencia de Jira.

![Choosing-a-swimlane.png](../../../../../../docs/integrations-apps/atlassian/images/21017725756946_Choosing-a-swimlane.png)*Elegir un campo para los carriles*

Por defecto, el planificador muestra todas las incidencias en tu backlog. Para enfocarte en el sprint actual, selecciona el ícono de filtro en la parte superior derecha y marca **Sprint**. Luego selecciona el filtro **Sprint** y habilita **Filtrar por sprint activo**. Selecciona **Aplicar** para aplicar tu filtro de sprint.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*Filtrar incidencias por sprint activo.*

También puedes usar el menú desplegable **Tipo de incidencia** y seleccionar qué tipos de incidencia mostrar en tu planificador. Por ejemplo, puedes filtrar solo por historia.

![Filtering-by-issue-type-planning-widget.png](../../../../../../docs/integrations-apps/atlassian/images/21017725749138_Filtering-by-issue-type-planning-widget.png)*Filtrar por tipo de incidencia*

Los participantes pueden comentar sobre las tarjetas de Jira para realizar un seguimiento de las discusiones y notas en curso.

![Commenting_on_a_story.png](../../../../../../docs/integrations-apps/atlassian/images/21017696024594_Commenting%20on%20a%20story.png)*Comentar sobre una tarjeta de Jira en el planificador*

:::note
Las tarjetas de Miro, las notas adhesivas y otros objetos no se pueden colocar dentro de un planificador.
:::

## Capacidad y carga

Toma decisiones de priorización informadas durante los Sprints y PI Planning visualizando los totales de los puntos de historia en columnas fáciles de leer. Aumenta la eficiencia de tu equipo y garantiza una distribución óptima del trabajo.

### Habilitar el campo de puntos de historia en las tarjetas de Jira

1. Ve a la [barra de creación](https://help.miro.com/hc/articles/360017730553-Toolbars#Creation_toolbar) en el lado izquierdo de tu tablero.
2. Haz clic en **Más aplicaciones** (**+**) y busca ‘tarjetas de Jira’.
3. Haz clic en **tarjetas de Jira** para abrir la aplicación.
4. Haz clic en **Configurar tarjetas**.
5. Desplázate hacia abajo y activa **puntos de historia**.

![Enabling-Story-Points-for-Jira-Cards.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696030866_Enabling-Story-Points-for-Jira-Cards.gif)
*Habilitación de puntos de historia para tarjetas de Jira*

### Usar capacidad y carga

Una vez que habilites los puntos de historia, puedes crear un nuevo planificador o actualizar un tablero que ya contenga uno. Siempre que al menos una incidencia en el tablero tenga puntos de historia asignados, verás instantáneamente los campos de **capacidad** y **carga** en la parte superior de cada columna de tu planificador.

![Balancing-Capacity-and-Load.gif](../../../../../../docs/integrations-apps/atlassian/images/21017725755794_Balancing-Capacity-and-Load.gif)*Equilibrar capacidad y carga*

### Comprender las variables de capacidad y carga

**Capacidad**: ingresa manualmente la capacidad de cada columna en tu planificador. Si la capacidad es menor que la carga, la columna se volverá roja para indicar que excediste la capacidad de tu equipo. Esta indicación visual te sugiere que consideres reasignar incidencias para mantener una carga de trabajo equilibrada.

**Carga**: representa la suma de los puntos de historia de todas las tarjetas en una columna determinada. Las tarjetas sin puntos de historia contarán como 0 en este cálculo.

## Configuración de Jira

Para configurar el planificador, comienza por elegir un tablero de Jira para importar incidencias. Esto puede ser desde un tablero de Scrum o Kanban de Jira.

Cuando creas un planificador, puedes elegir qué campo de Jira usar para tus columnas y filas (carriles), incluyendo:

- Sprints
- Estado
- Versión de corrección
- Componente
- Prioridad
- Persona asignada
- Cualquier campo personalizado con una selección de valor único en el menú desplegable
- Cualquier campo personalizado con una selección desplegable de valores múltiples

Actualmente, no contamos con soporte para otros campos de Jira o campos relacionados con fechas.

La opción Sprint solo aparecerá si el campo Sprint está disponible en la pantalla de edición de incidencias en Jira. Esto suele estar preconfigurado para el Servidor o Centro de Datos de Jira, pero con frecuencia en la versión Cloud se necesita agregar manualmente el campo Sprint. Lee más sobre [cómo configurar las pantallas de incidencias](https://support.atlassian.com/jira-cloud-administration/docs/configure-issue-screens/).

:::note
Los sprints cerrados no se pueden mostrar en el Planificador.
:::

### Cómo crear un planificador usando un JQL personalizado

Para crear un planificador utilizando un JQL personalizado, comienza por crear un tablero de Jira con tu consulta de JQL. Después de que se cree el tablero de Jira, sigue las instrucciones anteriores para crear un planificador. Cuando llegues al paso 5, recuerda elegir el tablero de Jira que creaste con tu consulta de JQL personalizada.

## Sincronización del planificador

### De Miro a Jira

Cuando arrastras una tarjeta entre campos personalizados en Miro, Jira se actualiza automáticamente. Esto puede tardar unos segundos.

### De Jira a Miro

Si realizas cambios en un sprint en Jira, verás una notificación de **Actualizaciones disponibles** en el menú contextual del planificador. Esto podría tardar unos segundos después de que hagas los cambios en Jira.

Haz clic en el planificador para abrir el menú contextual y haz clic en el ícono **Sincronizar con Jira** para sincronizar los cambios más recientes.

![Sync-planning-widget-with-jira.png](../../../../../../docs/integrations-apps/atlassian/images/21017696029970_Sync-planning-widget-with-jira.png)*Sincronizar actualizaciones de Jira a Miro*

## Mapeo de dependencias

Los participantes pueden mapear visualmente las dependencias entre tareas en el planificador. Aprende más sobre [Dependencias para Jira](https://help.miro.com/hc/articles/10649083010834).
