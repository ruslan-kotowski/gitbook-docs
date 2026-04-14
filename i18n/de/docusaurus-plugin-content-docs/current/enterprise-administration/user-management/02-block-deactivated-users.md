---
title: Deaktivierte Personen blockieren
article_id: 11846063620882
translation_id: 11846063620882
locale: de
sidebar_position: 2
created_at: '2023-06-06T12:47:53Z'
updated_at: '2025-11-04T11:30:33Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-deactivation
---

Wenn ein Unternehmens-Admin [jemanden deaktiviert](01-deactivated-users.md), verliert diese Person den Zugriff auf das Enterprise-Abo und kann sich nicht mehr über SSO anmelden. Deaktivierte Personen können aber mit derselben E-Mail-Adresse weiterhin auf andere Miro-Abos zugreifen.

Du kannst deaktivierte, [verwaltete Personen](06-managed-users-on-enterprise-plan.md) weiter blockieren, um zu verhindern, dass sie auf andere Miro-Abos zugreifen.

> **Erhältlich für: Enterprise-Preisplan
> **Verfügbar für:** Unternehmens-Admins**

## Deaktivierte Personen blockieren

**Wenn die Einstellung aktiviert ist,** verlieren deaktivierte, verwaltete Personen den Zugriff auf alle Miro-Abos. Diese Einstellung gilt für alle Personen, die derzeit in deinem Abo deaktiviert sind, sowie für alle Personen, die du in Zukunft deaktivierst.

**Wenn die Einstellung deaktiviert ist,** können deaktivierte, verwaltete Personen mit ihrer Unternehmens-E-Mail-Adresse und ihrem Passwort weiterhin auf andere Miro-Abos zugreifen.

>  Die Aktivierung der Einstellung **Deaktivierte Personen blockieren** wirkt sich auf alle bereits deaktivierten Personen in deinem Abo aus. Bevor du die Einstellung aktivierst oder neue Domains verifizierst, während die Einstellung aktiviert ist, empfehlen wir, zuerst die Liste der deaktivierten Personen zu überprüfen, um festzustellen, wer blockiert wird.

### So blockierst du deaktivierte Personen

1. Gehe zu **Einstellungen** > **Sicherheit** > **Verwaltete Domains**
2. Aktiviere **Deaktivierte Personen blockieren**
   *![Deaktivierte Nutzer in der Enterprise Admin-Konsole sperren](../../../../../../docs/enterprise-administration/user-management/images/23921780232082_image.png)*
   *Blockiere deaktivierte Nutzer in der Enterprise Admin-Konsole.*

## Was sehen blockierte Personen?

Blockierte und deaktivierte verwaltete Personen werden sofort abgemeldet. Wenn sie sich erneut anmelden möchten, sehen sie eine der folgenden Nachrichten:

![Konto](../../../../../../docs/enterprise-administration/user-management/images/21017430794898_Account%20deactivated.png)*Nutzer hat versucht, sich mit E-Mail und Passwort anzumelden*

![E-Mail](../../../../../../docs/enterprise-administration/user-management/images/21017417753746_Email%20not%20associated%20with%20an%20SSO%20account.png)*Nutzer hat versucht, sich mit SSO anzumelden*

## Blockierung für deaktivierte Personen aufheben

Unternehmens-Admins können die Blockierung von Personen auf drei Arten aufheben:

**Die Person reaktivieren oder erneut einladen**

Du kannst die Person reaktivieren oder erneut zu deinem Enterprise-Abo einladen, in dem die Domain verifiziert ist. Diese Person erhält Zugriff auf alle ihr zugeordneten Abos. Wenn diese Person dein Enterprise-Abo nicht aktiv verwendet, kannst du ihr eine [eingeschränkte kostenlose](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) Lizenz zuweisen. Weitere Informationen zum Einladen von Mitgliedern findest du unter Einladungen im Enterprise-Preisplan verwalten.

**Einstellung „Deaktivierte Personen blockieren“ deaktivieren**

Dadurch wird die Blockierung aller deaktivierten, verwalteten Personen aufgehoben. Sie können sich nun mit ihrer Unternehmens-E-Mail-Adresse bei Miro anmelden. Sie erhalten damit aber keinen Zugriff auf dein Enterprise-Abo. Diese Option funktioniert nur, wenn die Person nicht aus dem Abo gelöscht wurde. Geh zu den Einstellungen für **Verwaltete Domains** und deaktiviere **Deaktivierte Personen blockieren.**

**Die Domain löschen**

Du kannst die Domain aus der Liste der verifizierten Domains löschen. Dadurch wird die Blockierung aller verwalteten Personen von dieser Domain aufgehoben, es sei denn, sie wurden aus dem Abo gelöscht. Um eine Domain zu löschen, geh in den Einstellungen deines Unternehmens zu **Sicherheit & Compliance** > **Zusammenarbeit** > und klick neben dem Domain-Namen auf **Entfernen**.

> **✏️** Wenn der Zugriff einer Person auf Miro blockiert wird, kann sie sich weder mit ihrer Unternehmens-E-Mail-Adresse und ihrem Passwort noch über SSO bei anderen Miro-Abos anmelden. Die Aufhebung der Blockierung gewährt der Person keinen Zugriff auf das Enterprise-Abo, es sei denn, es wurde ihr explizit Zugriff gewährt.

## Szenarien für blockierte Personen

In dieser Tabelle siehst du, was in den verschiedenen Szenarien mit den blockierten Personen passiert.

|  |  |
| --- | --- |
| Aktion | Ergebnis |
| **Person ist blockiert** | |
| Unternehmens-Admin deaktiviert verwalteten Nutzer | Person ist blockiert |
| **Ein Mitglied deines Enterprise-Abos versucht, eine** deaktivierte, verwaltete Person in sein Team einzuladen | Person bleibt blockiert.  Die einladende Person sieht eine Nachricht, dass die Person deaktiviert ist. Sie kann nicht eingeladen werden. Admins können Personen reaktivieren. |
| Ein Unternehmens-Admin deaktiviert einen verwalteten Nutzer und löscht ihn | Person ist blockiert |
| Die verwaltete Person wird im IdP deaktiviert | Person ist blockiert |
| Die verwaltete Person wird im IdP aus der Miro-App/Gruppe entfernt | Person ist blockiert |
| Ein Unternehmens-Admin fügt eine Domain hinzu und überprüft sie, während die Einstellung aktiviert ist | Alle Personen aus den neu verifizierten Domains in der deaktivierten Liste werden blockiert. |
| Jemand aus einem anderen Abo (jedes andere Abo außer dem, für das die Domain überprüft wird) versucht, die deaktivierte, verwaltete Person zu ihrem Abo einzuladen.   Dies gilt auch, wenn die verwaltete Person aus deinem Abo gelöscht wird. | Person bleibt blockiert.  Sie kann zu anderen Abos eingeladen werden und erhält dann Einladungsbenachrichtigungen, kann sich jedoch nicht bei Miro anmelden. |
| **Blockierung der Person wird aufgehoben** | |
| Unternehmens-Admin reaktiviert einen deaktivierten, verwalteten Nutzer | Blockierung der Person wird aufgehoben |
| Ein Unternehmens-Admin lädt einen deaktiviertenn oder gelöschte, verwalteten Nutzer wieder zum Abo ein. | Person wird eingeladen und die Blockierung aufgehoben |
| Die verwaltete Person wird über SCIM reaktiviert | Blockierung der Person wird aufgehoben |
| Die verwaltete Person wird im IdP zur Miro-App/Gruppe wieder hinzugefügt und über SCIM synchronisiert | Blockierung der Person wird aufgehoben |
| **Ein Mitglied deines Enterprise-Abos lädt eine** gelöschte, verwaltete Person zu seinem Team ein | Wenn die [Einladungseinstellungen](03-invitation-settings-on-enterprise-plan.md) Mitgliedern erlauben, neue Personen zu ihren Teams einzuladen, wird die Blockierung der Person aufgehoben und die Person eingeladen. |
| **Gemischte Szenarien** | |
| Die verifizierte Domain wird aus der Domainsteuerung gelöscht | Blockierung für deaktivierte Personen aus der gelöschten Domain wird aufgehoben.  Gelöschte Personen bleiben blockiert und müssen erneut zum Abo eingeladen werden, um die Blockierung aufzuheben. |
| Die Einstellung wird deaktiviert, nachdem sie aktiviert wurde. | Blockierung aller verwalteten, deaktivierten Personen wird aufgehoben.  Gelöschte Personen bleiben blockiert und müssen erneut zum Abo eingeladen werden, um die Blockierung aufzuheben. |

## Häufige Fragen

**Was können andere Abos über blockierte, deaktivierte Personen sehen?**

Die Deaktivierung der Person in deinem Abo ist nur in deinem Enterprise-Abo wirksam. Die Blockierung betrifft nur die Anmeldung mithilfe der Unternehmens-E-Mail-Adresse bei Miro. Die Person sieht in anderen Abos aktiv aus, kann sich aber nicht mit ihrer Unternehmens-E-Mail-Adresse anmelden.

**Wenn jemand deaktiviert und gelöscht wurde, ist der Zugriff dieser Person auf Miro auch dann blockiert, wenn die Einstellung aktiviert ist?**

Personen, die du [aus deinem Abo gelöscht hast](01-deactivated-users.md), bleiben blockiert. Das Löschen der Person hat bestimmte Auswirkungen. Weitere Informationen findest du in unseren Szenarien für blockierte und deaktivierte Personen. Die Blockierung einer gelöschten Person kann nur aufgehoben werden, indem du sie erneut zum Abo mit der verifizierten Domain einlädst. Wenn die Person vor der Aktivierung der Einstellung aus dem Abo gelöscht wurde, hat dies keine Auswirkung auf sie.

**Hat diese Einstellung Auswirkungen auf nicht verwaltete Personen?**

Nein. Diese Einstellung betrifft nur verwaltete Personen.
