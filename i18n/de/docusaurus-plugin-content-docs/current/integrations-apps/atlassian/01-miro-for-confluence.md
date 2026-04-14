---
title: Miro für Confluence
article_id: 360020712594
translation_id: 7626017610258
locale: de
sidebar_position: 3
created_at: '2022-09-14T08:42:35Z'
updated_at: '2026-03-12T09:15:25Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
availability:
  notes: 'Verfügbar für: Alle Miro-Preispläne; Confluence Cloud (in Miro einbetten),
    Confluence Cloud/Server/DC (in Confluence einbetten) Wer kann das: Confluence-Admin'
---

Miro und Confluence arbeiten mit einer Zwei-Wege-Synchronisierung zusammen, um sicherzustellen, dass du die aktuellsten Inhalte von beiden Plattformen erhältst, egal auf welcher du arbeitest.

## So funktioniert Miro mit Confluence

Du kannst deine Miro-Boards und Confluence-Dokumente einbetten und durch die sofortige Synchronisierung alle Änderungen nachverfolgen. Du kannst die Zugriffsebenen für die Einbettung so festlegen, dass die entsprechenden Nutzer jederzeit auf alle nötigen Informationen zugreifen können.

Confluence-Dokumente in Miro-Boards einbetten

Miro-Boards in Confluence-Dokumente einbetten

## Confluence-Dokumente in Miro-Boards einbetten

Du kannst Confluence-Dokumente in Miro einbetten, indem du einfach einen Link in das Miro-Board einfügst. Beachte, dass **du zum Einbetten von Confluence-Dokumenten in Miro die Confluence Cloud benötigst.**

Wenn du einen Confluence-Link zu einem Miro-Board hinzufügst, erscheint er als [Miro-Smart-Link](https://help.miro.com/hc/articles/360017730993). Wenn du zum ersten Mal einen Confluence-Link einfügst, musst du auf **Verbinden** klicken, um den Confluence-Zugriff zu autorisieren.

:::warning
Aus Sicherheitsgründen werden die Details eines Confluence-Links nicht auf öffentlichen Miro-Boards angezeigt, und die Nutzer können auf privaten Boards nur den Titel eines Confluence-Links sehen. Den Titel der Seite sehen sie nur, wenn sie ihr Confluence-Konto autorisieren. Danach können sie das Confluence-Dokument erweitern und bearbeiten (abhängig von den bereitgestellten Zugriffsebenen).
:::

![Connect_Confluence.png](../../../../../../docs/integrations-apps/atlassian/images/21019693898258_Connect%20Confluence.png)*Die Confluence-Seite in Miro verknüpfen*

Sobald Confluence autorisiert wurde, können Nutzer, die auf das Board zugreifen, den Dokumenttitel, das Symbol des Anbieters und die Linkquelle sehen. Außerdem kann man den Miro Smart Link in den Vollbildmodus erweitern.

:::tip
Die Titel von Miro Smart Links werden aus der URL extrahiert. Wenn du den Titel des Confluence-Dokuments bearbeitest, musst du den Link erneut einfügen, um den aktualisierten Titel in deinem Miro Smart Link zu sehen.
:::

![Connected_Confluence_card.png](../../../../../../docs/integrations-apps/atlassian/images/21019704985746_Connected%20Confluence%20card.png)*Eine verknüpfte Confluence-Seite als Miro Smart Link*

Wenn Nutzer auf das Erweiterungssymbol klicken, werden sie aufgefordert, ihr eigenes Confluence-Konto zu autorisieren, bevor sie das Dokument in Miro ansehen und bearbeiten können.

![Expanded_Confluence_card.png](../../../../../../docs/integrations-apps/atlassian/images/21019693877138_Expanded%20Confluence%20card.png)*Das erweiterte Confluence-Dokument*

## Miro-Boards in Confluence-Dokumente einbetten

Du kannst Miro-Boards in Confluence-Dokumente einbetten mit dem Miro Plugin für Confluence oder direkt über Atlassian Smart Links. Dies kann mit der Confluence Cloud, dem Server oder dem DC erfolgen.

### Schritt 1: Das Miro-Plugin einrichten

Installiere zuerst die [App „Miro for Confluence“](https://marketplace.atlassian.com/apps/1217530/miro-for-confluence?tab=reviews&hosting=cloud) aus dem Atlassian Marketplace.

**So installierst du die App „Miro for Confluence“**

> **Wer kann es tun**: Confluence Admin

1. Melde dich als Admin bei deiner Confluence-Instanz an
2. Klicke auf das Admin-Dropdown und wähle **Add-ons (Apps)**
3. Wähle **Neue Apps suchen** oder **Neue Add-ons suchen**
4. Suche nach **Miro for Confluence**
5. Klicke auf **App holen**

![Miro_for_Confluence.png](../../../../../../docs/integrations-apps/atlassian/images/21019704969490_Miro%20for%20Confluence.png)*Die App „Miro for Confluence“*

Du siehst die folgende Meldung, wenn die App erfolgreich installiert wurde:

![success_message.jpg](../../../../../../docs/integrations-apps/atlassian/images/21019693910290_6bad2c9b-0232-4306-8596-b302e902d548.png)
*Die App wurde erfolgreich installiert*

### Schritt 2: Ein Board auf der Confluence-Seite einbetten

Es gibt drei Möglichkeiten, ein Miro-Board in eine Confluence-Seite einzubetten:

1. Indem du **/miro** direkt im Confluence-Dokument eingibst.
   ![Typing_miro_on_the_doc.png](../../../../../../docs/integrations-apps/atlassian/images/21019704972946_Typing%20miro%20on%20the%20doc.png)
   */miro auf der Confluence-Seite eingeben, um ein Board einzubetten*
2. Indem du in der App-Symbolleiste nach Miro suchst. Im Confluence-Dokument klicke auf **Einfügen** und wähle **Miro** aus der Liste der Apps aus.
   ![Miro_plugin.jpg](../../../../../../docs/integrations-apps/atlassian/images/21019693873682_Miro%20plugin.jpg)
   *Miro aus der App-Liste auswählen, um ein Board einzubetten*
3. Indem du einen Miro-Link mit Atlassian Smart Links direkt in Confluence einfügst.

### Schritt 3: Wähle ein Board aus der Board-Auswahl aus

Die Board-Auswahl wird geöffnet. Wähle das Board, das du einbetten möchtest, aus dem Dropdown-Menü aus oder suche nach einem Board. Nutzer sehen nur die Boards, die ihnen in Miro zur Verfügung stehen, und können Boards nur einbetten, wenn sie Bearbeitungszugriff haben.

![Board_picker.png](../../../../../../docs/integrations-apps/atlassian/images/21019693889298_Board%20picker.png)*Ein einzubettendes Board aus der Board-Auswahl auswählen*

Wähle die **Startansicht** für das eingebettete Board aus.

![Set-the-starting-view-for-your-embed.png](../../../../../../docs/integrations-apps/atlassian/images/21019693917842_Set-the-starting-view-for-your-embed.png)*Festlegen der Startansicht für das eingebettete Miro-Board*

Wähle die Zugriffsebene für **alle Besuchenden** der Confluence-Seite aus.

- **Kann ansehen:** Ermöglicht jedem Besuchenden auf der Confluence-Seite, das Board zu sehen.
- **Zugriff erfordern:** Beschränkt die Anzeige auf diejenigen, die in Miro Zugriff auf das Board haben.

![Access-level-for-embed.png](../../../../../../docs/integrations-apps/atlassian/images/21019693915666_Access-level-for-embed.png)*Festlegen der Zugriffsebene für das Miro-Board auf der Confluence-Seite*

### Schritt 4: Das Board einbetten

Sobald du auf **Board einbetten** klickst, wird das Miro-Board als iFrame auf der Confluence-Seite eingefügt. Nutzer können das Board ansehen und sich darin bewegen.

:::note
Für Nutzer im Enterprise-Preisplan gelten die Zugriffsebenen gemäß den unternehmensweiten Zugriffseinstellungen, weshalb einige Berechtigungen möglicherweise eingeschränkt sind. Erfahre mehr über die [Verwaltung eingebetteter Boards im Enterprise-Preisplan](https://help.miro.com/hc/articles/4405088016274).
:::

![Miro-board-embedded-in-confluence.png](../../../../../../docs/integrations-apps/atlassian/images/21019705017874_Miro-board-embedded-in-confluence.png)*Miro-Board eingebettet in eine Confluence-Seite*

Um das Board direkt in Miro zu öffnen, klicke auf das Miro-Logo.

![Open-embedded-board-in-miro.png](../../../../../../docs/integrations-apps/atlassian/images/21019693937554_Open-embedded-board-in-miro.png)
*Die Option, das Board in Miro zu öffnen*

#### **Nutzererfahrung in Confluence Cloud vs. Confluence Server**

Das Menü für die Fenstergröße für eingebettete Boards ist für Confluence Cloud und Confluence Server unterschiedlich.

In der Confluence Cloud siehst du das folgende Menü für die Fenstergröße mit der Option **In voller Breite**:

![Go-full-width-Miro-board-confluence.png](../../../../../../docs/integrations-apps/atlassian/images/21019693943826_Go-full-width-Miro-board-confluence.png)
*Fenstergrößenmenü im Confluence-Browser*

Im Confluence Server siehst du ein Menü mit der Option, eine kleine, mittlere oder große Fenstergröße (**S/M/L**) auszuwählen:

![Miro_in_Confluence_Server.jpg](../../../../../../docs/integrations-apps/atlassian/images/21019705005330_832eb85b-5925-4545-8cea-321d3b55d7ed.png)*Menü für Fenstergröße in der Confluence-App*

## Miro-Boards über Atlassian Smart Links einbetten

Mit der Atlassian Smart-Link-Funktion kannst du Miro-Boards auch in Confluence einbetten. Die Funktion ermöglicht es, ein Board automatisch einzubetten, ohne dass eine App installiert werden muss.

Gehe zu einer Confluence-Seite und füge einfach einen Board-Link ein oder gebe **/link** ein, um ihn einzufügen. Wenn du die Funktion zum ersten Mal verwendest, wirst du aufgefordert, eine Verbindung zu einem Miro-Team herzustellen. Klicke auf **Eine Verbindung herstellen, um eine Vorschau anzuzeigen**, autorisiere dich in Miro und wähle ein Team aus, aus dem du deine Boards einbetten möchtest.

:::note
Nur Nutzer, die auf der Seite von Miro Zugriff auf das eingebettete Board haben, können mit der eingebetteten Miro-Board-Vorschau arbeiten, nachdem sie ihr Miro- und Atlassian-Konto verknüpft haben. Wenn du die Board-Vorschau für alle Nutzer von Confluence verfügbar machen möchtest, kannst du die Miro-App verwenden.
:::

![install_Atllassian_links.jpg](../../../../../../docs/integrations-apps/atlassian/images/21019693912594_9c4c3ff4-4af4-4f11-a65e-54c796480f6d.png)
*Auswahl eines Teams zum Einbetten der Boards*

Wenn du den Link eines Miro-Boards in eine Confluence-Seite einfügst, wird es automatisch zu einem Widget. Klicke auf den Link, um die Anzeigeoptionen anzuzeigen. Du kannst wählen, ob das Miro-Board als **URL**, **Inline**-Text, als **Karte** oder als **Einbettung** angezeigt wird.

![Confluence_widget.png](../../../../../../docs/integrations-apps/atlassian/images/21019704980370_Confluence%20widget.png)*Miro-Board-Widget in Confluence*

Wenn du dich dafür entscheidest, das Board als Einbettung anzuzeigen, kannst du die Größe der Einbettung durch Ziehen an den Seiten ändern.

![changing_embed_size.gif](../../../../../../docs/integrations-apps/atlassian/images/21019693925394_8d053d95-3d71-4399-8431-3a57638cb095.png)
*Ändern der Miro-Einbettungsgröße in Confluence*

:::warning
Wenn Cookies von Drittanbietern in deinem Browser blockiert sind, kann es unerwartete Probleme bei der Anzeige von eingebetteten Boards geben.
:::

## Die Miro-App für Confluence deaktivieren

Um die App zu deaktivieren, gehe zu **Atlassian Marketplace** > **Apps verwalten** > **Miro für Confluence Cloud** > **Deinstallieren.**

*![Uninstall_Confluence_plugin.jpg](../../../../../../docs/integrations-apps/atlassian/images/21019693930898_f7e12afa-1bca-4da6-8046-0ed55ea8651c.png)*
*Die App „Miro für Confluence“ in der Liste der installierten Atlassian-Apps*

## Migration und Auswirkungen auf Boards in Confluence

Egal, ob du von einer On-Premise- zu einer Cloud-Instanz oder von Cloud zu Cloud migrierst, es sind keine speziellen Migrationsschritte für das Miro-Plugin erforderlich. Confluence zeigt Miro-Boards über iFrames an, die URL-basierte Einbettungen sind, was bedeutet, dass Confluence nur den Board-Link speichert, während das Board in Miro bleibt.
