---
title: Zwei-Faktor-Authentifizierung (2FA)
article_id: 27356474050834
translation_id: 27356474050834
locale: de
sidebar_position: 1
created_at: '2025-06-12T12:01:03Z'
updated_at: '2025-06-24T08:19:34Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: 2fa
availability:
  notes: 'Verfügbar für: Team-Admins, Unternehmens-Admins Welche Preispläne: Starter,
    Business, Education, Enterprise Plattformen: Browser, Desktop, Mobile'
---

Die Zwei-Faktor-Authentifizierung (2FA) fügt eine zusätzliche Sicherheitsebene zu Online-Konten hinzu, indem Nutzer zwei eindeutige Verifizierungsmethoden bereitstellen müssen, bevor sie auf ihre Konten zugreifen können.

Miro-Admins können 2FA für ihre Teams aktivieren und 2FA für Teammitglieder zurücksetzen. Nutzer haben die Möglichkeit, ein Gerät für 30 Tage zu vertrauen.

:::note
Dieser Artikel erklärt 2FA für Starter-, Business- und Education-Preispläne. Um mehr über 2FA für Enterprise zu erfahren, siehe [Zwei-Faktor-Authentifizierung (2FA) (Admin-Leitfaden).](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md)
:::

## Zwei-Faktor-Authentifizierung aktivieren

Bei Starter- und Education-Preisplänen stelle sicher, dass du die Team-Admin-Rolle hast.

Für einen Business-Preisplan stelle sicher, dass du die Rolle des Unternehmens-Admins hast.

Befolge diese Schritte:

1. Klicke in deinem Miro-Dashboard rechts oben auf deinen Avatar und wähle **Admin-Konsole** aus.
2. (Starter) Gehe zu **Sicherheit** > **Berechtigungen**.
   Gehe zu **Berechtigungen**.
   Geh zu **Sicherheit** > **Authentifizierung**.
3. Unter **Zwei-Faktor-Authentifizierung (2FA)** den Schalter **Zwei-Faktor-Authentifizierung beim Anmelden erforderlich machen** auf "Ein" stellen.

## Zwei-Faktor-Authentifizierung (2FA) Einrichtung für Nutzer

Für Teams, die 2FA aktiviert haben, müssen sich Nutzer zusätzlich zu ihrer E-Mail und ihrem Passwort über eine Authentifizierungs-App authentifizieren.

Um zu erfahren, wie du als Nutzer 2FA einrichtest, sieh dir den [Leitfaden zur Zwei-Faktor-Authentifizierung (2FA)](02-two-factor-authentication-2fa-–-user-guide.md) an.

## Vertrauenswürdige Geräte

Ein Nutzer, der sich mit 2FA bei Miro anmeldet, kann wählen, ob er seinem Gerät vertrauen möchte.

Wenn ein vertrauenswürdiges Gerät zum Anmelden verwendet wird, wird der Nutzer nur aufgefordert, sich mit seinem ersten Faktor zu authentifizieren, wobei der zweite Faktor übersprungen wird, da das Gerät als vertrauenswürdig gilt.

![](../../../../../../docs/administration/security-compliance/images/27358547112978_image.png)

*Vertrauenswürdiges Gerät für 2FA ist standardmäßig aktiviert.*

Bei der Anmeldung ist **Diesem Gerät für 30 Tage vertrauen** standardmäßig ausgewählt, was der Nutzer optional deaktivieren kann.

:::note
Der Vertrauenszeitraum des Geräts kann nur in einem Enterprise-Preisplan geändert werden. Weitere Informationen findest du im [Admin-Leitfaden zur Zwei-Faktor-Authentifizierung (2FA)](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md).
:::

Um einem versehentlich vertrauten Gerät das Vertrauen zu entziehen, kann sich ein Nutzer überall abmelden. Gehe zu **Profil**, unter **Profileinstellungen**, klicke **Überall abmelden**.

## Zwei-Faktor-Authentifizierung (2FA) zurücksetzen

Wenn ein Nutzer den Zugriff auf seinen zweiten Faktor verliert, kann er bei seinem Admin anfragen, dass seine 2FA zurückgesetzt wird.

Um 2FA für Nutzer auf Starter- und Education-Preisplänen zurückzusetzen, stelle sicher, dass du die Team-Admin-Rolle hast.

Um 2FA für Nutzer im Business-Preisplan zurückzusetzen, stelle sicher, dass du die Rolle des Unternehmens-Admins hast.

Befolge diese Schritte:

1. Klicke auf deinem Miro-Dashboard oben rechts auf deinen Avatar und wähle **Admin-Konsole**.
2. Gehe zu **Nutzer** > **Alle Nutzer**.
3. Finde den Nutzer, und klicke dann auf die drei Punkte (**...**) am Ende der Zeile.
4. Klicke auf **Zwei-Faktor-Authentifizierung zurücksetzen**.
   Der Nutzer erhält die Anweisungen zum Zurücksetzen per E-Mail.
