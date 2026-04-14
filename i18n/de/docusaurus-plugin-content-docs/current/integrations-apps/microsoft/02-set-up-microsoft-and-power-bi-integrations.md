---
title: Die Microsoft- und Power BI-Integrationen einrichten
article_id: 25132703621394
translation_id: 25132703621394
locale: de
sidebar_position: 3
created_at: '2025-03-06T10:27:14Z'
updated_at: '2025-11-25T15:49:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: powerbi
---

:::note
Für umfassende Admin-Dokumente speziell zur Miro-Integration mit Microsoft oder Power BI, einschließlich detaillierter Diagramme und weiterer FAQs, siehe bitte die [Microsoft Admin-Dokumentation](https://docs.google.com/document/d/1Gw94z5Pc-elS-pRXKGZVBWKKNEIFR9y9yzAAkbXKwMM/edit?usp=sharing) oder die [Power BI Admin-Dokumentation](https://docs.google.com/document/d/1hMepF163jQF8LI-U8ES8DzHVMW4TltXDr14fJ2KU29k/edit?tab=t.0#heading=h.gu9ng058yy7y).
:::

In diesem Artikel wird erläutert, wie du eine Microsoft- oder Power BI-Integration mit Miro einrichtest.

## Die Microsoft- oder Power BI-Integration einrichten

Um eine Microsoft- oder Power BI-Integration einzurichten, musst du Nutzer aktivieren, ihre eigenen Microsoft- oder Power BI-Inhalte in Miro zu autorisieren.

### Voraussetzungen

- Vergewissere dich, dass du Admin-Zugriff auf Microsoft Entra hast.
- Ein Unternehmens-Admin hat Microsoft oder Power BI für eure Miro-Organisation freigegeben (dies bezieht sich auf die Miro-seitigen App-Bewilligungsrichtlinien, falls eure Organisation App-Installationen einschränkt).

### Vorgehensweise

Diese Schritte konzentrieren sich darauf, Microsoft Entra so zu konfigurieren, dass die Miro-Integration ermöglicht wird.

1. Melde dich bei **Entra** als Admin an.
2. Gehe zu **Enterprise-Apps** > **Einwilligung und Berechtigungen**.
3. Wähle für **Nutzer können die Admin-Zustimmung für Apps anfordern, denen sie nicht zustimmen können** **Ja** aus.
4. Unter **Wer kann Admin-Zustimmungsanfragen überprüfen**, wähle die erforderlichen Nutzer, Rollen oder Gruppen aus, die du für die Überprüfung von Admin-Zustimmungsanfragen für Anwendungen zulassen möchtest.

:::note
Die in Schritt 4 ausgewählten Entra-Admins können dann in Microsoft Entra zu **Enterprise-Apps > Admin-Genehmigungsanfragen** gehen, um die Anwendung "Contenthub PowerBI Integratio" (oder eine ähnlich benannte) für die Organisation zu überprüfen und zu genehmigen.
:::

## Validiere deine Microsoft- oder PowerBI-Integration

Kopiere einen Link zu deinem Miro-Board und füge ihn ein.

Wenn die App von deinem Unternehmens-Admin vorab genehmigt wurde, folge den Anweisungen im Dialogfeld auf dem Bildschirm. Miro fügt deine App-Inhalte als iFrame dem Board hinzu.

Wenn die App nicht vorab genehmigt ist, öffnet sich das **Add & allow**-Dialogfeld und ermöglicht es dir, eine Anfrage an deinen Unternehmens-Admin zu senden. Anfrage senden

Wenn dein Unternehmens-Admin antwortet, erhältst du eine Benachrichtigung.

**Weitere Informationen:** Siehe [App-Verwaltung](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).
