---
title: Ein Miro-Board einbetten
article_id: 360016335640
translation_id: 360016335640
locale: de
sidebar_position: 2
created_at: '2020-09-09T07:54:13Z'
updated_at: '2025-09-19T09:07:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: comments
availability:
  notes: 'Personen: Bearbeiter des Boards Preispläne: Alle Preispläne Plattformen:
    Web, Desktop, Mobile'
---

Du kannst jedes Miro-Board oder ein spezifisches Element (Rahmen oder Format) aus dem Board in unterstützten Apps und Webseiten einbetten, sodass dein Team im Kontext arbeiten kann, ohne die Werkzeuge wechseln zu müssen.

Einbettungen übernehmen die [Freigabeeinstellungen](../../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) des Boards:

- **Öffentlicher Link an** — jeder mit dem Link kann das Board ansehen (oder bei kostenpflichtigen und Education-Plänen kommentieren oder bearbeiten).
- **Öffentlicher Link aus** — nur eingeladene Mitwirkende können die Einbettung öffnen, nachdem sie sich angemeldet haben.

[Enterprise-Admins](../../../plans-billing/miro-plans/04-enterprise-plan.md) können die Verfügbarkeit des öffentlichen Links in den [Sicherheitseinstellungen](../../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md) verwalten.

## Wähle deine Methode zum Einbetten

Miro bietet zwei Möglichkeiten, um Boards einzubetten:

- **Mit unterstützten Apps**:

  - Arbeiten auf Plattformen wie Zoom, Teams, Confluence, Jira oder Notion.
  - Native Integrationsfunktionen und nahtlose Workflows erwünscht.
  - Nutzer interagieren hauptsächlich über diese spezifische Plattform.
  - Einfachster Einrichtungsprozess erforderlich.
- **Mit Einbettungscode**:

  - Einbettung in Websites, Blogs oder benutzerdefinierte Plattformen.
  - Arbeiten mit WordPress, Webflow oder anderen Website-Baukästen.
  - Mehr Kontrolle über Größe und Erscheinungsbild erforderlich.
  - Die Plattform unterstützt iFrames, hat aber keine native Miro-Integration.

## Boards in unterstützten Apps einbetten

Miro unterstützt eine Reihe von Apps, in denen du deine Miro-Boards ganz einfach teilen kannst. Unterstützte Apps sind:

- [Zoom](../../../integrations-apps/zoom/02-miro-app-for-zoom-user-guide.md)
- [Webex](../../../integrations-apps/more-integrations/10-miro-for-webex.md)
- [Microsoft Teams](../../../integrations-apps/microsoft/microsoft-teams/02-miro-for-microsoft-teams-user-guide.md)
- [Jira](../../../integrations-apps/atlassian/02-miro-for-jira-cloud.md)
- [Confluence](../../../integrations-apps/atlassian/01-miro-for-confluence.md)
- [Notion](https://miro.com/marketplace/notion-embed/)
- [Coda](https://miro.com/marketplace/coda-embed/)
- [Productboard](https://miro.com/marketplace/productboard-embed/)
- Mittel

Wenn du ein Miro-Board in eine andere App einbettest, kannst du Zugriffsrechte speziell für Nutzer der App festlegen und ihnen erlauben, das Board von der App aus anzusehen, zu kommentieren oder zu bearbeiten. Der Zugriff auf das Board auf der Miro-Seite ist davon nicht betroffen. Erfahre, wie [das Freigeben und die Berechtigungen für eingebettete Boards funktionieren](../../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).

Um ein Board in einer der unterstützten Apps einzubetten:

1. Gib in der Ziel-App **/miro** ein oder wähle **Miro** aus dem Einfügemenü aus.
2. Wähle das Board aus.
3. Wähle die **Startansicht**:
   - **Komplettes Board** — der gesamte Canvas.
   - **Bestimmtes Element**, wie Rahmen oder Format (Dokument, Diagramm, Tabelle, Zeitachse oder Präsentationen).
4. Schalte den **Fokusmodus** ein, um eine ablenkungsfreie Einbettung zu erstellen. Lass ihn ausgeschaltet, um volle Interaktivität zu ermöglichen.
5. Wähle die **Zugriffseinstellungen** für alle Besucher aus:
   - **Ansichtbar** — alle, die die Einbettung sehen, können das Board ansehen.
   - **Zugriff erforderlich** — alle, die die Einbettung sehen, müssen Zugang haben, um das Board anzusehen, zu kommentieren oder zu bearbeiten.
6. Wähle **Board einbetten** aus.

Die Einbettung respektiert die Freigabeeinstellungen des Boards. Auf mobilen Geräten sind alle Einbettungen nur im Ansichtsmodus verfügbar.

## Ein Board mit Einbettungscode einbetten

Verwende diese Option für jede Plattform, die iFrame unterstützt, wie **WordPress** oder **Webflow**.

1. Öffne das **Freigabefeld** mit einer der folgenden Methoden:
   - Wähle oben rechts **Teilen** > **Einbetten** aus, oder
   - Wähle im Hauptmenü des Boards **Board** > **Exportieren** > **Einbetten** aus, oder
   - Wähle auf dem Canvas das Element aus, das du einbetten möchtest (Rahmen oder Format). Zum Beispiel ein Dokument. Öffne das Drei-Punkte-Kontextmenü und wähle **Dieses Dokument einbetten** aus.
2. Wähle die **Startansicht**:
   - **Board** — der gesamte Canvas.
   - **Bestimmtes Element**, wie Rahmen oder Format (Dokument, Diagramm, Tabelle, Zeitachse oder Präsentation).
3. (Optional) **Startbereich festlegen** — ziehe, um einen genauen Bereich des Boards zu markieren.
4. Interaktion entscheiden:
   - Wähle **Nur ansehen**, um die Ansicht zu sperren.
   - Deaktiviere **Nur ansehen**, um den Betrachtern das Verschieben, Zoomen, Kommentieren oder Bearbeiten (wenn sie die Berechtigung dazu haben) zu erlauben.
5. Wähle **Code kopieren** und füge ihn am gewünschten Ort ein.
   Wenn das Ziel nur URLs akzeptiert, wähle stattdessen **Link kopieren**.

Du kannst mehrere Einbettungen für dasselbe Board erstellen, jeweils mit eigener Startansicht, Startbereich oder Fokus-Objekt.

### Präsentationen automatisch abspielen

Um eine Präsentation automatisch abzuspielen, stelle im **Einbetten**-Tab das **Auto-Slide-Intervall** zwischen 1 und 30 Sekunden ein. Die automatische Wiedergabe wird ignoriert, wenn du ein Board in ein anderes Board einbettest.

## Wie Einbettungen erscheinen

- Der Boardname ist nicht anklickbar.
- Die Mini-Map, [Merkzettel](../../essential-tools/17-visual-notes.md) und Pop-ups sind standardmäßig geschlossen.
- Einige Menüoptionen wie **Startansicht festlegen** sind versteckt.
- Alle Einbettungen sind auf mobilen Geräten nur im Ansichtsmodus verfügbar.
- Drittanbieter-Cookie-Blocker können verhindern, dass Einbettungen richtig geladen werden.

## Häufige Fragen

**Was ist der Unterschied zwischen einer Startansicht und dem Fokusmodus?**
Eine Startansicht legt die Anfangsposition fest, aber Betrachter können das Board weiterhin erkunden. Der Fokusmodus blendet alles außer dem ausgewählten Objekt aus und ist immer im Ansichtsmodus.

**Kann ich eine Einbettung im Fokusmodus bearbeitbar machen?**
Nein. Um Zusammenarbeit zu ermöglichen, müssen Sie den **Ansichtsmodus** deaktivieren und Bearbeitungsrechte in den Freigabeeinstellungen des Boards gewähren.

**Welche Widgets werden unterstützt?**
Dokumente, Diagramme, Tabellen, Zeitachsen, Präsentationen und jeder Rahmen.

**Kann ich das Miro-Logo entfernen?**
Nein. Das Entfernen des Brandings ist nicht möglich.

**Kann ich ein Board in ein anderes Board einbetten?**
Ja. Kopiere den Einbettungscode und füge ihn in das Zielboard mit **iFrame-Code einfügen** ein.
