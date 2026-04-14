---
title: Datenklassifizierung
article_id: 4417739162258
translation_id: 4417739162258
locale: de
sidebar_position: 2
created_at: '2022-02-07T10:01:21Z'
updated_at: '2025-02-26T12:17:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Mithilfe der Datenklassifizierung können Personen im Enterprise-Preisplan ihren Boards Labels geben, um die Vertraulichkeit des Board-Inhalts festzulegen.

> **Verfügbar für**: Enterprise-Preisplan
> **Verfügbar auf**: Desktop, Tablet
> **Verfügbar für:** Unternehmens-Admins

Die Einstellungen für die Klassifizierung von Daten findest du in der Enterprise Admin-Konsole. Gehe zu **Einstellungen** und wähle **Klassifizierung**.

:::note
Für Kunden mit Enterprise Guard findest du die **Klassifizierung** in der Admin-Konsole unter **Enterprise Guard**. Gehe zu **Einstellungen** > **Enterprise Guard** > Klassifizierung.
:::

Vergewissere dich, dass du die folgenden wichtigen Punkte zur Klassifizierung von Daten verstehst:

- Die Klassifizierung der Daten ist ein internes Label und hat keinen Einfluss auf die Einstellungen zum Freigeben von Boards. Das bedeutet, dass Boards über ihre Klassifizierung hinaus freigegeben werden können.
- Boards, die vor der Einführung dieser Funktion erstellt wurden, werden als „nicht klassifiziert“ gekennzeichnet.
- Bei der [Duplikation eines Boards](../../../using-miro/managing-boards/03-how-to-duplicate-a-board.md) wird das aktuelle Datenklassifizierungslabel auch für die neue Board-Kopie verwendet.
- Die Labels werden derzeit weder im [Präsentationsmodus](https://help.miro.com/hc/articles/360017731073) noch im [Smart-Meetings-Modus](https://help.miro.com/hc/articles/4408834812690) oder auf Mobilgeräten angezeigt.

## Wie man Labels zur Klassifizierung einrichtet

In den **Einstellungen** wählst du **Klassifizierung**. Um Klassifizierungs-Labels für deine Unternehmensorganisation zu aktivieren, wähle **Klassifizierung einrichten.**

## So fügst du neue Labels zur Klassifizierung hinzu

Unternehmens-Admins können bis zu 30 Klassifizierungs-Labels erstellen und anpassen sowie ein Standard-Label für alle neuen Boards im Unternehmen festlegen.

In den Einstellungen zur **Klassifizierung** sind bereits vier Labels angelegt, die du anpassen kannst. Du kannst auch neue Labels erstellen, die deinen organisatorischen Anforderungen entsprechen.

So erstellst du eine neue Klassifizierung:

1. Wähle **Klassifizierungsstufen bearbeiten** aus.
2. Klicke auf **Ebene hinzufügen**
3. Lege die **Stufe** der Klassifizierung fest, füge einen **Namen** und eine **Beschreibung** hinzu und ändere die **Badge-Farbe**
4. Wenn du für Personen, die das Board nutzen, einen Verweis hinzufügen möchtest, füge einen **Link zu den Richtlinien** hinzu.
5. (Optional) Wähle **Vorschau** , um zu sehen, wie dein Label in der Produktion aussehen wird.
6. Wähle **Fertig** aus.
7. (Optional) Um deine Labels für die Klassifizierung neu zu ordnen, klicke auf die Pfeile nach oben**(Ʌ)** oder unten**(V**).
8. **Klicke auf Veröffentlichen, damit die Änderungen übernommen werden**

> Wenn du ein Klassifizierungslabel erstellst oder bearbeitest, werden deine Änderungen als Entwurf gespeichert und erst veröffentlicht, wenn du auf **Veröffentlichen** klickst. Das bedeutet, dass du die Klassifizierungskonfiguration jederzeit verlassen und zur Klassifizierung zurückkehren kannst.

Du kannst auch einen Link zu den Klassifizierungsrichtlinien deines Unternehmens hinzufügen, in denen Mitwirkende mehr über die bestehenden Datenklassifizierungsrichtlinien erfahren können.

![](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/23921802487570_image.png)

*Link zu Klassifizierungsrichtlinien*

## Wie du Klassifizierungsentwürfe anpasst

So bearbeitest du eine Klassifizierung, **ohne** dass ein Entwurf gespeichert wird:

1. Klicke auf **Klassifizierungsebenen bearbeiten**
2. Klicke auf Bleistiftsymbol zum **Bearbeiten**
3. Nimm deine Änderungen vor und klicke auf **Fertig**
4. **Klicke auf Veröffentlichen, damit die Änderungen übernommen werden**

So bearbeitest du eine Klassifizierung, **sodass** ein Entwurf gespeichert wird:

1. Klicke im Panel Datenklassifizierung auf **Konfiguration fortsetzen**
2. Klicke auf Bleistiftsymbol zum **Bearbeiten**
3. Nimm deine Änderungen vor und klicke auf **Fertig**
4. **Klicke auf Veröffentlichen, damit die Änderungen übernommen werden**

## So löschst du ein Label zur Klassifizierung

Klicke zum Löschen eines Labels auf das Papierkorbsymbol. Beachte, dass du das Standardlabel nicht löschen kannst.

![data_classification_delete_label.pngLöschen](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017013528978_data_classification_delete_label.png)
*eines Labels*

### Standardlabel auf Unternehmensebene hinzufügen

Wähle ein Standard Label für die Klassifizierung neu erstellter Boards. Jedes neue Board, das in der Unternehmensorganisation erstellt wird, erhält das Standard Label.

Um ein Standard Label für deine Organisation einzurichten, markiere **Standard Klassifizierungslabel** , wenn du ein Klassifizierungslabel hinzufügst oder bearbeitest.

![Einrichten des Standard Labels für die Klassifizierung von Daten](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/23921802487570_image.png)

*Standard-Klassifizierungslabel einrichten*

### Standardlabel auf Teamebene hinzufügen

> **Einrichtung durch:** Unternehmens-Admins, Team-Admins

Unternehmens- und Team-Admins können das **Standardlabel überschreiben** und ein eigenes Standardlabel auf Teamebene einrichten: Jedem neuen, im Team erstellten Board wird das neue Standardlabel zugewiesen und das Standardlabel auf Unternehmensebene vernachlässigt.

Um diese Einstellung zu aktivieren, gehe zu den Teameinstellungen > **Berechtigungen** und scrolle nach unten.

Beachte, dass du im Team das Label nur überschreiben kannst, wenn die Einstellung für die Datenklassifizierung auf Unternehmensebene aktiviert ist.

Für [neu erstellte Teams](../../managing-enterprise-teams-and-content/09-create-a-new-team-on-enterprise-plan.md) ist diese Einstellung deaktiviert, wenn du beim Erstellen des Teams die Standardeinstellungen auswählst.

### Boards Klassifizierunglabels hinzufügen

> **Einrichtung durch:** [Board-Eigentümer](../../../using-miro/sharing-boards/01-board-access-rights.md), [Board-Miteigentümer](../../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md), Bearbeitende, die Mitglieder des Teams sind, Unternehme[ns-Admins mit Berechtigungen als](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md) Inhalts-Admins

Wenn die Datenklassifizierung in den Einstellungen unter Unternehmen aktiviert ist, können Personen die Board-Labels sehen und ändern. Das Datenklassifizierungslabel wird neben dem Namen des Boards als Badge angezeigt. Wenn du mit dem Mauszeiger über das Badge gehst, werden der Name und die Beschreibung des Labels angezeigt.

[Board-Eigentümer,](../../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md) [Board-Miteigentümer](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md), Bearbeitende, die Mitglieder des Teams sind, und Unternehmens-Admins mit Berechtigungen als Inhalts-Admins können das Klassifizierungslabel entweder durch Klicken auf das Badge oder in den Board-Details aktualisieren. Wähle ein Label aus und klicke auf Aktualisieren. Wenn deine Unternehmens-Admins in den Einstellungen einen Link zu den Richtlinien bereitgestellt haben, kannst du auf den Link im Pop-up klicken, um weitere Details zu erhalten.

![data_classification_adding_labels_to_boards.gifDas](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017043043090_data_classification_adding_labels_to_boards.gif)
*Label für die Klassifizierung der Daten auf dem Board*

### Datenklassifizierungsfilter auf dem Dashboard

Alle Personen, bei denen im Enterprise-Preisplan die Datenklassifizierung aktiviert ist, können auf dem Dashboard ihre Boards nach Labels filtern. Standardmäßig ist **Jede Klassifizierung** ausgewählt.

![data_classification_classification_filter.pngBoard-Klassifizierungsfilter](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017043043986_data_classification_classification_filter.png)
*auf dem Dashboard*
