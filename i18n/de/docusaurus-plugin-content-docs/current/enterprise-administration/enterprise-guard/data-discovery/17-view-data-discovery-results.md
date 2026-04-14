---
title: Ergebnisse der Datenerkennung anzeigen
article_id: 15794382139154
translation_id: 15794382139154
locale: de
sidebar_position: 16
created_at: '2023-12-15T15:47:29Z'
updated_at: '2025-11-25T15:40:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

Der Datenerkennungszyklus läuft mindestens einmal pro Stunde und durchsucht alle Boards nach datenschutzrelevanten Informationen. Dazu zählen auch Boards, die bereits im vorherigen Datenerkennungszyklus gescannt wurden.

:::note
Um die Ergebnisse der Datenerkennung ansehen zu können, musst du die Rolle eines [Admins für sensible Inhalte](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Die Rolle des Admins für sensible Inhalte kannst du bei deinem Unternehmens-Admin anfordern.
:::

*![privacy_related_dd.png](images/25066209802770_privacy_related_dd.png)
Abbildung 1: Ergebnisse der Datenerkennung*

Obwohl wir kontinuierlich mit unseren Technologiepartnern und Kunden an der Verbesserung des Systems zur Erkennung sensibler Inhalte arbeiten, können wir nicht garantieren, dass 100 % der sensiblen Daten auf deinen Boards gefunden und markiert werden. Unser System zur Erkennung sensibler Inhalte verwendet Muster und andere Kriterien, um die Wahrscheinlichkeit einer Übereinstimmung zu bestimmen. Es kann vorkommen, dass das System Daten auf deinen Boards fälschlicherweise als wahrscheinlich sensibel kennzeichnet (falsch positiv) oder Daten nicht als sensibel kennzeichnet (falsch negativ). Dies wird von verschiedenen Faktoren beeinflusst, z. B. von der Nähe verwandter Begriffe oder der Formatierung sensibler Daten.

Weitere Informationen darüber, wie du falsch positive Treffer unterdrücken kannst, findest du unter [Unterdrückung eines Treffers mit sensiblem Inhalt](11-suppress-a-sensitive-content-match.md).

## Informationen zum letzten abgeschlossenen Datenerkennungsscan anzeigen

Im Abschnitt **Ergebnisse** der Datenerkennung wird angezeigt, wann der letzte Datenerkennungsscan abgeschlossen wurde, und zwar im Format Monat, Tag, Jahr, Stunde:Minute AM/PM und Zeitzone (im Verhältnis zu GMT). Zum Beispiel Dec 14, 2023, 10:15 PM GMT+1 (Abbildung 1).

## Ergebnisse der Datenerkennung anzeigen

Im Abschnitt **Ergebnisse** der Datenerkennung befinden sich Informationen wie der Name der Verordnung, eine kurze Beschreibung, das zugehörige Label und die Anzahl der Boards mit potenziell sensiblen Inhalten, die unter den Anwendungsbereich der Verordnung fallen könnten (Abbildung 1).

Um die Boards mit hochsensiblen Daten zu untersuchen, klicke auf den Link mit der Boardanzahl.  Dann wird die Inhaltssuche mit der Liste der Boards angezeigt. Weitere Informationen findest du unter [Boards mit hochsensiblen Daten überprüfen](16-review-boards-with-privacy-related-information.md).
