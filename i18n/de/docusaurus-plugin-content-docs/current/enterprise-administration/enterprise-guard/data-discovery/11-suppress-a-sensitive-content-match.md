---
title: "\xDCbereinstimmung mit vertraulichen Inhalten ausschlie\xDFen"
article_id: 17144258002962
translation_id: 17144258002962
locale: de
sidebar_position: 10
created_at: '2024-02-20T00:16:59Z'
updated_at: '2025-11-25T15:41:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

Während der Datenerkennung kann es vorkommen, dass das System Übereinstimmungen generiert, die zwar technisch korrekt sind, aber auf der Grundlage verschiedener Sicherheitsrichtlinien und spezifischer Bedürfnisse eines Unternehmens möglicherweise nicht relevant sind oder als vertrauliche Daten angesehen werden. Das Ausschließen einer Übereinstimmung, die kein Sicherheits- oder Datenschutzrisiko darstellt, ist entscheidend, um den Datenerkennungsprozess an die spezifischen Datensicherheits- und Datenschutzanforderungen eines Unternehmens anzupassen.

Es kann auch vorkommen, dass das System Daten auf deinen Boards fälschlicherweise als wahrscheinlich vertraulich kennzeichnet (falsch-positiv). Verschiedene Faktoren tragen zu diesen Ergebnissen bei, zum Beispiel nahe verwandte Begriffe oder die Formatierung vertraulicher Daten. Du kannst diese falsch-positiven Übereinstimmungen auch ausschließen.

Wenn du eine Übereinstimmung ausschließt, erfolgen die Aktualisierungen in Echtzeit. Die Board-Klassifizierung und die angewandten Vorgaben werden ebenfalls gemäß der Konfiguration der automatischen Klassifizierung und der intelligenten Vorgaben aktualisiert.

:::note
Um eine Übereinstimmung mit vertraulichen Inhalten auszuschließen, musst du die [Rolle des Admins für vertrauliche Inhalte](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Wende dich an den Unternehmensadministrator, um die Admin-Rolle „Vertrauliche Inhalte“ anzufordern.
:::

Führe folgende Schritte aus, um eine Übereinstimmung mit vertraulichen Inhalten auszuschließen:

1. Wenn du dich auf der Seite des **Inhalts-Explorers** befindest, überspringe den 1. Schritt.
   Wenn du dich nicht auf der Seite des **Inhalts-Explorers** befindest:
   a. Gehe zu deinen [Miro-Einstellungen.](https://help.miro.com/hc/articles/https://miro.com/app/settings)
   b. Klicke im linken Bereich unter **Sicherheit & Compliance** auf **Inhalts-Explorer**.
2. Klicke auf der Seite **Inhalts-Explorer/Datenerkennung** auf das Board, das du überprüfen möchtest.
   Auf der rechten Seite des Bildschirms wird ein erweiterbares Panel angezeigt.
   ![Abbildung 1: Erweiterbares Panel](images/17165300023954_slide_out_panel.png)*Abbildung 1: Erweiterbares Panel*
3. Klicke auf die Auslassungspunkte neben der Übereinstimmung mit vertraulichen Daten, die du ausschließen möchtest, und wähle dann **Übereinstimmung ausblenden** aus. Beachte, dass die Aktualisierungen in Echtzeit erfolgen. Die Board-Klassifizierung und die angewandten Vorgaben werden ebenfalls gemäß der Konfiguration der automatischen Klassifizierung und der intelligenten Vorgaben aktualisiert.

    Wenn du eine Übereinstimmung ausschließt, erfolgen die Aktualisierungen in Echtzeit. Die Board-Klassifizierung und die angewandten Vorgaben werden ebenfalls gemäß der Konfiguration der automatischen Klassifizierung und der intelligenten Vorgaben aktualisiert.

   Wiederhole diesen Schritt für jede Übereinstimmung mit vertraulichen Daten, die du ausschließen möchtest.
4. Du kannst auf das nächste Board in der Ergebnisliste des Inhalts-Explorers klicken und die erforderlichen Aktionen ausführen, oder du kannst das erweiterbare Panel schließen, indem du oben rechts im Panel auf **Schließen** klickst.
