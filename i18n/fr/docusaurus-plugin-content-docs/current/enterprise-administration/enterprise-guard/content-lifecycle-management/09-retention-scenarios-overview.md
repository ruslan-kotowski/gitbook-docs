---
title: "Aper\xE7u des sc\xE9narios de conservation"
article_id: 19205103343506
translation_id: 19205103343506
locale: fr
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

## Le tableau est mis à la corbeille pendant la période de conservation

**Les politiques de conservation l’emportent sur les politiques de gestion de la corbeille.** Si un tableau en cours de conservation est déplacé vers la corbeille pendant la phase initiale ou intermédiaire de sa période de conservation, le tableau reste dans la corbeille pendant la durée configurée dans la politique de mise à la corbeille (90 jours par défaut). Après cette durée, le tableau n’apparaît plus dans la corbeille. Toutefois, le tableau persiste et est conservé jusqu’à la fin de la période de conservation, après quoi le tableau est automatiquement purgé. La figure 1 illustre ce scénario.

![Figure 1: Board is trashed during retention period](images/21019694920466_board_trashed_during_retention_period.png)*Figure 1 : Le tableau est mis à la corbeille pendant la période de conservation*

## Les tableaux sont mis à la corbeille à la fin de la période de conservation.

**La politique de la corbeille reste active après la fin de la période de conservation.** Si un tableau en cours de conservation est déplacé vers la corbeille à la fin de la période de conservation, le tableau reste dans la corbeille pendant la durée configurée dans la politique de gestion de la corbeille (90 jours par défaut). Après cette durée, le tableau n’apparaît plus dans la corbeille. À l’issue de la période de conservation, le tableau peut être définitivement supprimé manuellement et est automatiquement purgé à la fin de la politique de gestion de la corbeille. La figure 2 illustre ce scénario.

![Figure 2: Le tableau est mis à la corbeille lorsque la période de conservation se termine](images/21019694924306_board_trashed_when_retention_period_is_ending.png)*Figure 2 : Le tableau est mis à la corbeille lorsque la période de conservation se termine*

## L’équipe est mise à la corbeille pendant la période de conservation.

**Lorsqu'une équipe est purgée, tous les tableaux appartenant à cette équipe sont définitivement supprimés.** Lorsqu’une équipe est mise à la corbeille, tous les tableaux appartenant à cette équipe sont définitivement supprimés au bout de 90 jours, y compris les tableaux faisant l’objet d’une politique de conservation. Si une équipe corbeille est définitivement supprimée manuellement par un admin, le même résultat s’applique, tous les tableaux appartenant à l’équipe sont définitivement supprimés, même si ces tableaux sont en cours de conservation. La figure 3 illustre ce scénario.

![Figure 3: L’équipe est mise à la corbeille pendant la période de conservation](images/21019706054034_team_trashed_during_retention_period.png)*Figure 3 : L’équipe est mise à la corbeille pendant la période de conservation*
