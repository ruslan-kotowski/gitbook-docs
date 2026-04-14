---
title: "Descripci\xF3n general de los escenarios de eliminaci\xF3n"
article_id: 19596032332434
translation_id: 19596032332434
locale: es
sidebar_position: 6
created_at: '2024-06-17T17:24:29Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

## Movimiento automático de tableros a la Papelera

Los tableros se mueven automáticamente a la Papelera en su fecha de eliminación designada. Si no hay una política de retención activa que afecte al tablero, su eliminación permanente será determinada por la política de papelera.
![disposition1.png](images/21019706093330_disposition1.png)

Por ejemplo, considera un tablero de proyecto que está programado para moverse a la Papelera el 1 de julio de 2025 según la política de eliminación y no hay una política de retención que lo afecte. El tablero se moverá automáticamente a la Papelera el 1 de julio de 2025 y se eliminará permanentemente el 29 de septiembre de 2025 según la política de papelera de 90 días.

:::note
Una política de retención activa reemplaza la política de papelera. Por lo tanto, la fecha de eliminación permanente del tablero seguirá la política de retención vigente.
:::

Si las notificaciones de eliminación están habilitadas para la política, los usuarios recibirán una notificación según el número de días configurado cuando la notificación de eliminación deba enviarse antes del movimiento programado del tablero a la Papelera.

La notificación aparece en el feed de notificaciones de Miro y enlaza directamente al tablero. También se muestra un banner en la parte superior del tablero advirtiendo al usuario sobre la próxima acción de mover a la papelera. oard owners and co-owners have los propietarios y copropietarios del tablero tienen la opción de conservar el tablero.

## Eliminación iniciada por el usuario del tablero

Cuando un propietario del tablero mueve un tablero a la papelera, la política de eliminación ya no afecta el ciclo de vida del tablero. Si no hay políticas de retención activas que apliquen al tablero, su eliminación permanente seguirá la política de papelera.

![disposition2.png](images/21019694962962_disposition2.png)

Por ejemplo, considera un tablero de plan operativo programado para eliminación el 13 de octubre de 2024. Si el propietario del tablero mueve preventivamente el tablero a la papelera el 15 de mayo de 2024, y no hay políticas de retención activas que afecten al tablero, se adherirá a la política de papelera. El tablero se eliminará de forma permanente el 13 de agosto de 2024, según la política de papelera de 90 días.

:::note
Si hay una política de retención activa que afecta al tablero, esta política anulará la política de papelera, estableciendo la fecha de eliminación permanente según la política de retención.
:::

## Restauración iniciada por el usuario del tablero

Cuando un usuario restaura un tablero de la papelera, cualquier política de eliminación relevante se vuelve a aplicar automáticamente. Esto garantiza que el tablero reingrese a su ciclo de vida con todas las configuraciones originales restauradas.

![disposition3.png](images/21019706096530_disposition3.png)

Por ejemplo, si un usuario restaura un tablero de estrategia de marketing de la papelera el 20 de junio de 2024 que anteriormente tenía aplicada una política de eliminación de 1 año, esta política se vuelve a aplicar automáticamente al restaurarlo. La nueva fecha de eliminación del tablero se recalculará desde la fecha de restauración, estableciendo su nueva fecha de eliminación para el 20 de junio de 2025 o un año a partir de la fecha en que este tablero fue modificado por última vez después de la restauración.

## Notificaciones de eliminación

Las notificaciones de eliminación alertan a los usuarios con anticipación cuando un tablero está programado para ser movido automáticamente a la papelera debido a inactividad, basado en una política de eliminación activa.

- Los admins pueden habilitar las notificaciones al publicar una política.
- El momento de la notificación es configurable de 1 a 30 días antes del movimiento programado.
- Las notificaciones se envían según la cantidad de días configurada cuando la notificación de eliminación debe enviarse antes de la fecha de la papelera.

Cuando un tablero entra en el período de inspección:

- Una notificación aparece en el feed de notificaciones del usuario.
- Al hacer clic, se abre el tablero con un banner superior que advierte sobre el próximo movimiento a la papelera.
- Los usuarios pueden elegir conservar el tablero para retenerlo, lo que restablece el temporizador de eliminación.

Este mecanismo de notificación se aplica a todos los escenarios donde:

- Una política de eliminación con notificaciones está activa.
- El tablero está entrando en su período de inspección (según el número de días configurado antes de la fecha de eliminación).

### Escenario 1: Tableros que coinciden con una política de eliminación

Estos tableros están bajo una política y se moverán a la papelera después del periodo de inactividad definido.

Si las notificaciones de eliminación están habilitadas para la política, se enviará una notificación según el número de días configurado cuando la notificación de eliminación deba enviarse antes de la fecha programada para mover el tablero a la papelera. El tablero también mostrará un banner que permitirá a los usuarios revisarlo o conservarlo.

### Escenario 2: Tableros con una etiqueta de clasificación que se añadió después de que el tablero fue modificado por última vez.

Estos tableros se incluyen retroactivamente en el alcance y aún siguen el mismo cronograma de eliminación basado en su última fecha de modificación.

Si las notificaciones de eliminación están habilitadas, los usuarios recibirán una notificación según el número de días configurado cuando la notificación de eliminación deba enviarse antes de la fecha programada para mover el tablero a la papelera, incluso si la etiqueta fue aplicada después de la última edición.

### Escenario 3: Tableros con una etiqueta de clasificación que se eliminó antes de que la política fuera publicada.

Estos tableros ya no están bajo la política y son excluidos de la evaluación de eliminación.

Dado que están fuera del alcance, no se enviarán notificaciones de eliminación.

### Escenario 4: Tableros recientemente modificados y aún no dentro del umbral de eliminación.

Estos tableros han sido editados recientemente y aún no son elegibles para la eliminación.

Solo se enviará una notificación si el tablero entra en el periodo de inspección, es decir, según el número de días configurado cuando la notificación de eliminación debe enviarse antes de la fecha de eliminación. Hasta entonces, no se dispara ninguna notificación.

### Escenario 5: Tableros modificados después de entrar en inspección

Una vez que un tablero entra en el periodo de inspección, su fecha de eliminación queda fijada. Esto significa que, a menos que el propietario del tablero elija explícitamente conservarlo, se moverá automáticamente a la papelera en la fecha programada.

Modificar o acceder al tablero durante el periodo de inspección no afecta el calendario de eliminación. Las siguientes acciones no cambiarán el resultado de la eliminación: editar o ver el tablero, cambiar su etiqueta de clasificación o equipo, e incluso eliminar la política asociada.

Si se habilitan las Notificaciones de Eliminación, se enviará una notificación conforme al número de días configurado cuando se deba enviar la notificación de eliminación antes de la fecha programada para la papelera, y el tablero mostrará un banner que permitirá al usuario revisarlo o conservarlo.

### Escenario 6: Tableros que ya han sido eliminados o movidos manualmente a la papelera

Estos tableros ya han sido eliminados del espacio de trabajo y ya no son gestionados por políticas de eliminación.

No se envían notificaciones de eliminación para los tableros que ya están en la papelera o se han eliminado de forma permanente.

### Escenario 7: Tableros bajo múltiples políticas

Los tableros pueden estar sujetos a más de una política de eliminación activa al mismo tiempo, especialmente si múltiples políticas apuntan a la misma etiqueta de clasificación o equipo.

Si más de una política con notificaciones habilitadas se aplica a un tablero, el usuario recibirá solo una notificación cuando el tablero entre en inspección. La notificación se basa en la política con la fecha de eliminación programada más próxima y se envía según la cantidad de días configurada cuando la notificación de eliminación debe ser enviada antes de esa fecha.

## Escenario 8: Tableros ya en estado de inspección y la política de eliminación se elimina posteriormente

Si un tablero ya ha entrado en el período de inspección y se han enviado las notificaciones de eliminación (si están habilitadas), la fecha de eliminación programada queda fijada. Incluso si la política de eliminación asociada se elimina o modifica más tarde, el tablero aún se moverá automáticamente a la papelera en la fecha de eliminación original, a menos que el propietario del tablero decida conservarlo.

En contraste, si la política se elimina antes de que un tablero entre en el período de inspección, el tablero se considera fuera de alcance y no se moverá a la papelera.
Esto garantiza que una vez que los usuarios han sido notificados, la acción de eliminación se mantenga coherente y predecible, independientemente de los cambios de política realizados después.
