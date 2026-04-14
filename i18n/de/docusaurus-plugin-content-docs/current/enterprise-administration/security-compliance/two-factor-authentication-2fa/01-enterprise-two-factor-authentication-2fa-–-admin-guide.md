---
title: Enterprise-Zwei-Faktor-Authentifizierung (2FA) – Admin-Leitfaden
article_id: 7935391125394
translation_id: 7935391125394
locale: de
sidebar_position: 1
created_at: '2022-10-04T08:57:18Z'
updated_at: '2026-01-13T13:35:36Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Relevant für: Enterprise-Plan Einrichtung durch: Unternehmens-Admins'
---

## Zwei-Faktor-Authentifizierung (2FA) für Organisationen

Mit der Zwei-Faktor-Authentifizierung erhalten Online-Profile über den Benutzernamen und das Passwort hinaus eine zusätzliche Sicherheitsebene. Unternehmens-Admins im Enterprise-Preisplan können einen zusätzlichen Identitätsnachweis verlangen, wenn Nutzer auf das Miro-Abo ihres Unternehmens zugreifen. Diese Anforderung gilt für alle Anmeldungen mit E-Mail-Adresse und Passwort.

Für Unternehmen, die Single Sign-on (SSO) verwenden, betrifft 2FA nur externe Mitwirkende ohne SSO. Für Unternehmen ohne SSO erstreckt sich 2FA auf alle Nutzer.

:::note
Dieser Artikel erklärt die Zwei-Faktor-Authentifizierung (2FA) für Enterprise-Preispläne. Für alle anderen Preispläne siehe [Zwei-Faktor-Authentifizierung (2FA)](../../../administration/security-compliance/01-two-factor-authentication-2fa.md) in der Administration.
:::

## Einrichten einer erzwungenen 2FA für deine Organisation

:::note
Vor der Aktivierung der Zwei-Faktor-Authentifizierung (2FA) ist es wichtig, alle betroffenen Nutzer zu informieren, sowohl Mitglieder deines Unternehmens als auch externe Mitwirkende. Um einen reibungslosen Übergang zu gewährleisten, empfehlen wir, unseren [2FA-Nutzerleitfaden](../../security-integrations/two-factor-authentication-2fa/02-enterprise-two-factor-authentication-2fa-–-user-guide.md) zu teilen, um ihnen bei diesem Prozess zu helfen.
:::

## 2FA für deine Nutzer aktivieren

1. Gehe zur Admin-Konsole > **Sicherheit** > **Authentifizierung**.
2. Aktiviere **2FA für Nutzer erzwingen, die nicht SSO nutzen**.

![2FA-enable.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24790277317394_2FA-enable.png)*2FA-Authentifizierung für Nutzer erzwingen, die nicht SSO nutzen*

### 2FA-Geräte als vertrauenswürdig einstufen

Wenn aktiviert, wird den 2FA-Nutzern ein Kästchen angezeigt, mit dem sie 2FA jedes Mal überspringen können, wenn sie sich auf diesem Gerät in den nächsten X Tagen anmelden, wobei "X" der vom Admin festgelegte Zeitraum ist. Du kannst es Nutzern erlauben, ihre Geräte für 7 bis 90 Tage als vertrauenswürdig einzustufen. Standardmäßig ist das Vertrauen von 2FA-Geräten aktiviert, aber du kannst diese Funktion in deiner Admin-Konsole deaktivieren.

![2FA-trusted-devices.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24790277323410_2FA-trusted-devices.png)

:::warning
Wenn das Vertrauen von 2FA-Geräten deaktiviert ist, müssen Nutzer bei jeder Anmeldung einen 2FA-Code eingeben. Dies verlangsamt ihre Anmeldung.
:::

2FA wird nach Ablauf des vertrauenswürdigen Zeitraums erneut erforderlich sein.

2FA wird nicht übersprungen, wenn Nutzer sich auf einem neuen Gerät oder Browser anmelden oder ihre Browser-Cookies löschen.

## Zurücksetzen von 2FA für Nutzer

Wenn ein Nutzer den Zugriff auf seine 2FA-Methode verliert, können Admins seine 2FA zurücksetzen. Sobald ein Nutzer um das Zurücksetzen seiner 2FA-Methode bittet, erhält der zuständige Admin eine E-Mail-Benachrichtigung.

:::note
Admins können die Zwei-Faktor-Authentifizierung nur für Nutzer zurücksetzen, deren E-Mail-Domains in ihrer Organisation verifiziert sind, wenn der Admin das Zurücksetzen initiiert. Wenn der Nutzer ein Zurücksetzen beantragt, kann jeder Admin in der Organisation dies genehmigen.
:::

So setzen Sie die 2FA-Methode für den Nutzer zurück:

1. Gehe zur **Admin-Konsole** > **Nutzer** > **Tab „Aktive Nutzer“**.
2. Finde den Nutzer, dessen 2FA-Methode zurückgesetzt werden muss.
3. Klicke auf das **Drei-Punkte-Symbol** (**...**) in der Zeile des Nutzers.
   ![reset-2fa.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24650686629138_reset-2fa.png)
   *Zurücksetzen der Zwei-Faktor-Authentifizierung in der Admin-Konsole*
4. Klicke auf **Zwei-Faktor-Authentifizierung zurücksetzen**.
   Ein Dialogfeld wird geöffnet, das um Bestätigung bittet.
5. Klicke auf die Schaltfläche **2FA zurücksetzen** im Dialogfeld.
6. Eine Bestätigungsnachricht wird oben auf Ihrem Bildschirm angezeigt, die bestätigt, dass Anweisungen zum Zurücksetzen an den Nutzer gesendet wurden.

## Auswirkungen auf die Nutzererfahrung

- Nutzer, die SSO nicht verwenden, werden beim nächsten Login aufgefordert, ihren zweiten Faktor einzurichten. Bei diesem Vorgang werden sie nicht von laufenden Sitzungen abgemeldet.
- Die Nutzer müssen 2FA mit ihrem mobilen Gerät und einer beliebigen zeitbasierten Einmal-Passwort-Anwendung (TOTP) wie Microsoft Authenticator, Google Authenticator oder Authy konfigurieren.
- Nutzer, die 2FA verwenden, haben 3 Versuche, einen gültigen TOTP-Code einzugeben. Wenn dieses Limit überschritten wird, müssen sie den Authentifizierungsprozess erneut starten.
- Obwohl die 2FA-Anmeldung in mobilen und Tablet-Apps verfügbar ist, wird der erste Registrierungsprozess ausschließlich in Browser- und Desktop-Anwendungen unterstützt.

## Wichtig zu wissen

Die Durchsetzung der 2FA gilt nur für *Nutzer, die sich mit ihrer E-Mail und ihrem Passwort oder über magische Links (per E-Mail gesendet) authentifizieren*.

- 2FA ist nicht für externe Mitwirkende aktiviert, die sich über Single Sign-on (SSO) authentifizieren.
- Externe Mitwirkende deiner Enterprise-Organisation, die sich bereits von ihrer eigenen Organisation aus über SSO authentifiziert haben, können weiterhin über SSO auf alle Teams und Boards in Miro zugreifen.
- Wenn sich ein Nutzer über eine Anmeldeintegration eines Drittanbieters (z. B. Google, Microsoft, Slack) authentifiziert, behält er über diese Anmeldeintegration Zugriff auf alle Miro-Teams und Boards. Admins haben die Möglichkeit, solche Nutzer dazu aufzufordern, innerhalb ihrer jeweiligen Anmeldeintegration einen zweiten Faktor einzurichten. Der Authentifizierungsfluss von Miro fordert diese Nutzer jedoch nicht auf, einen zweiten Faktor einzurichten.

## Audit-Protokolle

Admins können Nutzer, die 2FA eingerichtet haben, sowie erfolgreiche und fehlgeschlagene 2FA-Anmeldungen anhand der folgenden Audit-Protokollereignisse verfolgen:

- `mfa_setup_succeeded` – wenn eine Person ihren zweiten Faktor erfolgreich eingerichtet hat
- Aktualisierung des Ereignisses `sign_in_succeeded`, um das Attribut „MfaFactorType“ einzubeziehen, wenn eine erfolgreiche Anmeldung mit 2FA abgeschlossen wurde
- Aktualisierung des Ereignisses `sign_in_failed`, um das Attribut „MfaFactorType“ einzubeziehen, wenn eine Anmeldung mit 2FA nicht erfolgreich war, weil der Nutzer die maximale Anzahl von Versuchen überschritten hat (nicht-technischer Fehler)
