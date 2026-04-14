---
title: "C\xF3mo restaurar contenido a un tablero"
article_id: 360019838260
translation_id: 360019838260
locale: es
sidebar_position: 18
created_at: '2021-02-24T08:56:24Z'
updated_at: '2026-01-06T19:00:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: delete-board
---

Con la función de restauración de contenido del tablero puedes estar seguro de que la eliminación accidental de contenidos no será un obstáculo para la productividad de tu equipo. Los editores de tableros pueden restaurar fácilmente los objetos recientemente borrados de sus tableros.

> **Configurado por:** editores que fueron invitados explícitamente al tablero [mediante email](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) o que tengan acceso al tablero porque forman parte de un [proyecto](../sharing-boards/16-projects.md) o [equipo](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) en Miro
> **Disponible en:** versión para navegador, [aplicación de escritorio](../../getting-started/apps-for-devices/05-desktop-app.md), [aplicación para tabletas](../../getting-started/apps-for-devices/11-tablet-app.md)

> **⚠️**La función no está disponible para v[isitantes.](../sharing-boards/08-collaboration-with-visitors.md)

> Consulta e[sta guía](../managing-boards/12-board-history-versions.md) para aprender a restaurar una versión de un tablero.

### ¿Qué contenido se puede restaurar?

- Cualquier contenido eliminado del tablero durante la sesión activa actual o, en caso de que se haya finalizado la sesión, hasta 30 minutos después de que el contenido haya sido eliminado
- Los últimos 1000 objetos eliminados del tablero, si la restauración se produce más de 30 minutos después de que se haya eliminado el contenido
- Cualquier contenido eliminado del tablero si los objetos fueron seleccionados y eliminados simultáneamente por un período de tiempo indefinido, hasta que se eliminen los próximos 1000 objetos

### Cómo restaurar contenidos

Para restaurar objetos eliminados, haz lo siguiente:

1. Haz clic en el icono de **Open sidebar (abrir barra lateral)** ubicado en la esquina inferior izquierda.
2. En la vista general abierta del tablero, haz clic en el icono de **Board history (historial del tablero)**.
3. Haz clic en el icono **Restore (restaurar)** sobre cualquier objeto que desees recuperar.  Los objetos eliminados reaparecerán en el tablero (exactamente donde estaban antes de ser eliminados) y la vista hará un zoom sobre esa parte del tablero.

restore_board_content_restore_feature.jpg
Cómo restaurar un objeto eliminado

### Limitaciones

> **⚠️** Ten en cuenta que habrá casos límite cuando:

- el contenido se restaure a otra parte del tablero (por ejemplo, cuando se restaure una [línea](../essential-tools/05-connection-lines.md) de conexión y la [nota adhesiva](../essential-tools/14-sticky-notes.md) a la que esta haya estado pegada haya sido reposicionada en el tablero)
- el contenido perderá su conexión con el objeto al que estaba vinculado inicialmente (por ejemplo, cuando se elimina una [tarjeta](../essential-tools/02-cards.md) de una tabla y luego se restaura, la tarjeta se restaurará a la misma parte del tablero pero ya no estará ligada a la [tabla](../advanced-tools/05-grid.md))
- algunos contenidos no se restaurarán. Las limitaciones actuales incluyen:

- [Líneas](../essential-tools/05-connection-lines.md) que estuvieron conectadas a objetos eliminados del tablero más tarde
- texto de una celda de una tabla, si este se eliminó de la tabla (si la tabla se eliminó junto con el texto, sí se restaurará)
- [mapa de la historia de usuario](../advanced-tools/07-user-story-mapping.md) (tanto el marco como las tarjetas)
- [comentarios](../facilitation-tools/asynchronous-tools/01-comments.md) borrados por separado

  ![mceclip0.png](../../../../../../docs/using-miro/working-on-the-board/images/21017605949842_mceclip0.png)
  *El banner que aparece si no se ha restaurado algún contenido*

Como regla general, si los objetos fueron eliminados y luego restaurados simultáneamente, todos los enlaces dentro de ese lote también se restaurarán, pero existe la posibilidad de que no se restauren los enlaces a objetos externos al tablero.

Ten en cuenta que [los tableros duplicados](../managing-boards/03-how-to-duplicate-a-board.md) no admiten la opción de restaurar objetos que se hayan eliminado en el tablero original.

### Preguntas frecuentes

1. *Mi contenido desapareció pero no veo la opción de restaurar objetos eliminados.*  ¿Qué hago?
   - Ten en cuenta que algunos contenidos no se pueden restaurar (consulta las limitaciones anteriores). Si tu contenido incluía otros tipos de widgets, por favor: /span>
   - asegúrate de haber abierto el tablero correcto
   - revisa tu lista de [plantillas personalizadas](../../getting-started/start-here/your-first-board/02-custom-templates.md) con nombres similares
   - Revisa el [minimapa](21-work-smarter-not-harder.md#utilizar-minimapa) del tablero para ver si hay contenido en diferentes partes del tablero
   - si tienes varios perfiles de Miro, asegúrate de estar autorizado bajo la dirección de correo electrónico correcta.
