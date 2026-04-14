---
title: Doświadczenie użytkownika podczas przenoszenia danych między regionami
article_id: 25075857856658
translation_id: 25075857856658
locale: pl-pl
sidebar_position: 4
created_at: '2025-03-04T08:51:38Z'
updated_at: '2025-05-09T08:47:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Kto może to zrobić: Wszyscy użytkownicy Jakie wersje: Przedsiębiorstwo Jakie
    platformy: Przeglądarka, aplikacja komputerowa, urządzenia mobilne'
---

Ten artykuł opisuje doświadczenie użytkownika podczas migracji danych między regionami, zarówno dla [automated">zautomatyzowanego](../../canvas-25-admin-features/data-residency/05-move-data-between-regions-–-automated-migration.md), jak i [ręcznego eksportu i importu](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md) danych.

## Doświadczenie użytkownika podczas automatycznej migracji (wersja beta)

W następnych sekcjach opisano, czego można się spodziewać przed, w trakcie i po automatycznym przeniesieniu danych między regionami.

### Przed automatyczną migracją

Dwa tygodnie przed migracją wszyscy użytkownicy w Twojej organizacji Enterprise otrzymują następujące powiadomienia:

- **Baner w produkcie**
  Wyświetla datę migracji i przewidywany czas trwania w lokalnej strefie czasowej
- **Powiadomienie e-mail**
  Opisuje nadchodzącą zaplanowaną konserwację dla wszystkich użytkowników w Twojej organizacji Enterprise

:::note
Jeśli jesteś członkiem wielu kont Miro, to Twoje pozostałe konta pozostają dostępne podczas migracji.
:::

### Podczas automatycznej migracji

Zautomatyzowana migracja wymaga około 8 godzin przestoju.

Podczas automatycznej migracji nie możesz uzyskać dostępu do danych swojej organizacji Enterprise, w tym tablic, zespołów i ustawień.

Pulpit Miro wyświetla powiadomienie, że trwa migracja danych dla Twojej organizacji. Podczas procesu migracji nie będziesz mieć dostępu do tablic organizacji, zespołów ani ustawień.

:::tip
Jeśli jesteś członkiem wielu organizacji, możesz przełączyć się do innej organizacji z poziomu swojego pulpitu i kontynuować korzystanie z Miro.
:::

### Po automatycznej migracji

Po pomyślnym zakończeniu migracji otrzymasz wiadomość e-mail z potwierdzeniem. Na Twoim pulpicie nawigacyjnym Miro pojawia się komunikat potwierdzający pomyślną migrację.

Jeśli migracja nie powiedzie się, otrzymasz powiadomienie e-mail. Możesz nadal korzystać z Miro w regionie UE, logując się ze strony [miro.com](https://miro.com).

### Przekierowanie tablicy po automatycznej migracji

Każda tablica, którą dodałeś do zakładek w poprzednim regionie, automatycznie przekierowuje do nowego regionu i korzysta z zaktualizowanego adresu URL.

## Doświadczenia użytkownika podczas ręcznego eksportu i importu

Użytkownicy muszą ręcznie eksportować kopie zapasowe tablic ze swojego regionu źródłowego i importować je do docelowego regionu.

**Więcej informacji:** Zobacz [Przenoszenie danych między regionami – Ręczny eksport i import](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md).

## Współpraca między regionami

Użytkownicy Miro są regionalni. Aby współpracować z użytkownikami w organizacjach spoza Twojego regionu, musisz mieć profil użytkownika w każdym z tych regionów.

Na przykład, jeśli jesteś użytkownikiem z regionu UE i chcesz współpracować z użytkownikami organizacji z regionu AU, musisz utworzyć oddzielny profil użytkownika na stronie [au.miro.com](https://au.miro.com/).
