---
title: An Display senden
article_id: 4406230245010
translation_id: 7697958801554
locale: de
sidebar_position: 10
created_at: '2022-09-19T08:32:58Z'
updated_at: '2026-04-10T12:06:14Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: interactive-displays
---

Du kannst in Sekundenschnelle mit der Zusammenarbeit beginnen. Mit der Funktion „An Display senden“ kannst du ein beliebiges Miro-Board auf deinem interaktiven Display starten.

> ***Miro UI-Updates werden schrittweise eingeführt***
> Miro verbessert die Benutzeroberfläche des Boards, um integrativer und intuitiver zu werden, und führt eine Weiterentwicklung von Projekten namens Bereiche ein. Der Rollout wird für alle Miro-Konten über mehrere Wochen nach und nach durchgeführt.
>
> Falls du bereits die verbesserte Benutzeroberfläche und das Layout der Bereiche hast, beschreibt dieser Artikel möglicherweise Eintrittspunkte, die sich geändert haben.
>
> Um die aktuellste Dokumentation zu sehen, siehe [Miors neue vereinfachte Benutzeroberfläche](../../using-miro/working-on-the-board/02-miro's-new-simplified-user-interface.md).
>
> Dieser Artikel wird aktualisiert, sobald der Rollout abgeschlossen ist.

Erfahre [wie du Miro auf deinem interaktiven Display einrichtest](07-interactive-displays.md).

## So funktioniert „An Display senden“

1. Öffne die Miro-App auf deinem interaktiven Display oder öffne den Browser und gehe auf [miro.com/displays](https://miro.com/displays/).
2. Öffne das Miro-Board auf deinem persönlichen Gerät.

**Von deinem Laptop oder Tablet**

1. Wähle in der Board-Leiste deines Laptops oder Tablets die vertikalen drei Punkte aus.
   Das **Hauptmenü** öffnet sich.
2. Wähle **An interaktives Display senden**.
3. Gib den eindeutigen Paarungscode ein, den du auf dem interaktiven Display siehst. Dadurch wird das Board von deinem Laptop oder Tablet an das Display gesendet.

**Von deinem mobilen Gerät**

:::note
Wenn du ein mobiles Gerät verwendest, stelle sicher, dass du zuerst die Miro-App für [iOS](https://apps.apple.com/us/app/miro-collaborative-whiteboard/id1180074773) oder [Android](https://play.google.com/store/apps/details?id=com.realtimeboard&hl=en&gl=US) herunterlädst.
:::

1. Auf dem Miro-Board auf deinem mobilen Gerät tippe auf das **Einstellungen** Symbol in der rechten oberen Ecke.
   **![board_settings.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4967840616850_board%20settings.jpg)**
   *Öffnen der Board-Einstellungen in der mobilen App*
2. Tippe auf **An interaktives Display senden.**
   **![send_to_interactive_display.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4967865515794_send%20to%20interactive%20display.jpg)**
   ***Die Option „An interaktives Display senden“ in der mobilen App***
3. Gib den eindeutigen Paarungscode ein, den du auf dem interaktiven Display siehst. Dadurch wird das Board von deinem Handy an das Display gesendet.
   ![enter_code.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4967892004114_enter%20code.jpg)
   *Die Option, den Code einzugeben*

:::tip
Denke daran, dich nach der Sitzung vom Display abzumelden, um deine Daten zu schützen. Wenn du das vergisst, wirst du nach 15 Minuten Inaktivität automatisch abgemeldet.
:::

## Fehlerbehebung

Wenn du „An Display senden“ in der Desktop-App auf Windows nicht siehst, versuche die folgenden Schritte zur Fehlerbehebung.

1. Installiere die [Miro-App für den Desktop](https://miro.com/apps/).
2. Klicke mit der rechten Maustaste auf das Symbol der Miro Desktop-App und wähle **Eigenschaften**.
   ![Eigenschaften.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4949111804946_properties.jpg)*Eigenschaften der Miro-App*
3. Wechsle zum **Tab Verknüpfung** und füge den untenstehenden Zusatz zu den CLI-Argumenten im Feld **Ziel** hinzu und klicke auf OK, um die Änderungen zu übernehmen.

   ```
   --public-device
   ```

   ![target_field.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4949083211538_target%20field.jpg)*Der Verknüpfung-Tab in den Miro Eigenschaften*
4. Jetzt wird die Option „An Display senden“ standardmäßig angezeigt, wenn du die App startest.

:::tip
Erfahre mehr darüber, [welche Displays von Miro unterstützt werden](07-interactive-displays.md) und [lies nach, wie du das richtige Display für hybride Zusammenarbeit auswählst](09-selecting-the-right-interactive-display-for-hybrid-collaboration.md).
:::
