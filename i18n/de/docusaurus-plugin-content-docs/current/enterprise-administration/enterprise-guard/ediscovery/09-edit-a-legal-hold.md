---
title: Aufbewahrungsfrist bearbeiten
article_id: 27968005251090
translation_id: 27968005251090
locale: de
sidebar_position: 8
created_at: '2025-07-09T17:31:49Z'
updated_at: '2025-11-25T15:52:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
---

Das Bearbeiten einer Aufbewahrungsfrist ermöglicht es eDiscovery-Admins, laufende rechtliche Aufbewahrungsmaßnahmen anzupassen und zu verfeinern, während sich die Anforderungen der Untersuchung weiterentwickeln. Egal, ob neue Verwalter identifiziert werden, zusätzliche Miro-Boards relevant werden oder bestehende Boards oder Nutzer nicht mehr im Geltungsbereich liegen, durch das Bearbeiten einer Aufbewahrungsfrist wird sichergestellt, dass die richtigen Daten während des gesamten rechtlichen Verfahrens erhalten und vertretbar bleiben.

Admins können den Namen oder die Beschreibung der Aufbewahrungsfrist aktualisieren und Nutzer sowie Boards nach Bedarf hinzufügen oder entfernen. Diese Flexibilität unterstützt dynamische rechtliche Workflows und stellt sicher, dass die Aufbewahrung präzise, aktuell und am Geltungsbereich der rechtlichen Angelegenheit ausgerichtet bleibt—unter Einhaltung der Compliance und Vermeidung unnötiger Datenaufbewahrung.

Wenn eine Aufbewahrungsfrist bearbeitet wird:

- Boards, die neu zur Aufbewahrung hinzugefügt werden, beginnen ab diesem Zeitpunkt damit, ihre Versionen zu speichern.
- Boards oder Nutzer, die von der Aufbewahrungsfrist entfernt werden, werden nicht mehr aufbewahrt, und ihre Versionen werden nicht mehr als Teil dieser Aufbewahrungsfrist bewahrt.
- Boards, die unter Aufbewahrung stehen, werden weiterhin alle Versionen aufbewahren, einschließlich aller Löschungen, die nach der Anwendung der Aufbewahrung erfolgen.

Dieser Ansatz stellt sicher, dass Organisationen mit Genauigkeit und Rechenschaftspflicht auf rechtliche Anforderungen reagieren können, während sich die Untersuchung entwickelt.

Um eine Aufbewahrungsfrist zu bearbeiten, führe die folgenden Schritte aus:

:::note
Du musst die [Rolle des eDiscovery-Admins](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben, um diese Aufgabe auszuführen. Um die eDiscovery-Admin-Rolle anzufordern, wende dich bitte an deinen Unternehmens-Admin.
:::

1. Gehe zu deinen Miro-Einstellungen.
2. Klicke im linken Bereich unter **Enterprise Guard** auf **eDiscovery**.
3. Klicke auf der **eDiscovery**-Seite auf den **Tab "Untersuchungen"**.
4. Klicke auf den Fall, in dem du die Aufbewahrungsfrist bearbeiten möchtest.
   Die Liste der Aufbewahrungsfristen innerhalb der Untersuchung wird angezeigt.
5. Klicke in der Zeile der Aufbewahrungsfrist, die du bearbeiten möchtest, auf die drei Punkte und dann auf **Aufbewahrungsfrist bearbeiten**.
6. Auf der Seite **„Aufbewahrungsfrist bearbeiten“** gib die entsprechenden Informationen für jedes Feld ein oder wähle sie aus. Die einzelnen Felder und ihre Beschreibungen findest du in der nachstehenden Tabelle.

   |  |  |
   | --- | --- |
   | **Feld** | **Beschreibung** |
   | Name der Aufbewahrungsfrist  **(erforderlich)** | Name der Aufbewahrungsfrist.  Maximale Länge: 60 Zeichen. |
   | Kriterien  **(erforderlich)** | Art der Inhalte, die für diese Aufbewahrungsfrist gelten Diese Version unterstützt nur alle Inhalte. |
   | **Nutzer, die Inhalte besitzen, gemeinsam besitzen, darauf zugegriffen, sie geändert oder erstellt haben**  **(erforderlich)** | Füge die Nutzer hinzu, die von der Aufbewahrungsfrist betroffen sind. Klicke auf das Feld, um nach Namen oder E-Mail-Adresse zu suchen. Du kannst bis zu 200 Nutzer pro Aufbewahrungsfrist haben, einschließlich der Nutzer, die in Aktualisierungen der Aufbewahrungsfrist hinzugefügt wurden.  **Notizen:**  - Wenn ein Nutzer, der einer Aufbewahrungsfrist unterliegt, ein Board öffnet, ändert oder in irgendeiner Weise damit interagiert (umbenennt oder Inhalte hinzufügt), wird dieses Board gekennzeichnet und bleibt erhalten. Wird beispielsweise der Name des Boards geändert oder die Inhalte aktualisiert, werden sie automatisch in die Aufbewahrungsfrist verschoben. Darüber hinaus werden die Board-Eigentümerschaft und die Board-Erstellung ausgesetzt.  - Wenn eine Aufbewahrungsfrist bearbeitet wird, gilt sie für Boards, die von den jeweiligen Nutzern zum Zeitpunkt der Aufbewahrung erstellt, besessen oder mitbesessen wurden. Darüber hinaus sind alle Boards betroffen, auf die Nutzer nach dem Inkrafttreten der Aufbewahrungsfrist zugreifen und die sie ändern. Historische Board-Zugriffs- und Update-Details sind in dieser Version nicht verfügbar.  - Boards, die neu zur Aufbewahrungsfrist hinzugefügt werden, beginnen ab dem Zeitpunkt, an dem du die Änderungen zur Aufbewahrungsfrist in Schritt 9 speicherst, deren Versionen zu speichern.  - Boards oder Nutzer, die aus der Aufbewahrungsfrist entfernt werden, werden nicht mehr aufgehoben, und ihre Versionen werden nicht mehr im Rahmen dieser gesetzlichen Aufbewahrungsfrist behalten.  - Boards, die unter Aufbewahrung bleiben, werden weiterhin alle Versionen beibehalten, einschließlich aller Löschungen, die nach der Anwendung der Aufbewahrung stattfinden. |
7. **Weiter** klicken. Die Seite **Auswirkungen überprüfen** wird angezeigt.
8. Sieh dir die Auswirkungen der Erstellung dieser Aufbewahrungsfrist an, wie zum Beispiel:
   - Die Anzahl der Boards, die unter Aufbewahrung bleiben, von der Aufbewahrung freigegeben werden und zur Aufbewahrung hinzugefügt werden.
   - Die Nutzer, die die Boards besessen, gemeinsam besessen, darauf zugegriffen, sie geändert oder erstellt haben.
   - Die Kriterien für die Aufbewahrung.
   - Die Liste der Boards, die unter Aufbewahrung bleiben.

   **Notizen:**
   - Boards, die einer Aufbewahrungsfrist unterliegen, können weiterhin abgerufen und bearbeitet werden, aber alle Versionen bleiben erhalten. Wenn Inhalte gelöscht werden, sind sie innerhalb der Aufbewahrungsfrist weiterhin verfügbar. Die Anzahl der Inhaltselemente, die aufbewahrt werden, kann sich je nach zukünftigen Nutzeraktionen erhöhen.

   - Wenn ein Nutzer, der einer Aufbewahrungsfrist unterliegt, ein Board öffnet, ändert oder in irgendeiner Weise damit interagiert (umbenennen oder Inhalte hinzufügen), wird dieses Board gekennzeichnet und bleibt erhalten. Wird beispielsweise der Name des Boards geändert oder die Inhalte aktualisiert, werden sie automatisch in die Aufbewahrungsfrist verschoben. Darüber hinaus werden die Board-Eigentümerschaft und die Board-Erstellung ausgesetzt.

   - Wenn eine Aufbewahrungsfrist erstellt wird, gilt sie für Boards, die zum Zeitpunkt der Aufbewahrung von den jeweiligen Nutzern erstellt, besessen oder mitbesessen wurden. Darüber hinaus sind alle Boards, auf die die Nutzer nach dem Inkrafttreten der Aufbewahrungsfrist zugreifen und die sie ändern, ebenfalls betroffen. Historische Board-Zugriffs- und Update-Details sind in dieser Version nicht verfügbar.
9. Nachdem du die Auswirkungen der von dir erstellten Aufbewahrungsfrist überprüft hast, klicke auf **Aufbewahrungsfrist speichern**.
   Auf der Untersuchungsseite wird die aktualisierte Aufbewahrungsfrist angezeigt, wie der Name der Aufbewahrungsfrist, die Art der Inhalte, die von der Aufbewahrungsfrist betroffen sind, die Anzahl der Nutzer in dieser Aufbewahrungsfrist, das Erstellungsdatum der Aufbewahrungsfrist, der Status der Aufbewahrungsfrist und die Anzahl der Boards, die auf die Aufbewahrungsfrist gesetzt wurden.
