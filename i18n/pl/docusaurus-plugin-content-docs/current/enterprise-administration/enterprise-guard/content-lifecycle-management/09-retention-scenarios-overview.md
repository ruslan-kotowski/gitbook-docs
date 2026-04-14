---
title: "Przegl\u0105d scenariuszy retencji"
article_id: 19205103343506
translation_id: 19205103343506
locale: pl-pl
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

## Tablica jest przeniesiona do kosza w okresie retencji

**Zasady retencji mają pierwszeństwo przed zasadami kosza.** Jeśli tablica objęta retencją zostanie przeniesiona do kosza w początkowej lub środkowej fazie okresu retencji, pozostaje w koszu przez czas określony w Zasadzie Kosza (domyślnie 90 dni). Po tym czasie tablica nie będzie już widoczna w koszu. Tablica będzie jednak istnieć i zostanie zachowana do momentu zakończenia okresu retencji, po którym zostanie automatycznie usunięta. Rysunek 1 ilustruje ten scenariusz.

![Figure 1: Board is trashed during retention period](images/28839393875090_board_trashed_during_retention_period.png)*Rysunek 1: Tablica jest przeniesiona do kosza w okresie retencji*

## Tablica jest przeniesiona do kosza, gdy zbliża się koniec okresu retencji

**Zasada kosza pozostaje aktywna po zakończeniu okresu retencji.** Jeśli tablica objęta retencją zostanie przeniesiona do kosza, gdy zbliża się koniec okresu retencji, pozostaje w koszu przez czas określony w zasadzie kosza (domyślnie 90 dni). Po tym czasie tablica nie będzie już widoczna w koszu. Po zakończeniu okresu retencji tablica może zostać trwale usunięta ręcznie i zostanie automatycznie usunięta po zakończeniu Zasady Kosza. Rysunek 2 ilustruje ten scenariusz.

![Figure 2: Tablica jest przeniesiona do kosza, gdy kończy się okres retencji](images/28839361914514_board_trashed_when_retention_period_is_ending.png)*Rysunek 2: Tablica jest przeniesiona do kosza, gdy kończy się okres retencji*

## Zespół jest przeniesiony do kosza podczas okresu retencji

**Kiedy zespół zostanie trwale usunięty, wszystkie tablice należące do zespołu zostaną trwale usunięte.** Kiedy zespół zostanie przeniesiony do kosza, wszystkie tablice należące do tego zespołu zostaną trwale usunięte po 90 dniach, w tym tablice objęte zasadą retencji. Jeśli zespół przeniesiony do kosza zostanie trwale usunięty ręcznie przez administratora, wynik jest ten sam: wszystkie tablice należące do zespołu zostaną trwale usunięte, nawet jeśli te tablice są objęte retencją. Rysunek 3 ilustruje ten scenariusz.

![Rysunek 3: Zespół jest przeniesiony do kosza podczas okresu retencji](images/28839361916434_team_trashed_during_retention_period.png)*Rysunek 3: Zespół przeniesiony do kosza podczas okresu retencji*
