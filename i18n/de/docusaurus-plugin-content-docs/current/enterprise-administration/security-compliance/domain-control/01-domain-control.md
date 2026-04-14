---
title: Domainsteuerung
article_id: 360034831793
translation_id: 7316173359506
locale: de
sidebar_position: 1
created_at: '2022-08-25T09:50:43Z'
updated_at: '2026-03-27T15:52:06Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
availability:
  plans: business, enterprise
  roles: company_admin, system_admin
---

> **Verfügbar für:** Business, Enterprise
> **Erforderliche Rolle:** Unternehmens-Admin, System-Admin

Über die Domainsteuerung können Unternehmens-Admins den Zugriff der Nutzer innerhalb ihres Abos verwalten. Mit der Domainsteuerung können Admins die Einhaltung der Sicherheitsvorschriften des Unternehmens erzwingen und die verwalteten Nutzeraktivitäten innerhalb ihrer Domains im Auge behalten.

Hier erfährst du, wie du die Domainsteuerung für dein Unternehmen einrichten kannst.

**Mit der Domainsteuerung können Admins des Enterprise-Preisplans:**

- Audits durchführen, um Nutzer zu identifizieren, die mit einer verwalteten Domain assoziiert werden, die nicht in deinem Abo enthalten ist, und sie einladen, beizutreten.
- verhindern, dass Nutzer innerhalb einer Domain unautorisierte Abos erstellen.
- neu registrierte Nutzer automatisch zu bestimmten Teams hinzufügen.
- [Deaktivierte Nutzer blockieren](../../user-management/02-block-deactivated-users.md), um deren Zugriff auf Miro mit ihrer E-Mail-Adresse zu verhindern.

**Admins im Business-Preisplan:**

- können die automatisierte Domainverifizierung zur Verwaltung von Domains verwenden. Nur neu hinzugefügte Domains werden automatisch überprüft.
- können die Richtlinien für die Domainsteuerung nicht ändern.
- können kein Domain-Audit anfordern.

![domain-policies-business.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21046889202834_domain-policies-business.png)

*Die Domain-Richtlinien können unter „Verwaltete Domains für Nutzer des Business-Preisplans“ angezeigt werden*

Nutzer des Business-Preisplans müssen für andere erweiterte Funktionen ein Upgrade machen.

:::note
Die Massenverwaltung von Domains wird derzeit nicht unterstützt.
:::

## Primärdomäne

Deine primäre Domain bestimmt, wie Miro interne und externe Nutzer in deiner Organisation identifiziert. Um zu erfahren, wie du deine primäre Domain ansehen, ändern oder verwalten kannst, sieh dir [Verwalten deiner primären Domain](https://help.miro.com/hc/en-us/articles/34249718672274) an.

## Domainsteuerung einrichten

### Schritt 1: Domains hinzufügen

1. Öffne dein Miro-Dashboard.
2. Klicke auf dein Profilbild in der rechten oberen Ecke.
3. Wähle **Einstellungen** aus dem Dropdown-Menü aus.
4. Wechsle im linken Menü zu **Sicherheit & Compliance** und klicke auf **Verwaltete Domains**

   > ✏️ In Business-Preisplänen findest du **Verwaltete Domains** im **Konto**.
5. Klicke auf **+ Eine Domain hinzufügen** und gib den vollständigen Domainnamen ein (z. B. deinefirma.com).
   ![Managed-domains-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318776338_Managed-domains-settings.png)
*Verwaltete Domain-Einstellungen*

:::note
Wenn du [**Deaktivierte Nutzer blockieren**](../../user-management/02-block-deactivated-users.md) aktiviert hast, werden alle deaktivierten Nutzer, die mit einer neu bestätigten Domain verknüpft sind, automatisch blockiert.
:::

### Schritt 2: Domains bestätigen

1. Nachdem du eine Domain hinzugefügt hast, erhältst du einen Bestätigungscode in deinen **Managed domain**-Einstellungen. Kopiere diesen Code.

   ![Complete-domain-verification.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318779282_Complete-domain-verification.png)
*Den Bestätigungscode kopieren*
2. Wenn du deine DNS-Einträge verwaltest, aktualisiere deine DNS-Einstellungen, indem du einen TXT-Eintrag mit dem Bestätigungscode als dessen **Wert** hinzufügst. (Wenn jemand anders deine DNS-Einträge verwaltet, sende der Person den Bestätigungscode mit Anweisungen zur Aktualisierung der DNS-Einträge.)
3. Melde dich auf der Website deines Domain-Anbieters an (GoDaddy, Amazon, Cloudflare usw.) und gehe zum Abschnitt **DNS**-**Einträge**.
4. Erstelle einen neuen **TXT-Eintrag** mit den folgenden Spezifikationen:
   **Wert/Antwort/Beschreibung:** *„miro-verification=[EINFÜGEN VERIFIKATIONSCODE]“*
   **Name/Host/Alias:** Lassen Sie dieses Feld leer oder geben Sie @ ein, um ein Subdomain einzufügen.
   **Time to live (TTL):** „86400“ (dies kann auch von der Standardkonfiguration übernommen werden).

   ![Creating-new-TXT-record.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318775314_Creating-new-TXT-record.png)
   *Einen neuen TXT-Eintrag erstellen*

:::note
Du kannst den TXT-Eintrag über die Administrationskonsole oder das Dashboard des Hosting-Providers der Domain aktualisieren. [Liste der DNS-Provider ansehen](https://support.google.com/a/topic/1409901).
:::

### Schritt 3: Domain-Verifizierung prüfen

1. Nachdem du den DNS-Eintrag aktualisiert hast, überprüfe den Status deiner Domain-Verifizierung sofort in deinen **verwalteten Domains** Einstellungen, indem du auf **Verifizierung überprüfen** klickst.
2. Wenn die Domain nicht sofort verifiziert wird, prüft Miro in den nächsten 30 Tagen alle 2 Stunden automatisch den Verifizierungscode.

### Schritt 4: Benachrichtigung über den Verifizierungsstatus

1. Sobald deine Domain erfolgreich verifiziert wurde, erhältst du eine E-Mail, die den Verifizierungsstatus bestätigt.
2. Bitte entferne den DNS-Eintrag nach der Verifizierung nicht, da er für zukünftige Verifizierungen erforderlich sein kann.
   ![Check-domain-verification.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017348597650_Check-domain-verification.png)
*Verifizierung der Domain überprüfen*

## Regeln bei der Verifizierung von Domains

- Du musst einen separaten TXT-Eintrag für jede Top-Level-Domain und jede Subdomain, die du verwendest, erstellen. Befolge die obigen Schritte 1–4 für jede Domain oder Subdomain, die du verifizieren möchtest.
- Deine Domain muss genau übereinstimmen.

  > ✏️ Subdomains sind nicht erlaubt.
- Vergewissere dich, dass alle Zonen, die in der verifizierten Domain-Konfiguration verwendet werden, enthalten sind.
- Der Fully Qualified Domain Name (FQDN) sollte mit deiner Domain-Adresse übereinstimmen. Zum Beispiel, [www.mycompanydomain.com](http://www.mycompanydomain.com).
- Wenn du sowohl internes als auch externes DNS verwendest, empfehlen wir, beide zu bestätigen, um eine umfassende Domainsteuerung sicherzustellen.

## Nutzer und Zugriff verwalten

### Domain-Einstellungen bearbeiten

Die Domain-Einstellungen bestimmen, wie bestehende und neu registrierte Nutzer innerhalb deiner Domain(s) verwaltet werden.

1. Sobald eine Domain verifiziert wurde, klicke auf die drei Punkte (**...**) und wähle **Domain-Einstellungen bearbeiten**.
   ![Edit-domain-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318773138_Edit-domain-settings.png)
*Domain-Einstellungen bearbeiten*
2. Hier siehst du Optionen für den Umgang mit neuen Nutzern in deiner Domain:

- **Neue Nutzer automatisch erfassen**: Nutzer, die sich mit einer E-Mail-Adresse einer verwalteten Domain bei Miro registrieren, werden automatisch zum Abo dieser Domain mit dem Standard-Lizenztyp hinzugefügt. Du kannst auch definieren, zu welchen Teams die Nutzer hinzugefügt werden (erforderlich).
- **Die Erstellung eigener Abos unterbinden**: Verbiete verwalteten Nutzern innerhalb deiner Domain(s), neue Teams außerhalb deines Abos zu erstellen. Diese Nutzer können jedoch weiterhin zu Teams in deinen Domains eingeladen werden und extern zusammenarbeiten.

  ![Managed-domain-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318773778_Managed-domain-settings.png)
*Optionen zur Verwaltung neuer Nutzer deiner Domain*

  > ✏️ Wenn du die Option **Die Erstellung eigener Abos unterbinden** aktiviert hast, können Nutzer sich nicht selbst registrieren, es sei denn, sie wurden eingeladen, oder Auto-Capture oder JIT ist aktiviert.

### Interne und externe Nutzer

Wenn eine Domain beansprucht wird, enthalten die Nutzerdetails eine **Interne** oder **Externe** Klassifizierung.

![](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/33613933595794_image.png) *Nutzerdetails zeigen, ob der Nutzer extern oder intern zu deiner verifizierten Domain ist*

Interne Nutzer haben eine E-Mail-Adresse von einer Domain, die von deinem Enterprise-Konto beansprucht wird. Zum Beispiel `user@acme.com`, wobei `acme.com` eine deiner verifizierten Domains ist.

Externe Nutzer haben eine E-Mail-Adresse außerhalb jeder Domain, die von deinem Enterprise-Konto beansprucht wird. Zum Beispiel `user@not-domain.com`, wobei `not-domain.com` nicht eine deiner verifizierten Domains ist.

:::note
Nutzerdetails sind im Nutzerprofil sichtbar. In der Admin-Konsole sind Nutzerdetails auch in der Nutzerliste einsehbar, wo du optional nach **interner** oder **externer** Klassifizierung filtern kannst.
:::

Die interne oder externe Klassifizierung erfolgt automatisch, basierend darauf, ob die Domain des Nutzers von deinem Enterprise-Konto beansprucht und verifiziert wurde.

## Zusammenführung von Self-Service-Teams zum Enterprise-Preisplan

Als Unternehmens-Admin kannst du alle Teams, die von deinen Domains erstellt wurden, in deinen Enterprise-Preisplan migrieren. Dies gewährleistet höhere Sicherheit, bessere Zusammenarbeit und unkompliziertere Verwaltung, da alle Teams an einem Ort zusammengeführt werden. Darüber hinaus kannst du auch Domains prüfen, um Nutzer und Teams zu identifizieren und zusammenzuführen, die Teil deiner verwalteten Domain sind, aber derzeit außerhalb deines Abos sind.

Für weitere Informationen siehe die [Dokumentation zur Zusammenführung von Teams](../../managing-enterprise-teams-and-content/06-self-serve-teams-to-enterprise-plan-consolidation.md).

## Anfragen zur Änderung der E-Mail-Adresse

Wenn dein Unternehmen eine Domain beansprucht hat, können mit dieser Domain verbundene Nutzer ihre E-Mail-Adresse in Miro nicht ohne die Genehmigung des Unternehmens-Admins ändern. Wenn Nutzer versuchen, ihre E-Mail-Adresse zu ändern, erhalten sie die folgende Fehlermeldung: **Sie können Ihre E-Mail-Adresse nicht zu oder von einer Domain einer Organisation ändern.** Es wird empfohlen, dass sich die Nutzer an ihren Unternehmens-Admin wenden, der daraufhin den Miro-Support um Unterstützung bitten kann.

## Häufige Fragen

Kann ich die Domainsteuerung mit einer Subdomain verwenden?

Ja, Subdomains werden als separate Entitäten von den primären Domains behandelt. Befolge den Einrichtungsprozess für jede Subdomain, die du bestätigen möchtest.

Wie verwende ich SSO mit der Domainsteuerung?

Du musst die Domainsteuerung einrichten, bevor du die [SSO](../../security-integrations/single-sign-on-sso/09-single-sign-on-(sso).md)-Authentifizierung aktivierst.

Was ist, wenn sich der Name meiner Domain ändert oder ich eine Subdomain hinzufügen möchte?

Wenn sich der Name deiner Domain ändert, entferne die Domain und starte den Verifizierungsprozess mit der neuen Domain oder allen Subdomains, die du hinzufügst, neu.

Wo finde ich die DNS-Einträge für meine Domain?

Um die DNS-Einträge für deine Domain zu finden, musst du auf die Plattform des Registrars zugreifen, auf der deine Domain registriert ist. Wenn du dir nicht sicher bist, wer dein Domain-Registrar ist, kannst du diese Informationen finden, indem du mit **who.is** nach der Domain suchst. Sobald du deinen Registrar identifiziert hast, melde dich auf seiner Website an und gehe zu dem Bereich, der normalerweise mit **Domains** oder **DNS-Management** bezeichnet wird. Hier findest du die DNS-Einstellungen oder -Einträge für deine Domain.

Warum kann ich **Verwaltete Domains** in meinen **Sicherheits- und Compliance**-Einstellungen nicht sehen?

Wenn du die Option für **Verwaltete Domains** nicht siehst, kann das zwei Gründe haben:

- Du hast keinen Enterprise-Preisplan abonniert, der diese Funktion enthält.
- Du bist nicht Unternehmens-Admin – diese Rolle ist für den Zugriff auf diese Einstellung erforderlich.

Bitte überprüfe die Details deines Preisplans und schau, ob du Unternehmens-Admin bist, um weitere Unterstützung zu erhalten.

Kann ich den TXT-Eintrag für meine Domain löschen, sobald er überprüft wurde?

Wenn du den TXT-Eintrag nach der Verifizierung löschst, hat das zwar keinen unmittelbaren Einfluss auf den Betrieb deiner Domainsteuerung, aber wir empfehlen dir, diesen Eintrag aufzubewahren. Den TXT-Eintrag aufzubewahren, ist für potenzielle erneute Verifizierungsprozesse in der Zukunft wichtig. Wenn du den TXT-Eintrag entfernst, kann das diese Prozesse erschweren und du musst die Verifizierungsschritte erneut durchlaufen.
