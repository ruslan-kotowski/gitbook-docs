---
title: CA Agile Central (Rally)
article_id: 360017731133
translation_id: 360017731133
locale: de
sidebar_position: 4
created_at: '2019-02-11T10:13:34Z'
updated_at: '2025-11-25T16:02:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: rally-cards
---

Nutze die Vorteile der führenden agilen Software und Methodik von CA direkt auf dem Board. Wandle deine CA Agile Central-Aufgaben in praktische Karten um und genieße Backlog-Priorisierung, Story Mapping und andere Teamaktivitäten, die deinem Team stets weiterhelfen und die Entwicklung hochwertiger Projekte beschleunigen.

> **Erhältlich für:** [Enterprise-Preisplan](../../plans-billing/miro-plans/04-enterprise-plan.md)

## CA Agile verbinden

Die Autorisierung von CA Agile erfolgt über das OAuth 2.0-Protokoll (Authorization Code Grant) und alle Anfragen laufen über SSL. Es gibt zwei Ebenen, um deine Miro-Daten mit deinem CA Agile Central-Konto zu verknüpfen: Nutzerprofilebene und Teamebene.

Es ist wichtig zu wissen, dass die Verbindung zu CA Agile nur in eine Richtung erfolgt: CA Agile --> Miro. Du kannst die Karten in ein Miro-Board importieren und sie über die Schaltfläche „Quelle“ bearbeiten, die unten im Abschnitt Karten bearbeiten beschrieben wird. Du kannst CA Agile-Karten nicht direkt in Miro bearbeiten.

### Teamebene

> **Einrichtung durch:** Team-Admins

:::warning
Bitte beachte, dass du für jedes Team in Miro unterschiedliche Rally-Nutzerkonten zur Verknüpfung mit derselben Rally-Instanz verwenden musst.
:::

Um die Verknüpfung auf Teamebene herzustellen, muss der Team-Admin die App **CA Agile** im [Miro Marketplace](https://miro.com/marketplace/) suchen und sie für das Team installieren: Klicke auf **App installieren**, wähle dann ein Team aus und klicke auf **Installieren & autorisieren**.

![install_Rally_for_a_team.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416392594_install%20Rally%20for%20a%20team.jpg)
*Rally für ein Team installieren*

Du kannst die App auch von einem Board aus installieren:

1. Wähle dazu in der Erstellungsleiste die Option **Tools, Medien und Integrationen** (**+**) aus.Das Panel **Tools, Medien und Integrationen** wird geöffnet.
2. Suche im Tab **Tools** nach CA Agile und wähle es aus.
   Das Panel **CA Agile** wird geöffnet.

![ca-agile-entry-point.png](../../../../../../docs/integrations-apps/more-integrations/images/21537455155858_ca-agile-entry-point.png)
*Die App von einem Board aus installieren*

Öffne dann die **Teameinstellungen > Apps & Integrationen** und **verknüpfe** die Integration von dort. Falls du in Rally nicht autorisiert bist, wirst du aufgefordert, dich bei deinem Rally-Konto einzuloggen.

![connect_Rally.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416393874_connect%20Rally.jpg)
*Die Integration auf Teamebene verknüpfen*

Während dieser Einrichtung wird auf der Seite von Rally ein Webhook erstellt, der dann Updates für importierte Karten an Miro sendet.

Sobald die Integration auf Teamebene eingerichtet ist, kann jedes Teammitglied die von anderen Teilnehmern importierten Rally-Karten auf den Boards und den aktuellen Status der Karten sehen.

Bitte beachte, dass das Rally-Konto, das für die Einrichtung der Integration auf Teamebene verwendet wird, Zugriff auf alle Rally-Projekte haben muss, aus denen die Karten importiert werden. Sollte irgendein Rally-Projekt für dieses Rally-Konto nicht zugänglich sein, werden die aus solch einem Projekt importierten Karten nicht auf dem Board aktualisiert und für alle Nutzer des Teams als eingefroren angezeigt.

### Profilebene

> **Einrichtung durch:** jeden Nutzer

:::warning
Bevor du die Integration verknüpfst, musst du dich in einem separaten Browsertab bei Rally einloggen.
:::

Wenn eine Person wünscht, dass sie Rally-Karten eigenständig in das Board importieren kann, muss sie die Integration auch auf Profilebene konfigurieren. Um dein Miro-Profil zu verknüpfen, musst du die [Profileinstellungen](https://miro.com/app/account/profile/) öffnen, zu den **Integrationen** gehen, **CA Agile Central (Rally)** suchen und auf **Verknüpfen** klicken:

![connect_Rally_on_profile_level.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017429433746_connect%20Rally%20on%20profile%20level.jpg)
*Die Integration auf Profilebene verknüpfen*

Wenn die Verknüpfung auf Profilebene hergestellt ist, kann der Nutzer das Rally-Symbol in seiner Symbolleiste verwenden und die Auswahl der Rally-Bibliothek öffnen. Dort kann der Nutzer alle für das Rally-Konto verfügbaren Rally-Elemente (User Storys, Aufgaben, Fehler) sehen, die für die Einrichtung der Integration auf Profilebene verwendet wurden. Das bedeutet, dass der Nutzer mit der Rally-Auswahl nur die Elemente importieren kann, die ihm in Rally zur Verfügung stehen.

## CA Agile-Karten zum Board hinzufügen

Um eine Karte auf dem Board hinzuzufügen, musst du lediglich die URL-Adresse der Aufgabe kopieren und sie auf dem Board einfügen (dies geht auch über die üblichen [Tastenkombinationen](https://help.realtimeboard.com/support/solutions/articles/1000206698-shortcuts-hotkeys)).

Um Aufgaben zu filtern oder Karten als Massenaktion hinzuzufügen, wähle **CA Agile**in der Erstellungssymbolleiste aus.

Du siehst die Auswahl von CA Agile Central, in der du die Suchfilter wie Projekt, Typ, Iteration, Release usw. festlegen kannst. Wähle eine oder mehrere aus und klicke auf **Exportieren**:

![Rally_picker.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416397714_Rally%20picker.jpg)
*CA Agile Central-Auswahl*

Die Aufgaben werden automatisch zum Board hinzugefügt. Falls der Aufgabenname lang ist, ziehe an der Unterseite der Karte, um ihn vollständig anzuzeigen.

*![Rally_cards_on_the_board.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416398482_Rally%20cards%20on%20the%20board.jpg)
Rally-Karten auf dem Board*

> Beachte, dass die Rally-Integration von Miro nicht die Möglichkeit bietet, Rally-Karten in Miro zu erstellen oder dort zu bearbeiten.

## Karten bearbeiten

Klicke zum Bearbeiten der Karteninhalte bitte auf den Quelllink auf der Karte:

![Rally_card_source.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416398866_Rally%20card%20source.jpg)
*Das Bearbeitungssymbol auf der Karte*

Die Quellaufgabe wird in einem neuen Tab geöffnet, in dem sie bearbeitet werden kann. Alle Änderungen werden sofort für die Karte übernommen.

## Die Integration deaktivieren

Um die Verknüpfung mit deinen Rally-Iterationen aufzuheben, musst du die Integration in den **Teameinstellungen > Apps & Integrationen** **Deaktivieren** und **Deinstallieren**.

![uninstall_Rally.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017429436562_uninstall%20Rally.jpg)
*Die Option zum Deaktivieren der Integration*

## Mögliche Probleme und wie man sie löst

1. *Die Miro-Rally-Auswahl zeigt einige meiner Projekte nicht an*
   - Unsere Rally-Integration verwendet die [Rally-SDK-Auswahl](https://rally1.rallydev.com/docs/saas/apps/2.1/doc/index.html#!/api/Rally.ui.picker.project.ProjectPicker), um die Daten auszufüllen. Er funktioniert nur mit Open-State-Projekten und ist leider nicht anpassbar. Um ein Projekt in Miro anzuzeigen, ändere den Status des Projekts auf „Open“.
2. *Die Updates für die Karten oder die Felder einiger Karten werden nicht an Miro übermittelt*- Wenn du die Integration für Rally-Karten mit mehreren Miro-Teams verwendest, überprüfe bitte, ob alle Teams mit deiner Rally-Instanz über ein *anderes* Rally-Nutzerkonto verknüpft sind. Es ist möglich, dass das Aktualisierungsproblem in dem jeweiligen Team auftritt, weil die Anmeldedaten für die Verknüpfung bereits in einem anderen Miro-Team verwendet werden. Verknüpfe die Integration erneut und verwende dabei ggf. andere Rally-Nutzeranmeldedaten.
3. *Endloses Laden, wenn ich versuche, die Rally-Auswahl in Miro zu öffnen.*- Befolge die unten aufgeführten Schritte zur Fehlerbehebung.

   1. Öffne das Abo-Menü (`https://rally1.rallydev.com/#/subscription`).

   2. Klicke auf das Dropdown-Menü **Aktionen** und wähle **Bearbeiten** aus.

   3. Scrolle nach unten zum Feld **CORS Allowed Origins**.

   4. Gib `https://miro.com,https://*.miro.com` (`http://miro.com`) in das Feld ein.

   5. Klicke auf **Speichern und schließen**.
