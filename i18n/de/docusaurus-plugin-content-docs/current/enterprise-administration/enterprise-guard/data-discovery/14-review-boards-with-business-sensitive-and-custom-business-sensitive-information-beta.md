---
title: "Boards mit gesch\xE4ftskritischen und benutzerdefinierten, gesch\xE4ftskritischen\
  \ Informationen \xFCberpr\xFCfen (Beta)"
article_id: 24090123693586
translation_id: 24090123693586
locale: de
sidebar_position: 13
created_at: '2025-01-21T15:10:56Z'
updated_at: '2025-11-25T16:22:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

Über die Inhaltssuche können [Admins für sensible Inhalte](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) Vorkommen von geschäftskritischen oder benutzerdefinierten geschäftskritischen Daten überprüfen.

:::note
- Um Boards mit geschäftskritischen oder benutzerdefiniert geschäftskritischen Daten zu überprüfen, musst du die [Rolle des Admins für sensible Inhalte](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Um die Rolle des Admins für sensible Inhalte anzufordern, kontaktiere deinen Unternehmens-Admin.
- Übereinstimmungen mit geschäftskritischen Daten werden entweder als CUSTOMER, TECH oder STRATEGY gekennzeichnet und die Ergebnisse werden oben in der Ergebnisliste aufgeführt.

– Übereinstimmungen mit benutzerdefinierten geschäftskritischen Daten werden mit den entsprechenden benutzerdefinierten Labels versehen.
:::

Um ein Board mit geschäftskritischen oder benutzerdefinierten geschäftskritischen Daten zu überprüfen, führe folgende Schritte aus:

1. Wenn du auf der Seite **Content Explorer** bist, fahre mit Schritt 2 fort.
   Wenn du dich nicht auf der Seite **Content Explorer** befindest:
   a. Gehe zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
   b. Klicke im linken Bereich unter **Enterprise Guard** auf **Content Explorer**.
   c. Klicke auf **Data Discovery**.
2. Klicke auf der Seite **Inhaltssuche/Datenerkennung** auf das Board, das du überprüfen möchtest.
   Rechts auf dem Bildschirm wird ein ausklappbarer Bereich angezeigt.
3. Im ausklappbaren Bereich kannst du folgende Aktionen ausführen:

   - Nur für benutzerdefinierte Abgleiche geschäftskritischer Daten: **geschäftskritische Informationen** anzeigen oder ausblenden
   Standardmäßig sind benutzerdefinierte **geschäftskritische Informationen** geschwärzt. Wenn du benutzerdefinierte geschäftskritische Daten ansehen möchtest, aktiviere den Schalter **Geschäftskritische Informationen anzeigen**.
   geschäftskritische Daten sichtbar sind, kannst du die Daten ausblenden, indem du auf die Schaltfläche **Sensible Informationen anzeigen** klickst, um sie zu deaktivieren.

   > ✏️ - Geschäftskritische Daten werden als entweder CUSTOMER, TECH oder STRATEGY markiert und die Ergebnisse werden oben in der Ergebnisliste aufgeführt.
   > - Übereinstimmungen mit benutzerdefinierten geschäftskritischen Daten werden mit den entsprechenden benutzerdefinierten Labels versehen.

   - Sowohl für geschäftskritische Daten als auch für benutzerdefinierte geschäftskritische Daten: **Informationen basierend auf der Kategorie für geschäftskritische Daten filtern**
   Um geschäftskritische Daten anzusehen, die zu einer bestimmten Kategorie gehören, klicke auf den Tab **Geschäftskritische Informationen** und klicke dann auf die entsprechende Filterschaltfläche unter dem Tab.

   -Nur für Übereinstimmungen mit geschäftskritischen Daten: **Falsch-positive Übereinstimmungen unterdrücken**
   Bei der Erkennung geschäftskritischer Daten kannst du auf Situationen stoßen, in denen das System Übereinstimmungen generiert, die zwar theoretisch korrekt sind, aber basierend auf verschiedenen Sicherheitsrichtlinien und spezifischen Anforderungen einer Organisation möglicherweise nicht relevant oder nicht als sensible Daten erachtet werden. Das Unterdrücken einer Übereinstimmung, die kein Sicherheits- oder Geschäftsrisiko darstellt, ist entscheidend, um den Prozess der Datenerkennung an die spezifischen Datensicherheits- und Geschäftsanforderungen einer Organisation anzupassen.

   Es kann auch vorkommen, dass das System Daten auf deinen Boards fälschlicherweise als wahrscheinlich sensibel kennzeichnet (ein falsches positives Ergebnis). Dies wird von verschiedenen Faktoren beeinflusst, z. B. von der Nähe verwandter Begriffe oder der Formatierung von geschäftsbezogenen Daten. Du kannst auch falsch positive Übereinstimmungen unterdrücken.

   Wenn du eine Übereinstimmung unterdrückst, erfolgen die Updates in Echtzeit. Die Board-Klassifizierung und die angewendeten Vorgaben werden auch gemäß der Konfiguration für die automatische Klassifizierung und intelligente Vorgaben aktualisiert.

   Um eine falsch-positive Übereinstimmung zu unterdrücken, klicke auf die drei Punkte neben der geschäftskritischen Datenübereinstimmung, die du unterdrücken möchtest, und wähle dann **Übereinstimmung verbergen**. Beachte, dass die Updates in Echtzeit erfolgen. Die Board-Klassifizierung und die angewendeten Vorgaben werden auch gemäß der Konfiguration für die automatische Klassifizierung und intelligente Vorgaben aktualisiert.
4. Klicke in der Ergebnisliste der Inhaltssuche auf das nächste Board, mit dem du arbeiten möchtest, und führe die notwendigen Aktionen aus, oder schließe das ausklappbare Feld, indem du oben rechts im Feld auf die Schaltfläche **Schließen** klickst.
