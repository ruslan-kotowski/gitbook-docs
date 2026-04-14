---
title: "Aufbewahrungsfrist im \xDCberblick"
article_id: 21922434361618
translation_id: 21922434361618
locale: de
sidebar_position: 1
created_at: '2024-10-11T12:20:34Z'
updated_at: '2025-11-25T15:48:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
---

Die Aufbewahrungsfrist wurde entwickelt, um Compliance- und eDiscovery-Prozesse zu unterstützen, indem sie Boards aufbewahrt, die Gegenstand einer Untersuchung sind oder für laufende Rechtsverfahren relevant sind.

[eDiscovery-Admins](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) können die dauerhafte Löschung von Inhalten verhindern, indem sie Aufbewahrungsfristen basierend auf bestimmten Nutzern und deren Aktionen in Miro erstellen. Diese Funktion ist unerlässlich, um sicherzustellen, dass relevante Informationen während des Gerichtsverfahrens aufbewahrt und gesichert werden.

Wenn ein Nutzer, für den eine Aufbewahrungsfrist gilt, beispielsweise mit einem Board interagiert, wird dieses Board automatisch in die Aufbewahrungsfrist verschoben, um die dauerhafte Löschung zu verhindern.

Darüber hinaus werden alle Versionen des Boards gespeichert, um sicherzustellen, dass die Inhalte des Boards für rechtliche Zwecke aufbewahrt werden.

![legalholdoverview.png](images/22388638765842_legalholdoverview.png)

:::note
Du musst die [eDiscovery-Admin-Rolle](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) besitzen, um Aufbewahrungsfrist-Aufgaben durchzuführen. Um die eDiscovery-Admin-Rolle anzufordern, wende dich an deinen Unternehmens-Admin.
:::

## Die wichtigsten Vorteile der Aufbewahrungsfrist

- **Aufbewahrung von Informationen:** Die Aufbewahrungsfrist sorgt dafür, dass alle relevanten Daten aufbewahrt werden, wodurch eine dauerhafte Löschung verhindert wird. Dies ist für die Compliance und rechtliche Untersuchungen von entscheidender Bedeutung, da es garantiert, dass die in einem Rechtsstreit präsentierten Daten korrekt und unverändert bleiben.
- **Einhaltung gesetzlicher Anforderungen:** Die Aufbewahrungsfrist unterstützt Organisationen bei der Einhaltung gesetzlicher und regulatorischer Verpflichtungen, indem sie sicherstellt, dass notwendige Informationen gespeichert und bei Bedarf verfügbar sind, um Strafen oder rechtliche Herausforderungen zu vermeiden.
- **Risikominderung:** Durch die Sicherung wichtiger Daten reduziert die Aufbewahrungsfrist das Risiko eines Datenverlusts, der erhebliche rechtliche oder finanzielle Folgen haben könnte.
- **Audit und Überwachung:** Jedes Mal, wenn eine Aufbewahrungsfrist erstellt oder geändert wird, wird ein Audit-Protokoll generiert, das für volle Transparenz und Nachvollziehbarkeit sorgt. Alle Audit-Protokolle in einer Organisation werden unbegrenzt gespeichert, wenn mindestens eine Aufbewahrungsfrist aktiv ist. Dies gewährleistet die Rechenschaftspflicht und Transparenz bei der Verwaltung von Aufbewahrungsfristen.

## So funktioniert die Aufbewahrungsfrist

- **Nutzer- oder Board-Interaktionen:** Wenn ein Nutzer, der einer Aufbewahrungsfrist unterliegt, ein Board öffnet, ändert oder in irgendeiner Weise damit interagiert (durch Umbenennung oder Hinzufügen von Inhalten), wird dieses Board gekennzeichnet und bleibt erhalten. Wird beispielsweise der Name des Boards geändert oder die Inhalte aktualisiert, werden sie automatisch in die Aufbewahrungsfrist verschoben. Darüber hinaus werden die Board-Eigentümerschaft und die Board-Erstellung ausgesetzt.

  Wenn eine Aufbewahrungsfrist erstellt wird, gilt diese für Boards, die zum Zeitpunkt der Aufbewahrung von den jeweiligen Nutzern erstellt wurden, im Besitz oder Miteigentum waren. Darüber hinaus sind alle Boards betroffen, auf die die Nutzer nach dem Inkrafttreten der Aufbewahrungsfrist zugreifen und die sie ändern. Historische Board-Zugriffs- und Update-Details sind in dieser Version nicht verfügbar.
- **Endnutzeraktionen und Board-Löschung:** Auch wenn die Endnutzer Boards löschen, bleiben diese Boards erhalten, wenn eine Aufbewahrungsfrist vorliegt. Sie bleiben für den Endnutzer unzugänglich, werden jedoch für rechtliche und administrative Zwecke aufbewahrt.
- **Administrative Kontrolle:** eDiscovery-Admins können Aufbewahrungsfristen im Abschnitt „eDiscovery“ in den Einstellungen erstellen und löschen. Die Aufbewahrungsfrist kann auf alle Boards angewendet werden, die ein Nutzer erstellt hat, besitzt, mitbesitzt, bearbeitet oder auf die er zugegriffen hat. Um mehrere Aufbewahrungsfristen zu verwalten, können Admins zuerst einen Fall erstellen, in dem diese Aufbewahrungsfristen gruppiert werden.
- **Teamlöschung:** Wenn es ein Board in einem Team gibt, das einer Aufbewahrungsfrist unterliegt, kann dieses Team nicht dauerhaft gelöscht werden, bevor die Aufbewahrungsfrist aufgehoben wurde. Dadurch wird ein unbeabsichtigter Datenverlust verhindert und sichergestellt, dass alle relevanten Inhalte erhalten bleiben. In Fällen, in denen ein Team gelöscht wird, dies aber ein Board mit einer Aufbewahrungsfrist enthält, wird das Team auf der Seite der gelöschten Teams als „aufbewahrt“ markiert und seine dauerhafte Löschung wird bis zur Aufhebung der Aufbewahrungsfrist ausgesetzt.
- **Admin und eDiscovery-Perspektive:** Endnutzer haben keinen Zugriff auf ein gelöschtes Board, das sich in der Aufbewahrungsfrist befindet, und können es auch nicht wiederherstellen. Admins und E-Discovery-Teams können jedoch weiterhin damit interagieren. Das Board wird solange aufbewahrt, bis der Rechtsfall abgeschlossen ist. Danach kann die Aufbewahrungsfrist aufgehoben werden und das Board dauerhaft gelöscht werden.
- **Board-Exportfunktion:** Boards, die einer Aufbewahrungsfrist unterliegen, können weiterhin mit der Board-Exportfunktion exportiert werden, sodass du relevante Daten für rechtliche Fälle einfach erfassen kannst.
- **Boards verschieben:** Boards, die einer Aufbewahrungsfrist unterliegen, können nicht außerhalb der Organisation verschoben werden. Wenn ein Board einer Aufbewahrungsfrist unterliegt, werden externe Teams automatisch aus der Liste der Teams herausgefiltert, in die das Board verschoben werden kann.
