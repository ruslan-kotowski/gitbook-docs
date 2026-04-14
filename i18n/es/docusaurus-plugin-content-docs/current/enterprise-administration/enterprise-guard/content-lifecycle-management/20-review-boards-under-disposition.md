---
title: "Revisar tableros afectados por pol\xEDticas de eliminaci\xF3n"
article_id: 19944607919890
translation_id: 19944607919890
locale: es
sidebar_position: 20
created_at: '2024-07-04T15:26:03Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

El panel del ciclo de vida del contenido permite a [los administradores de la gobernanza de datos](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) ver todos los tableros con una política de disposición aplicada, incluyendo aquellos que son movidos automáticamente a la papelera. Cuando haces clic en el encabezado **Eliminación** en el tablero del ciclo de vida del contenido, aparece la página **Retención y eliminación** donde puedes:

- Ver tableros con una política de eliminación aplicada. Ver información como el nombre del tablero, el propietario del tablero, el equipo al que pertenece el tablero, el estado actual del tablero (activo, en la papelera o retenido), la fecha en que el tablero se moverá automáticamente a la papelera según la política de disposición, o si el tablero está en la papelera según la política de disposición.
- Filtrar los resultados para ver la información específica que necesitas. Por ejemplo, puedes filtrar la lista de tableros en función del equipo, el propietario, el nivel de clasificación, el estado del tablero o los criterios de uso del tablero, como la duración de la última edición (fechas de última edición desde y última edición hasta). También puedes filtrar el contenido en función de los criterios de la política de disposición o retención, como la política de disposición aplicada, la fecha de inicio y fin de disposición, la política de retención, la fecha de inicio y fin de retención.
- Revisar cada resultado haciendo clic en el elemento de la fila. Aparece un panel lateral (Figura 2) donde puedes ver información, como el nombre del tablero, el propietario del tablero, el equipo al que pertenece el tablero, el estado actual del tablero (activo, en la papelera o retenido), información aplicable sobre la política de retención y disposición.

:::note
Para revisar tableros bajo disposición, debes tener el [rol de admin de gobernanza de datos](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de gobernanza de datos, ponte en contacto con el admin de empresa.
:::

## Revisar tableros con política de eliminación aplicada

Para revisar un tablero con una política de eliminación aplicada, realiza los siguientes pasos:

1. Haz clic en tu avatar de perfil y luego en **Consola de administración**.
2. En la barra lateral izquierda, haz clic en **Enterprise Guard** y luego en **Ciclo de vida del contenido**.
3. En la página **Resumen del ciclo de vida del contenido**, haz clic en el encabezado **Retención**.
   La página de **Retención y eliminación** aparece con una lista de tableros.
4. En la página de **Retención y disposición** , haz clic en el tablero que quieres revisar.
   Aparece un panel lateral a la derecha de la pantalla con la siguiente información:
   - Nombre del tablero
   - Propietario del tablero
   - Equipo al que pertenece el tablero
   - Estado actual del tablero (activo, en la papelera o retenido)
   - Fecha hasta la que el tablero está bajo retención
   - Política de retención aplicada al tablero, si corresponde, e información asociada, como el alcance de la retención y la fecha hasta la que el tablero está bajo retención
   - Política de eliminación aplicada al tablero, si corresponde, y la información asociada, como la fecha en que el tablero se moverá automáticamente a la papelera.

## Filtrar la lista de tableros

Puede haber ocasiones en las que la lista de tableros muestre una larga lista de tableros que están bajo disposición y quieras personalizar la lista de resultados en función de requisitos específicos. [Los admins de gobernanza de datos](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) tienen ahora la capacidad de filtrar la lista de tableros según diversos criterios, mejorando la capacidad de centrarse en aspectos clave de sus tareas de gestión del ciclo de vida del contenido.

Las opciones de filtrado no solo incluyen criterios de equipo y propietario de los tableros, sino que también se extienden a criterios relacionados con el uso y la retención de los tableros. Puedes filtrar la lista de tableros en función de varios criterios relacionados con los tableros, como el equipo, el propietario, el nivel de clasificación, el estado del tablero o los criterios de uso del tablero, como la duración de la última edición (fechas de última edición desde y hasta). También puedes filtrar el contenido según los criterios de la política de disposición, como la política de disposición aplicada o la fecha de inicio y fin de la disposición.

Para más información, consulta [Filtrar la lista de tableros bajo disposición](21-search-filter-or-sort-list-of-boards-under-disposition.md).
