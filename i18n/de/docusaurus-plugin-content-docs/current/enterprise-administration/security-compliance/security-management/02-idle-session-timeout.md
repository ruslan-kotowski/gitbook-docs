---
title: Zeitlimit bei Inaktivität
article_id: 360017571454
translation_id: 360017571454
locale: de
sidebar_position: 2
created_at: '2019-02-11T10:09:05Z'
updated_at: '2025-02-06T08:46:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '**Erhältlich für: Enterprise-Preisplan Erforderliche Rolle: Unternehmens-Admin'
---

Mit der Funktion Sitzungszeitüberschreitung kannst du festlegen, **wie** lange deine Nutzer inaktiv sein dürfen. Die Einstellung betrifft alle Mitglieder und [Gäste](../../../using-miro/sharing-boards/07-collaboration-with-guests.md). Wenn die Sitzung des Nutzers das Limit erreicht und abläuft, wird er automatisch von seinem Miro-Profil abgemeldet und muss sich erneut autorisieren, bevor er auf die Unternehmensdaten zugreifen kann.

:::warning
Sei achtsam, wenn du Zeitlimits festlegst. Hochgesicherte Timeout-Limits, die zu kurz sind, führen dazu, dass Nutzer ständig von ihren Boards abgemeldet werden. Achte beim Festlegen von Zeitlimits auf ein gutes Gleichgewicht zwischen Sicherheit und Komfort und vergiss nicht, die Zeitlimits den Nutzern klar zu kommunizieren.
:::

### So aktivierst du das Zeitlimit bei Inaktivität

1. Gehe zu **Unternehmenseinstellungen** > **Sicherheit** > **Authentifizierung** > **Idle Session Timeout**
2. Schalte die Option **Inaktive Nutzer automatisch abmelden** ein und lege das **Timeout-Limit** fest

   ![](../../../../../../../docs/enterprise-administration/security-compliance/security-management/images/23921804858002_idle-session-timeout.png)
*altidle-session-timeout.png Zeitlimit bei Inaktivität ist aktiviert*

Wenn du die Funktion für das Timeout der Leerlaufsitzung zum ersten Mal aktivierst, wird die Standard-Sitzung für 1 Tag aktiviert. Der Admin kann die Dauer anpassen, indem er einen benutzerdefinierten Ganzzahlwert von 1 bis 9999 eingibt und die Einheit festlegt: Minuten, Stunden oder Tage. Die zulässige Mindestdauer beträgt 1 Stunde und die zulässige Höchstdauer beträgt 14 Tage. Wir empfehlen, eine Dauer von mindestens 8 Stunden einzustellen.

Für die Funktion "Idle Session Timeout" definieren wir Inaktivität als keine der folgenden Aktionen in der App während der festgelegten Zeit:

- Mausbewegung (oder Touchscreen-Bewegung)
- Mausklicks (oder Touchscreen-Berührungen)
- Tastatureingaben

Einige Minuten vor der Abmeldung wird den Nutzern eine Warnmeldung angezeigt. Die Nutzer können einfach die Maus bewegen oder eine beliebige Taste auf ihrer Tastatur drücken, um eingeloggt zu bleiben.

:::note
Der Standardwert für die Zeitüberschreitung der Leerlaufsitzung ist 1 Tag. Die Einstellungen können von 1 Stunde bis 14 Tage reichen.
:::

:::note
Idle Session Timeout funktioniert überall (Zugriff auf Nutzeraktivitäten auf verschiedenen Geräten, Integrationen usw.).
:::

:::note
Wenn ein Nutzer ein Besucher auf einem öffentlichen Board ist, das in einem Enterprise-Preisplan gespeichert ist, aber nicht zu dem Enterprise-Preisplan gehört, der die Sitzungszeitüberschreitung aktiviert hat, ist er davon nicht betroffen.
:::

:::note
Wenn ein Nutzer mehreren Organisationen angehört, die unterschiedliche Intervalle für das Timeout der Leerlaufsitzung festgelegt haben, gilt die kürzeste Dauer. Wenn ein Nutzer z. B. einer Organisation angehört, für die eine 6-stündige Leerlaufzeit gilt, und einer Organisation, für die eine 30-minütige Leerlaufzeit gilt, wird er nach 30 Minuten aus allen aktiven Sitzungen ausgeschlossen.
:::
