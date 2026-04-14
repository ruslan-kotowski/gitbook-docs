---
title: "Vorgaben\xFCbersicht"
article_id: 28839068735890
translation_id: 28839068735890
locale: de
sidebar_position: 1
created_at: '2025-08-18T09:35:15Z'
updated_at: '2025-11-25T15:53:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

## Vorgaben für die Inhaltssicherheit

Die folgende Tabelle listet die in der aktuellen Version unterstützten Vorgaben für die Inhaltssicherheit auf.

|  |  |  |
| --- | --- | --- |
| **Vorgabe** | **Beschreibung** | **Betroffene Nutzer** |
| **Inhaltsreplikation blockieren** | - Optionen zum Verwalten der Inhaltsreplikation sind sowohl in der Miro-Oberfläche als auch in den Miro-APIs nicht verfügbar. Zum Beispiel ist die Option, festzulegen, wer Board-Inhalte kopieren kann, in der Benutzeroberfläche nicht verfügbar, und die Option, den Zugriff über die Update-Board-API zu aktualisieren, ist nicht verfügbar.  - Optionen für die Inhaltsreplikation sind in der Miro-Oberfläche nicht verfügbar. Dies beinhaltet:     - Ein Board in andere     Teams anderer Nutzer     - Dateien auf dem Board herunterladen     - Bilder auf dem Board herunterladen     - Herunterladen von PDFs auf dem Board     - Kopieren von Inhalten oder Objekten von      das Board zu einem anderen Board     - Boards als Bild exportieren     - Boards als PDF exportieren     - Boards als eigene Vorlage speichern      Vorlage     - Inhaltsreplikation über APIs ist      Nicht verfügbar. Die API gibt ein      Fehler 403 als Antwort. | Der Eigentümer und Miteigentümer des Boards sind nicht eingeschränkt. Der Eigentümer und Miteigentümer des Boards können Inhaltsreplikationsaktionen durchführen, da dies für den Eigentümer notwendig ist, um das Board zu aktualisieren und bereinigte Versionen der Boards für die weitere Zusammenarbeit zu erstellen.  Alle anderen sind eingeschränkt. |
| **Die Nutzung von Miro AI blockieren** | - Alle Miro AI-Funktionen sind deaktiviert, wodurch der Zugriff auf KI-gesteuerte Funktionen wie Textgenerierung, Bildverarbeitung und intelligente Vorschläge verhindert wird.  - Nutzer werden innerhalb von Miro nicht mit KI-gestützten Tools interagieren oder diese aktivieren können.  - Bestehende von Miro AI generierte Inhalte bleiben unverändert, und Nutzer können diese Inhalte ändern oder erweitern. Jedoch können Nutzer Miro AI nicht mehr verwenden, um die Inhalte zu bearbeiten oder zu aktualisieren. | Alle sind eingeschränkt, einschließlich des Eigentümers und der Miteigentümer des Boards. |

## Freigabevorgaben

Die folgende Tabelle listet die in der aktuellen Version unterstützten Freigabevorgaben auf.

|  |  |  |
| --- | --- | --- |
| **Vorgabe** | **Beschreibung** | **Betroffene Nutzer** |
| **Öffentliche Freigabe blockieren** | - Die Option zum Freigeben für *Jede Person mit Link* ist in der Miro-UI nicht verfügbar.  - Öffentliche Freigabe über die API ist nicht verfügbar. Die API gibt einen Fehler 403 als Antwort zurück.  - Öffentliche Freigabe blockieren gilt nicht für Boards, die mithilfe des Zugriffslinks der Live-Einbettung eingebettet sind, da diese Boards nicht über einen öffentlichen Link geteilt werden. Weitere Informationen findest du unter [So erlaubst oder beschränkst du das Einbetten von Miro-Boards in unterstützte Apps.](../../managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md) | Alle sind eingeschränkt, einschließlich des Board-Eigentümers. |
| **Freigabe für Teams blockieren** | - Die Option zum Freigeben für *Jede Person im Team* ist in der Miro-Oberfläche nicht verfügbar.  - Die Freigabe für Teams über die API ist nicht verfügbar. Die API gibt einen Fehler 403 als Antwort zurück. | Alle sind eingeschränkt, einschließlich des Board-Eigentümers. |
| **Freigabe für das Unternehmen blockieren** | - Option zum Freigeben für *Jede Person bei der Organisation* ist in der Miro-Oberfläche nicht verfügbar.  - Die Freigabe für das Unternehmen über die API ist nicht verfügbar. Die API gibt einen Fehler 403 als Antwort zurück. | Jeder ist eingeschränkt, einschließlich des Board-Eigentümers. |
| **Freigabe außerhalb zugelassener Domains blockieren** | - Die Freigabe von Boards über direkte E-Mail-Einladungen ist auf Nutzer beschränkt, deren E-Mail-Adressen zu den in dieser Liste aufgeführten Domains gehören. Diese Vorgabe betrifft nicht den Zugang, der über Team-, Organisations- oder öffentliche Links gewährt wird, da diese durch separate Vorgaben kontrolliert werden.  - Du kannst bis zu 20 zugelassene Domains in dieser Liste hinzufügen.  - Diese Vorgabe ist darauf ausgelegt, mit der Einstellung [**Sicherheit > Freigabe > Zugelassene Domains**](../data-security/07-sharing-policy-on-enterprise-plan.md) zusammenzuarbeiten, die sowohl auf Organisations- als auch auf Teamebene konfiguriert werden kann. Das bedeutet, dass du, wenn die Einstellung **Zugelassene Domains** aktiviert ist, sicherstellen musst, dass die Domain, für die du das Teilen von Boards erlauben möchtest, sowohl in der Einstellung für Intelligente Vorgaben als auch in der Einstellung [**Sicherheit > Freigabe > Zugelassene Domains**](../data-security/07-sharing-policy-on-enterprise-plan.md) aufgelistet ist.   **Hinweise:**  - Wenn das Board bereits mit E-Mail-Adressen geteilt wurde, die nicht auf dieser Liste stehen, behalten die Nutzer, die bereits Zugriff auf das Board haben, weiterhin ihren Zugang.  - Bestehende Nutzer, die bereits Zugriff auf ein Board haben, aber nicht in der Liste der zugelassenen Domains stehen, werden in der Verwalten von Board-Zugriffen-Oberfläche angezeigt. Du kannst diesen Nutzern den Zugriff manuell entziehen. - Du kannst Informationen über Domain-Einschränkungen, die über die Klassifizierungsseite angewendet wurden, ganz einfach ansehen.   **Beispiel 1:** **Sicherheit > Freigabe > Zugelassene Domains:** miro.com, gmail.com  **Zugelassene Domains für Vorgaben:** miro.com  ***Ergebnis:*** Die Freigabe von Boards über direkte E-Mail-Einladung ist auf E-Mail-Adressen beschränkt, die auf miro.com enden. Obwohl gmail.com in der Einstellung "Sicherheit > Freigabe > Erlaubte Domains" zugelassen ist, wird es durch die Sicherheitsvorgabe nicht erlaubt.  **Beispiel 2:** **Sicherheit > Freigabe > Erlaubte Domains:** miro.com, gmail.com  **Zulässige Domains der Sicherheitsvorgabe:** example.org, example.com  ***Ergebnis:*** Das Teilen von Boards über direkte E-Mail-Einladungen ist für keine Domain erlaubt, da es keine Überschneidung zwischen den beiden Listen gibt. | Die Freigabe von Boards über direkte E-Mail-Einladungen ist auf Nutzer beschränkt, deren E-Mail-Adressen zu den in dieser Liste erlaubten Domains gehören. Diese Vorgabe beeinflusst nicht den Zugriff, der durch Team-, Organisations- oder öffentliche Links gewährt wird, da diese durch separate Vorgaben kontrolliert werden.  Wenn das Board bereits mit E-Mail-Adressen geteilt wurde, die nicht auf dieser Liste stehen, werden die Personen, die bereits Zugriff auf das Board haben, diesen weiterhin behalten.   Diese Vorgabe ist darauf ausgelegt, mit der Einstellung [**Sicherheit > Freigabe > Erlaubte Domains**](../data-security/07-sharing-policy-on-enterprise-plan.md) zu arbeiten, die sowohl auf Organisations- als auch Teamebene konfiguriert werden kann. Sieh dir die Beschreibungs-Spalte für ausführliche Erläuterungen und Beispiele an. |
