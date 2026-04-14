---
title: "Visi\xF3n general de los escenarios de retenci\xF3n"
article_id: 19205103343506
translation_id: 19205103343506
locale: es
sidebar_position: 9
created_at: '2024-05-28T17:58:22Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

## El tablero se mueve a la papelera durante el periodo de retención

**Las políticas de retención anulan las políticas de papelera.** Si un tablero bajo retención se mueve a la papelera durante la fase inicial o media de su periodo de retención, el tablero permanece en la papelera durante el tiempo configurado en la política de papelera (por defecto 90 días). Después de esta duración, el tablero ya no aparece en la papelera. Sin embargo, el tablero persistirá y se conservará hasta que finalice el periodo de retención, y luego el tablero se eliminará automáticamente. La figura 1 ilustra este escenario.

![Figure 1: Board is trashed during retention period](images/21019706035218_board_trashed_during_retention_period.png)*Figura 1: El tablero se mueve a la papelera durante el periodo de retención*

## El tablero se mueve a la papelera cuando termina el periodo de retención

**La política de papelera permanece activa una vez finalizado el periodo de retención.** Si un tablero bajo retención se mueve a la papelera cuando el periodo de retención está finalizando, el tablero permanece en la papelera durante el tiempo configurado en la política de papelera (por defecto 90 días). Después de esta duración, el tablero ya no aparece en la papelera. Una vez finalizado el periodo de retención, el tablero puede borrarse permanentemente de forma manual y se elimina automáticamente cuando finaliza la política de papelera. La Figura 2 ilustra este escenario.

![Figure 2: El tablero se mueve a la papelera cuando finaliza el periodo de retención](images/21019706040978_board_trashed_when_retention_period_is_ending.png)*Figura 2: El tablero se mueve a la papelera cuando termina el periodo de retención*

## El equipo se mueve a la papelera durante el periodo de retención

**Cuando se borra un equipo, todos los tableros que pertenecen a un equipo se eliminan permanentemente.** Cuando un equipo se mueve a la papelera, todos los tableros pertenecientes a ese equipo se eliminan permanentemente después de 90 días, incluidos los tableros que tienen una política de retención. Si un admin elimina manualmente de forma permanente un equipo de la papelera, se aplica el mismo resultado: todos los tableros pertenecientes al equipo se eliminan permanentemente aunque esos tableros estén bajo retención. La figura 3 ilustra este escenario.

![Figura 3: El equipo se mueve a la papelera durante el periodo de retención](images/21019706042514_team_trashed_during_retention_period.png)*Figura 3: El equipo se mueve a la papelera durante el periodo de retención*
