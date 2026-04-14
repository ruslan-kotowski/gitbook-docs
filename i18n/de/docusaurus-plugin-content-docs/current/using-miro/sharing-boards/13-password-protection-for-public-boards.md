---
title: "Passwortschutz f\xFCr \xF6ffentliche Boards"
article_id: 360014617239
translation_id: 360014617239
locale: de
sidebar_position: 13
created_at: '2020-06-22T10:42:25Z'
updated_at: '2026-01-06T19:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: board-roles-and-permissions
---

Hier erfährst du, wie du ein Passwort für deine öffentlichen Boards einrichten kannst und wie der Passwortschutz in den Preisplänen funktioniert.

> **Verfügbar für:** Board-Eigentümer, [Board-Miteigentümer](06-co-owners-of-boards-and-spaces.md) und Unternehmens-Admins in Enterprise-Preisplänen mit [Content Admin-Berechtigungen](../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md)
> **Relevant für:** Starter-, Business-, Enterprise- und Education-Preispläne
> **Verfügbar mit:** Browser, [Desktop-App](../../getting-started/apps-for-devices/05-desktop-app.md), [Tablet-App](../../getting-started/apps-for-devices/11-tablet-app.md)

## Passwörter für öffentliche Boards

Die Einladung von Besuchenden zu deinem Board über einen öffentlichen Link ist eine großartige Option für die sofortige, einmalige oder kurzfristige Zusammenarbeit mit Personen außerhalb deines Teams oder Unternehmens – auch Personen, die Miro nicht nutzen, können auf öffentliche Boards zugreifen.

Wenn du öffentliche Miro-Boards teilst, kannst du eine zusätzliche Sicherheitsebene einrichten, indem du ein Passwort festlegst.

### Passwortschutz auf Basis deines Preisplans

Der Passwortschutz und der Umfang der Berechtigungen hängen von deinem Preisplan ab.

|  |  |  |  |
| --- | --- | --- | --- |
|  | **Free** | **Starter, Business** | **Enterprise** |
| **Aktiviere, ändere oder entferne Passwörter** | ✘ | ✔  Board-Eigentümer, Miteigentümer | ✔  Board-Eigentümer, Miteigentümer, Unternehmens-Admins* |
| **Obligatorische Passwörter aktivieren** | ✘ | ✘ | ✔  [Ein obligatorisches Passwort festlegen](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md) |
| **Verlangt komplexe Passwörter** | ✘ | ✘ | ✔  [Erfordere ein komplexes Passwort](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md) |

*[Content-Admin](../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md) Berechtigungen müssen aktiviert sein.

:::note
Erfahren Sie mehr über unsere [Richtlinien zum Freigeben des Enterprise-Preisplans](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).
:::

## So fügst du einen Passwortschutz für ein Board hinzu

1. Wenn du den Zugriff auf **Jede Person mit Link** festlegst, klicke auf die  Schaltfläche **Passwort festlegen**.

2. Gib ein sicheres alphanumerisches Passwort mit mindestens 8 Zeichen ein und klicke dann auf **Festlegen**.

3. Das Passwort wird in deine Zwischenablage kopiert.

![3-1-720p-10fps-s4-r20.gif](../../../../../../docs/using-miro/sharing-boards/images/20257248240274_3-1-720p-10fps-s4-r20.gif)
*Ein Passwort für ein per Link freigegebenes Board setzen*

:::note
Enterprise-Preisplan Admins können [obligatorische Passwörter für alle Boards innerhalb des Abos festlegen](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).
:::

## Wie der Passwortschutz funktioniert

Nachdem du den Link zum Board erhalten und geöffnet hast, werden die Besucher aufgefordert, das Passwort einzugeben.

![3-2-720p-10fps-s4-r20.gif](../../../../../../docs/using-miro/sharing-boards/images/20257248243730_3-2-720p-10fps-s4-r20.gif)

Sobald sie das Passwort eingegeben haben, haben sie vollen Zugriff auf dein Board. Sie müssen das Passwort nur alle 72 Stunden neu eingeben.

Wenn sich die Nutzer häufiger anmelden müssen, hat der Miro-Admin des Unternehmens möglicherweise ein [Zeitlimit bei Inaktivität](../tools/troubleshooting/19-why-does-miro-keep-logging-me-out.md) festgelegt, um die Sicherheit zu erhöhen.

Bitte beachte, dass Boards, die passwortgeschützt sind, nur in den Listen „Favoriten“ und „Zuletzt verwendet“ angezeigt werden, solange sie für den Nutzer sichtbar sind.

Sobald die Sitzung für den Nutzer abläuft, sind die Boards für ihn nicht mehr verfügbar und werden aus den Listen „Favoriten“ und „Zuletzt verwendet“ entfernt. Wenn der Nutzer das Board über einen Direktlink öffnet und das Board-Passwort erneut eingibt, wird das Board wieder in den entsprechenden Listen angezeigt.

## Das Passwort für ein öffentliches Board ändern

Wenn du das Passwort änderst, wird der Zugang für alle Besucher des Boards sofort gesperrt, auch wenn sie gerade im Board sind.

:::note
Nutzer, die einen Link zu einem passwortgeschützten Board freigeben können, können das Passwort nicht ändern, es sei denn, sie sind Eigentümer oder Miteigentümer des Boards.
:::

**So änderst du das Passwort für ein öffentliches Board:**

1. Klicke auf **Passwort bearbeiten** in den Freigabeeinstellungen und dann auf **Passwort ändern**.
![3-1.png](../../../../../../docs/using-miro/sharing-boards/images/20235526720658_3-1.png)
*Ein Board-Passwort in den Freigabeeinstellungen bearbeiten*
2. Es erscheint ein Bestätigungsfenster, in dem du darauf hingewiesen wirst, dass du das neue Passwort bestehenden Mitwirkende mitteilen musst, damit diese weiterhin auf das Board zugreifen können. Klicke auf **Passwort ändern**.

![passwort_ändern.png](../../../../../../docs/using-miro/sharing-boards/images/20022115780754_change_password.png)
*Fenster zur Bestätigung der Passwortänderung*
3. Gib ein sicheres alphanumerisches Passwort mit mindestens 8 Zeichen ein.
Dein Admin hat möglicherweise bestimmte Passwortanforderungen für dein Konto festgelegt. Wenn du dein Passwort erstellst, werden die erforderlichen Kriterien deutlich angezeigt, um dich zu leiten.
![Die Passwortanforderungen werden angezeigt, wenn du dein Passwort eingibst.](../../../../../../docs/using-miro/sharing-boards/images/23762870609298_image.png)*Die Passwortanforderungen werden bei der Eingabe deines Passworts angezeigt.*

4. Klicke auf **Passwort festlegen**.

:::note
Wenn du das Passwort änderst, wird der Zugriff für alle Besucher des Boards sofort gesperrt, auch wenn sie gerade im Board sind.
:::

## Deaktivierung eines öffentlichen Links

Du kannst [aufhören, ein öffentliches Board freizugeben](03-sharing-boards-and-inviting-collaborators.md) Du kannst die Freigabe eines öffentlichen Boards jederzeit beenden, allerdings wird dadurch nicht automatisch das Passwort für dein Board zurückgesetzt. Um Besuchern den Zugriff auf das Board mit demselben Passwort zu aktivieren, musst du das Board erneut per Link freigeben.

Um zu erfahren, wie du das Passwort ändern kannst, siehe Das Passwort für ein öffentliches Board ändern.

## Ich habe das Passwort für mein Board vergessen

Wenn du das Passwort vergisst, kannst du ganz einfach dein Board-Passwort ändern in den Einstellungen zum Freigeben ändern.

:::note
Die Einrichtung eines Passwortschutzes für Boards für Mobilgeräte ist in unserem Backlog.
:::
