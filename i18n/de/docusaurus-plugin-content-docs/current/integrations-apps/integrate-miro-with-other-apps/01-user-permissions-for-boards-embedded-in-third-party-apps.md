---
title: Nutzerberechtigungen für Boards, die in Apps von Drittanbietern eingebettet
  sind
article_id: 4411883577618
translation_id: 4411883577618
locale: de
sidebar_position: 1
created_at: '2021-12-08T10:13:42Z'
updated_at: '2025-11-25T16:07:55Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
availability:
  notes: 'Personen: Board-Eigentümer, Board-Miteigentümer Preispläne: Alle Preispläne
    Plattformen: Browser, Desktop-App'
---

Miro bietet mehrere Integrationen, die die Zusammenarbeit mit Boards in Drittanbieter-Umgebungen wie [Microsoft Teams](../microsoft), [Confluence](../atlassian/01-miro-for-confluence.md), Notion und Google Meet ermöglichen. Du kannst weitere unterstützte Apps im [Miro Marketplace](https://miro.com/marketplace/category/embed-miro/) entdecken. Beim Einbetten von Boards kannst du verschiedene Zugriffsebenen für Nutzer festlegen und diese Berechtigungen direkt in Miro verwalten.

## Zugriff auf Einbettungen verstehen

Wenn du ein Board in einer externen App teilst, kannst du Nutzern dieser App unabhängig von ihrem Miro-Zugang Zugriff zum Ansehen, Kommentieren oder Bearbeiten für eine einmalige Zusammenarbeit gewähren. Diese Nutzer benötigen kein Miro-Profil, um auf das Board innerhalb der App zuzugreifen. So kannst du bestimmte Zugriffsrechte für Boards erteilen und Nutzer der App, die nicht bei Miro registriert sind, können damit arbeiten, ohne dass du das Board öffentlich zugänglich machen musst.

Um maximale Sicherheit zu gewährleisten, raten wir davon ab, diese Methode außerhalb einer einmaligen Zusammenarbeit (z. B. bei einem Workshop) zu verwenden, und empfehlen, dass deine Organisation Nutzern bei Bedarf einen entsprechenden Miro-Zugang zuweist.

![embed_Miro_in_Zoom.gif](../../../../../../docs/integrations-apps/integrate-miro-with-other-apps/images/21020254296722_embed%20Miro%20in%20Zoom.gif) *Einrichten von Zugriffsrechten für ein eingebettetes Board*

Der Zugriff auf das Board ist nur in der App möglich, in der es eingebettet wurde. Die Zugriffsebene, die du für ein eingebettetes Board in der App einstellst, hat keinen Einfluss auf die Einstellungen zum Teilen des Boards außerhalb der App. Zum Beispiel können Nutzer in einem Microsoft Teams-Kanal auf das Board zugreifen, ohne sich bei Miro anzumelden, wenn ein [privates Board](../../using-miro/sharing-boards/15-make-a-miro-board-private.md) mit der Zugriffsberechtigung „Alle können ansehen“ eingebettet ist. Wenn dieselben Nutzer versuchen, auf das Board außerhalb des Microsoft Teams-Kanals zuzugreifen, indem sie dem Board-Link folgen, haben sie keinen Zugriff.

Bitte beachte jedoch, dass die Freigabeeinstellungen für das Board auf der Miro-Seite Vorrang vor der in der externen App festgelegten Zugriffsebene haben. Wenn ein Board beispielsweise [öffentlich auf Seiten von Miro freigegeben wird](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), ist es für jeden in Microsoft Teams verfügbar, selbst wenn du das Board als Privat eingebettet hast.

## Zugriff auf Einbettungen verwalten und widerrufen

Du kannst den Zugriff auf Boards, die in unterstützte externe Apps eingebettet sind, ganz einfach nachverfolgen, verwalten und widerrufen.

So verwaltest und entziehst du Zugriffsrechte für eingebettete Boards:

1. Klicke auf die Schaltfläche **Freigeben**, um die Freigabeeinstellungen eines Miro-Boards zu öffnen.
2. Wähle **Freigabeeinstellungen** aus.
3. Öffne den **Tab** Einbettungen.
4. Du siehst die externen Apps, in denen das Board eingebettet ist, einschließlich des Namens der Integration, wann und von wem es eingebettet wurde, sowie die Board-Zugriffseinstellungen innerhalb der App.
5. Um den Zugriff auf das Board in einer App zu widerrufen, klicke auf **Zugriff widerrufen** neben der App. Bitte beachte: Diese Aktion kann nicht rückgängig gemacht werden.

ol

![remove_an_access_link.gif](../../../../../../docs/integrations-apps/integrate-miro-with-other-apps/images/21020265344914_remove%20an%20access%20link.gif)
*Entfernen eines Zugrifflinks*

Nachdem der Einbettungszugriff widerrufen wurde, ist der Board-Zugriff in der App eingeschränkt. Beachte, dass das Board möglicherweise immer noch in der App zugänglich ist, wenn es auf Seiten von Miro freigegeben wurde. Zum Beispiel:

- Wenn alle das Board in der **App** **bearbeiten** können und dasselbe Board auf der Miro-Seite [öffentlich freigegeben](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) ist, können alle das Board in der App weiterhin **ansehen**.
- Wenn das Board privat ist und nur [per E-Mail mit anderen Nutzern geteilt wird](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), ist für den Zugriff auf das eingebettete Board die **Anmeldung** in der App erforderlich.

## Einbettungsregeln und Einschränkungen

Bitte beachte die folgenden Regeln und Einschränkungen beim Einbetten von Boards:

- Du kannst ein Board nicht einbetten, wenn es [inaktiv](../../using-miro/tools/troubleshooting/15-the-board-is-locked.md) ist oder du nur Ansichtsrechte für das Board hast.
- Boards, die in [Free-Teams](../../plans-billing/miro-plans/09-free-plan.md) gespeichert sind, können nicht mit Kommentarzugriff eingebettet werden.
- Für Nutzer im [Enterprise-Preisplan](../../plans-billing/miro-plans/04-enterprise-plan.md) folgen die Zugriffseinstellungen den organisationsweiten Zugriffskontrollen, die möglicherweise einige Freigabeoptionen einschränken können. Mehr erfahren: [Freigaberichtlinie bei Enterprise-Preisplänen für die Einbettung von Integrationen verwalten](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
- Bei einigen alten Links siehst du nur die Zugriffsebene und die App, aber nicht, wer das Board erstellt hat oder wann es eingebettet wurde.
- Wenn du das Einbetten von Miro-Boards in externe Apps für deine Enterprise-Organisation beschränken möchtest, findest du alle nötigen Infos unter [Freigaberichtlinie bei Enterprise-Preisplänen für Einbettungsintegrationen verwalten](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
- Die Verwaltung von eingebetteten Board-Zugriffslinks wird auf mobilen und Tablet-Geräten noch nicht unterstützt.

Erfahre mehr über den Zugriff auf eingebettete Boards für Nutzer mit [kostenlosen eingeschränkten Lizenzen](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).
