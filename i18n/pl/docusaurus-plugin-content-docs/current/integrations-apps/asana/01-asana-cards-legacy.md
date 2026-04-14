---
title: Karty Asana (Legacy)
article_id: 360039492573
translation_id: 360039492573
locale: pl-pl
sidebar_position: 1
created_at: '2019-11-25T10:03:42Z'
updated_at: '2025-11-25T16:05:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: asana-cards
---

:::warning
Ta strona opisuje naszą starą integrację Asana. W przypadku nowej integracji zapoznaj się z [dokumentacją Asana (wersja beta)](asana).
:::

**Kluczowe funkcje**

- Importuj zadania z Asany na tablice Miro, aby wizualizować postępy zespołu
- Znajdź określone zadania do importu bezpośrednio z Miro, używając filtrów Asany lub wyszukując po nazwie zadania
- Automatyczna synchronizacja: wszystkie zmiany wprowadzone w zadaniach Asany są automatycznie wyświetlane na kartach Asany w Miro

> **Dostępne w**: Starter, Business, Enterprise. *Administratorzy mogą potrzebować autoryzacji korzystania z Asany dla swojego zespołu w Miro. Członkowie zespołu mogą korzystać z aplikacji Asana Cards tylko, jeśli jest ona zainstalowana na poziomie zespołu.*

### Jak zainstalować Asana Cards

1. Najpierw potrzebujesz aktywnego konta Miro oraz Asana. Jeśli nie masz profilu Miro, zarejestruj się [tutaj](https://miro.com/signup/).
2. W Miro Marketplace, otwórz [Asana Cards](https://miro.com/marketplace/asana-cards/?backUrl=%2Fmarketplace%2F)*.* Kliknij przycisk **Pobierz aplikację**.
   Zostaniesz poproszony o wybranie zespołu, w którym chcesz zainstalować Asana. Wybierz zespół i kliknij **Zainstaluj i autoryzuj**.
   > ⚠️ Użytkownicy niebędący administratorami nie mogą zainstalować aplikacji, jeśli jest to niedozwolone w ustawieniach zespołu.

![install_Asana_cards.jpg](../../../../../../docs/integrations-apps/asana/images/21020254087442_install%20Asana%20cards.jpg)
*Autoryzacja kart Asana*

3. Następnym krokiem jest kliknięcie **Połącz** w ustawieniach aplikacji Asana Cards.

![connect_Asana_and_Miro.jpg](../../../../../../docs/integrations-apps/asana/images/21020265147410_connect%20Asana%20and%20Miro.jpg)
*Ustawienia aplikacji Asana Cards w ustawieniach zespołu*
Inni członkowie zespołu znajdą ikonę kart Asana na pasku tworzenia tablicy i będą mogli połączyć swoje konta Asana stamtąd.

![Asana_cards_on_the_toolbar.jpg](../../../../../../docs/integrations-apps/asana/images/21020254085010_Asana%20cards%20on%20the%20toolbar.jpg)
*Karty Asana na pasku narzędzi*

4. Zezwól Asana Connect na dostęp do Twojego konta Asana. Jeśli nie jesteś obecnie zalogowany do aplikacji, zostaniesz poproszony o zalogowanie się do Asany.

**![grant_permission_to_Asana.jpg](../../../../../../docs/integrations-apps/asana/images/21020254090386_grant%20permission%20to%20Asana.jpg)*****Zezwolenie Miro na dostęp do konta Asana***

### Jak importować i używać kart Asana

1. Po połączeniu Miro z Twoim kontem Asana, możesz dodawać karty Asana do swoich tablic Miro. Aby uzyskać wybierak, w pasku tworzenia wybierz **Narzędzia, Multimedia i Integracje** (**+**)**.** Otworzy się panel. Wyszukaj i wybierz karty Asana.
2. Selektor umożliwia filtrowanie zadań. Najpierw wybierz przestrzeń roboczą, a następnie filtruj karty według projektów, tagów lub osób przypisanych. Lista projektów jest sortowana według daty utworzenia.

   > ⚠️ Selektor wyświetli tylko te zadania, do których masz dostęp w Asanie. Jeśli użytkownik Miro otworzy stronę źródłową zadania, do którego nie ma dostępu, zobaczy komunikat o braku dostępu.

   ![Asana_picker.gif](../../../../../../docs/integrations-apps/asana/images/21020254098578_Asana%20picker.gif)
   **Importowanie Kart Asana na tablicę**

Kliknij przycisk **źródło**, aby otworzyć kartę w Asanie.
![go_to_source.jpg](../../../../../../docs/integrations-apps/asana/images/21020265150226_go%20to%20source.jpg)
**Przycisk źródła karty**

Możesz swobodnie dodawać swoje karty z Asany do [kanbanów](../../using-miro/advanced-tools/02-columns-formerly-kanban.md) i [map historyjek użytkownika](../../using-miro/advanced-tools/07-user-story-mapping.md), po prostu przeciągając je.

:::warning
Choć na razie nie ma opcji tworzenia lub edycji kart Asana po stronie Miro, wszystkie zmiany dokonane po stronie Asana są synchronizowane w Miro (proszę pamiętać, że może wystąpić niewielkie opóźnienie w aktualizacji karty).
:::

![Asana_cards_and_kanban.gif](../../../../../../docs/integrations-apps/asana/images/21020254093074_Asana%20cards%20and%20kanban.gif)
*Dodawanie kart Asana do kanban*

### Zmiana koloru karty

Aby zmienić kolor karty, kliknij kartę lub karty i wybierz **kolor wypełnienia** z menu kontekstowego. Jeśli zduplikujesz kartę, nowy kolor zostanie zastosowany. ![asana_card_color.png](../../../../../../docs/integrations-apps/asana/images/21020254100242_asana_card_color.png)
*Zmiana koloru wypełnienia karty*

### Jak odinstalować karty Asana

Aby odinstalować karty Asana na poziomie zespołu, otwórz Ustawienia zespołu **> Aplikacje & Integracje > Karty Asana**, przewiń w dół i kliknij **Odinstaluj dla zespołu.**

**Jeśli chcesz odinstalować aplikację na poziomie indywidualnym, kliknij** **Odinstaluj dla mnie.**

![uninstall_Asna_Cards.jpg](../../../../../../docs/integrations-apps/asana/images/21020265153426_uninstall%20Asna%20Cards.jpg)
*Odinstalowywanie kart Asana*

### Często zadawane pytania

1. *Jakie adresy IP powinny być na liście dozwolonych dla Asana Cards?*
   *-*18.203.61.162, 54.220.74.201, 54.216.81.236, 54.73.153.141, 52.215.228.26, 52.16.47.17, 54.217.180.21.
