---
title: "App Estimaci\xF3n"
article_id: 5651786248210
translation_id: 5651786248210
locale: es
sidebar_position: 8
created_at: '2022-05-20T11:28:11Z'
updated_at: '2025-11-25T16:08:42Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: estimation
---

Las estimaciones son una parte vital del desarrollo y la planificación Agile. Ayudan a alinear a los miembros del equipo sobre el alcance del trabajo, a identificar falencias en el análisis o la comprensión y a establecer expectativas claras para la entrega.

Durante las estimaciones, los miembros del equipo asignan un número a una tarea que refleje la cantidad de trabajo requerido. Para hacer estimaciones realistas, se utiliza un sistema de numeración que va sumando los números anteriores. De esa forma, los miembros del equipo pueden conversar y alinearse en relación con el número que eligieron.

Usa nuestra app Estimación para realizar sesiones de estimación con varios participantes en un tablero de Miro con [tarjetas](../essential-tools/02-cards.md), [notas adhesivas](../essential-tools/14-sticky-notes.md) y [tarjetas Jira](../../integrations-apps/atlassian/03-jira-cards.md).

> **Disponible para:** planes Starter, Business y Enterprise
> **Configurado por**: miembros del equipo con derechos para editar el tablero

Para iniciar la estimación:

1. Accede a la app Estimación desde la barra de herramientas de creación y selecciona **Iniciar nueva sesión**. Puede que tengas que añadir la app Estimación desde el icono **Herramientas, medios e integraciones** (**+**):
   ![estimation-entry-point.png](../../../../../../docs/using-miro/facilitation-tools/images/21537436002962_estimation-entry-point.png)*App Estimación en la barra de herramientas*
2. Selecciona la escala de estimación: en el menú desplegable, elige la **camiseta** (disponible solo para las [tarjetas](../essential-tools/02-cards.md) de Miro) o  **la técnica de estimación Fibonacci**
3. Arrastra el área de estimación a través de los objetos que quieras estimar. Puedes seleccionar tarjetas, notas adhesivas o [tarjetas de Jira](../../integrations-apps/atlassian/03-jira-cards.md) para la estimación. Puedes excluir objetos específicos de la estimación haciendo clic en los puntos azules.
4. Si la selección incluye tarjetas de Jira, se te pedirá que selecciones el tablero de Jira al que pertenecen estas tarjetas. Esto garantiza que tus estimaciones se guarden de forma precisa y predecible en Jira. Sin este paso, Jira no puede guardar estas estimaciones.
5. Haz clic en **Estimar x tarjetas/stickies** cuando estés listo para iniciar la estimación.![estimation_launch.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016786471186_estimation%20launch.gif)*Inicio de la sesión de estimación*![estimation_app_jira_cards.png](../../../../../../docs/using-miro/facilitation-tools/images/21016786474514_estimation_app_jira_cards.png)*Uso de la app Estimación con las tarjetas de Jira*

Todos los usuarios del tablero (y aquellos que se unan al tablero mientras la sesión de estimación está en curso) podrán unirse a la sesión. Todos los participantes deben tener acceso de edición del tablero y permisos de Jira. Las estimaciones se pueden hacer de forma sincrónica o asíncrona. Todas las estimaciones son anónimas.

![join_estimation.jpg](../../../../../../docs/using-miro/facilitation-tools/images/21016751234578_join%20estimation.jpg)
*Ventana emergente para unirse a la sesión de estimación*

Los usuarios serán redirigidos al primer elemento para agregar sus estimaciones después de hacer clic en **Unirse a la estimación**. Los usuarios pueden votar sobre todos los elementos o saltarse algunos y votar solo sobre algunos en particular. Para añadir una estimación, haz clic en el icono de bolígrafo.

![adding_estimates.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016751237010_adding%20estimates.gif)
*Estimación en curso*

A medida que se ejecuta la sesión, el facilitador puede ver una encuesta de las estimaciones proporcionadas para cada elemento y los avatares de quienes las proporcionaron. Cuando todos los participantes afectados hayan proporcionado estimaciones de todos los elementos, el facilitador puede “Elegir la estimación final” para cada elemento. El facilitador también puede editar las estimaciones acordadas.

![agreed_estimates.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016751238162_agreed%20estimates.gif)
*Estimación finalizada*

Una vez que acuerden las estimaciones de todos los elementos, el facilitador verá la ventana emergente con la opción para finalizar la sesión y compartir los resultados. El facilitador también puede hacer clic en **Finalizar para todos** para terminar la sesión en cualquier momento. Esto mostrará el número total de puntos. Haz clic en **Finalizar y compartir resultados** en la ventana emergente, y los resultados de la sesión se guardarán.

![end_session.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016751242386_end%20session.gif)
*Acuerdo de estimación*

Si estimas tarjetas o notas adhesivas de Miro, las estimaciones se guardan como etiquetas en las tarjetas o notas adhesivas.

![estimate_tags.jpg](../../../../../../docs/using-miro/facilitation-tools/images/21016786489362_estimate%20tags.jpg)
*Las etiquetas muestran las estimaciones de las tarjetas*

Si estimas tarjetas de Jira usando la técnica de estimación de **Fibonacci**, los cálculos se guardan en Jira (al momento, la sincronización solo funciona para los estimados de Fibonacci). Ten en cuenta que el facilitador debe autorizar con sus credenciales de Jira antes de dar las estimaciones finales. Los resultados de la estimación se sincronizarán automáticamente con las incidencias de Jira correspondientes.

**Para que las estimaciones de Fibonacci aparezcan en las tarjetas y tareas de Jira:**

1. Asegúrate de que el campo puntos de historia esté configurado en Jira.
2. Asegúrate de tener el permiso relevante en Jira para actualizar el valor del campo puntos de historia.
