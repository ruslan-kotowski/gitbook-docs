---
title: Verwaltung von eigenen AGB
article_id: 27621616452882
translation_id: 27621616452882
locale: de
sidebar_position: 3
created_at: '2025-06-24T23:29:13Z'
updated_at: '2025-11-04T14:10:40Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

## Eigene AGB erstellen

:::note
Hinweise:

- Admins müssen die folgenden Enterprise Guard-Berechtigungen haben, um die eigenen AGB anzusehen und zu verwalten:
  - Admin für sensible Inhalte hat von vornherein die nötigen Berechtigungen.
  - Benutzerdefinierte Admin-Rollen müssen Folgendes beinhalten:
    - Eigene AGB ansehen
    - Eigene AGB verwalten
- Gäste und externe Nutzer sind ausgeschlossen.
- Miro speichert nicht die AGB, sondern nur den Link und die Metadaten.
:::

1. Gehe zu **Einstellungen** > **Enterprise Guard** > **AGB**.
2. Wenn du zum ersten Mal AGB erstellst, klicke auf **AGB hinzufügen**.
   Wenn du bereits eine bestehende Konfiguration hast und eine weitere hinzufügen möchtest, klicke im Listenansicht auf **Neu erstellen**.
3. Unter **Einrichten** → **Bedingungen**:

- **Trigger**: Wähle zwischen **Erfolgreiche Anmeldung** oder **AI-Nutzung**.
  **Erfolgreiche Anmeldung**

  - Der Dialog erscheint unmittelbar nach der Anmeldung.
  - Nutzer können auf **Weiter** klicken, um zu akzeptieren und fortzufahren, oder auf **Abmelden**.

  **AI-Nutzung**

  - Der Dialog erscheint, wenn der Nutzer mit Miro AI interagiert, beispielsweise beim Umschalten des AI-Layouts, beim Öffnen des seitlichen AI-Felds oder beim Starten eines AI-Tools oder AI-Aktion (zum Beispiel KI-Kollege).
  - Nutzer können auf **Fortfahren** klicken, um zuzustimmen und AI-Funktionen zu nutzen. Wenn sie **Abbrechen** klicken, bleiben sie angemeldet und können alle nicht mit AI verbundenen Funktionen weiter nutzen.
- **Geltungsbereich**: **Alle Nutzer und Admins in der Organisation**.
- **Wiederholungszeitraum**: Geben Sie eine Zahl ein und wählen Sie **Tage**, **Wochen** oder **Monate**.Standard: zwei Wochen.
  Nutzer werden nicht erneut aufgefordert, bis der Wiederholungszeitraum endet oder die Bedingungen aktualisiert werden.

4. Unter **Einrichten** → **Inhalt**:
   - **Titel** (max. 32 Zeichen)
   - **Beschreibung** (max. 200 Zeichen)
   - **Link:** Richtlinienlinks (extern gehostet). Um zusätzliche Links einzufügen, klicke auf +Link hinzufügen. Es werden bis zu drei Links unterstützt. Jede Link-URL muss eindeutig sein.
   - **Linktext** (max. 60 Zeichen). Jeder Linktext muss eindeutig sein.
5. Klicke auf **Vorschau anzeigen** (oben rechts), um den Inhalt des Dialogfelds der AGB anzusehen. Nimm bei Bedarf Anpassungen an den Inhalten der AGB vor.
6. Sobald du mit dem Inhalt der AGB fertig bist, klicke auf **Weiter**.
7. Überprüfe die AGB, bestätige deine Einstellungen und Inhalte und klicke dann auf **Veröffentlichen**.
   Die Durchsetzung erfolgt sofort für den ausgewählten Auslöser.

## Eigene AGB bearbeiten

1. Öffnen Sie **Einstellungen** > **Enterprise Guard** > **Benutzerdefinierte AGB**.
2. Wählen Sie in der Liste die Konfiguration der benutzerdefinierten AGB aus, die Sie aktualisieren möchten, und klicken Sie dann auf **Bearbeiten**.
3. Aktualisieren Sie die Felder in **Bedingungen** und **Inhalt** nach Bedarf.
4. Wenn Sie die benutzerdefinierten AGB aktualisieren und alle Nutzerbestätigungen sofort zurücksetzen möchten, klicken Sie auf **Sofort veröffentlichen.**
   Wenn Sie die benutzerdefinierten AGB aktualisieren und die Nutzer nach Ablauf der konfigurierten Wiederholungsperiode erneut auffordern möchten, klicken Sie auf den Pfeil nach unten, wählen Sie **Im nächsten Zyklus veröffentlichen**, und klicken Sie dann auf **Im nächsten Zyklus veröffentlichen**.

## Löschen eigener AGB

Das Löschen deaktiviert die eigenen AGB sofort und kann nicht rückgängig gemacht werden.

1. Öffne **Einstellungen** > **Enterprise Guard** > **Eigene AGB**.
2. Wähle in der Liste die Konfiguration der eigenen AGB aus, die du entfernen möchtest, und klicke dann auf **Löschen**.
3. Um die ausgewählten eigenen AGB dauerhaft zu löschen, klicke auf **AGB löschen**.
