---
title: Gestionar anuncios del admin
article_id: 31013703080722
translation_id: 31013754574354
locale: es
sidebar_position: 6
created_at: '2025-11-12T21:54:08Z'
updated_at: '2026-03-19T07:59:12Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: in-app-notifications
---

Usa la página de anuncios para ver todos los anuncios, realizar un seguimiento de su estado y gestionarlos a lo largo de su ciclo de vida.

## Ver y comprender los anuncios

Ve a **Consola de administración > Organización > Anuncios**. La tabla de anuncios proporciona una visión general de todos los anuncios, incluidos su nombre, estado, fechas, audiencia y creador.

## Estados de los anuncios

| Estado | Descripción |
| --- | --- |
| **Borrador** | Guardado pero no publicado aún. |
| **Programado** | Publicado y programado para aparecer en una fecha futura. |
| **En vivo** | Actualmente visible para los usuarios. |
| **Finalizado** | Ya no está activo después de la fecha final. |
| **Cancelado** | Detenido antes de la fecha de inicio. |

## Actualizar anuncios

### Editar un anuncio

1. Ve a **Anuncios**.
2. Selecciona el anuncio.
3. Haz clic en **Editar**.
4. Actualiza los detalles del anuncio.
   Puedes actualizar el mensaje, el texto del enlace, la URL del enlace, el público, el horario o la prioridad.
5. Haz clic en **Publicar**.
   Los cambios se aplican de inmediato, incluso para los anuncios en vivo.

### Publicar un anuncio

1. Abre el anuncio.
2. Revisa los detalles.
3. Haz clic en **Publicar**.
   El anuncio se vuelve **Programado** si la fecha de inicio es en el futuro, o **En vivo** si la fecha de inicio es actual o pasada.

## Reutilizar anuncios

### Duplicar un anuncio

1. En la lista de anuncios, abre el menú de **Acciones**.
2. Haz clic en **Duplicar**.
3. Actualiza los detalles del anuncio.
   Cambia el nombre, las fechas, la audiencia u otros campos según sea necesario.
4. Haz clic en **Guardar borrador** o **Publicar**.
   **Guardar borrador** almacena el anuncio sin publicarlo.
   **Publicar** hace que el anuncio esté activo o lo programa según las fechas seleccionadas.

## Controlar el ciclo de vida del anuncio

### Cancelar un anuncio

1. En la lista de anuncios, abre el menú de **Acciones**.
2. Haz clic en **Cancelar**.

Puedes cancelar un anuncio en cualquier estado. El anuncio ya no se muestra a los usuarios.

### Eliminar un anuncio

1. En la lista de anuncios, abre el menú de **Acciones**.
2. Haz clic en **Eliminar**.

El anuncio se elimina permanentemente y no se puede recuperar.

## Monitorear cambios

Cada anuncio incluye una sección de historial que muestra los eventos de su ciclo de vida y actualizaciones.

El historial incluye acciones como:

- Creado
- Publicado o en vivo
- Editado
- Cancelado

Estas acciones también se registran en los registros de auditoría.
