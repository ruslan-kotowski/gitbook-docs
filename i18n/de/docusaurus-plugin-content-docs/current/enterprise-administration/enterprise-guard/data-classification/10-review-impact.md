---
title: "Auswirkungen \xFCberpr\xFCfen"
article_id: 16494764223378
translation_id: 16494764223378
locale: de
sidebar_position: 10
created_at: '2024-01-19T19:02:16Z'
updated_at: '2025-08-18T09:36:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
id: 10-review-impact
---

Dies ist der letzte Schritt der Konfiguration der automatischen Klassifizierung und der Vorgaben. In diesem Schritt des Ablaufs musst du die Auswirkungen der Aktualisierungen der Klassifizierung oder der Vorgaben für die Konfiguration überprüfen. In diesem Schritt des Ablaufs musst du die Auswirkungen der Änderungen überprüfen, die du an der Konfiguration der Klassifizierung oder der Vorgaben vornimmst. Die folgenden Abschnitte beschreiben die Informationen, die auf der Seite mit den Auswirkungen der Überprüfung verfügbar sind, und die verschiedenen Maßnahmen, die du ergreifen kannst.

## Verteilung der Klassifizierungsstufen

In diesem Abschnitt kannst du die Auswirkungen deiner aktualisierten Konfiguration im Hinblick auf die Änderungen für jede Klassifizierungsstufe des Boards überprüfen.

Der Abschnitt " **Verteilung der Klassifizierungsstufen** " ist zusammenklappbar, damit du effizienter durch die Liste der Aktualisierungen blättern kannst (siehe Abbildung 1).

![Zusammenklappbarer Abschnitt Verteilung der Klassifizierungsstufen](images/24937148542482_Collapsible_Distribution_of_classification.png)

*Abbildung 1: Zusammenklappbarer Abschnitt Verteilung der Klassifizierungsstufen*
Die spaltenbasierte UI vereinfacht den Vergleich und die Überprüfung von Aktualisierungen der Klassifizierung von Boards. Wir haben für jede Klassifizierungsstufe eigene Spalten erstellt, in denen die Anzahl der hinzugefügten Boards, die Anzahl der entfernten Boards und die aktualisierte Gesamtzahl angezeigt werden (Abbildung 2).

![Spaltenbasierte UI, die die Anzahl der hinzugefügten Boards, die Anzahl der entfernten Boards und die aktualisierte Gesamtsumme für jede Klassifizierungsstufe anzeigt](images/24937148548114_columnview.png)

*Abbildung 2: Spaltenbasierte UI, die die Anzahl der hinzugefügten Boards, die Anzahl der entfernten Boards und die aktualisierte Gesamtsumme für jede Klassifizierungsstufe anzeigt*

Die Drill-Down-Funktion bietet eine umfassende Ansicht (Abbildung 3) der folgenden Details:
- Labels für die automatische Klassifizierung hinzugefügt oder entfernt.
- Vorgaben hinzugefügt oder entfernt.
- Anzahl der Boards, die in eine bestimmte Klassifizierungsstufe gewechselt sind.
- Anzahl der Boards, die von den vorgenommenen Konfigurationsänderungen nicht betroffen sind.

![Drill-Down-Funktion mit umfassender Ansicht der Aktualisierungen](images/24937158222610_drilldown_feature_classification.png)

*Abbildung 3: Drill-Down-Funktion mit umfassender Ansicht der Aktualisierungen*

## Auswirkungen der Vorgaben

In diesem Abschnitt werden die Vorgaben angezeigt, die auf der Klassifizierungsstufe eines Boards basieren, sowie die Gesamtzahl der Boards, die mit den jeweiligen Vorgaben versehen werden. Die Zahl in Klammern gibt die Anzahl der Boards an, für die die Leitplanke nach der Veröffentlichung der neuen Konfiguration hinzugefügt oder entfernt wird. Außerdem wird in diesem Abschnitt auch die Anzahl der Boards angezeigt, die nicht klassifiziert sind (Abb. 4).

Um die Konfiguration der Vorgaben zu aktualisieren, klicke auf **Zurück**.
*![Klassifizierung konfigurieren Auswirkungen überprüfen](images/24937158224530_guardrails.png)
Abbildung 4: Klassifizierung konfigurieren > Auswirkungen überprüfen*

## Aktualisiere die Konfiguration für die automatische Klassifizierung

Um Aktualisierungen vorzunehmen, nachdem du die Auswirkungen der Aktualisierungen der Konfiguration der automatischen Klassifizierung und der Vorgaben überprüft hast, klicke auf die Schaltfläche **"Zurück"**, nimm die Aktualisierungen der Konfiguration vor und überprüfe die Auswirkungen noch einmal.

## Konfiguration veröffentlichen

Nachdem du die Auswirkungen der Klassifizierung oder der Vorgaben überprüft hast, klicke auf **Veröffentlichen**.

:::note
Hinweise:
- Die Konfiguration der Klassifizierungsstufe wird sofort angewendet.
- Die Konfiguration der Vorgaben wird sofort übernommen.
- Wenn neue Boards mit sensiblen Daten hinzugefügt werden, werden diese Boards automatisch klassifiziert, nachdem der nächste Datenerkennungszyklus abgeschlossen ist.
- Wenn Board-Inhalte aktualisiert werden (Entfernen oder Hinzufügen sensibler Inhalte), werden diese Boards nach Abschluss des nächsten Datenerkennungszyklus automatisch klassifiziert.
:::
