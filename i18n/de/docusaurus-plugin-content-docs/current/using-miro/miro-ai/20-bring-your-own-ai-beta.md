---
title: Eigene KI verwenden (BETA)
article_id: 21885197978642
translation_id: 21885197978642
locale: de
sidebar_position: 20
created_at: '2024-10-09T18:45:40Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: ai-generate-image
---

Bring Your Own AI (BYOAI) aktiviert für einige Miro AI-Funktionen deinen eigenen KI-Anbieter anstelle von Miro AI.

> **Erhältlich für:** Enterprise
> **Verfügbar mit:** Desktop

Mit BYOAI kannst du deinen KI-Anbieter mit Miro verbinden und [KI-Funktionen](18-miro-ai-reference.md) nutzen [, die auf GPT basieren](18-miro-ai-reference.md). Miro AI-Funktionen, die von BYOAI nicht unterstützt werden, wie die Bilderzeugung, können optional deaktiviert werden. Weitere Informationen findest du unter Deaktivieren von KI-Funktionen, die nicht von Bring Your Own KI verwendet werden.

Derzeit unterstützt BYOAI OpenAI und Azure OpenAI.

:::note
BYOAI unterstützt nur Miro AI-Funktionen, die von GPT unterstützt werden. Welche Miro AI-Funktionen GPT-fähig sind, erfährst du im [Miro AI-Überblick](18-miro-ai-reference.md).
:::

## Wie man Bring Your Own KI verwendet

> **Erhältlich für:** Unternehmens-Admins

Die folgenden Verfahren erklären, wie du Bring Your Own KI (BYOAI) für Open AI und Azure OpenAI verwendest.

### OpenAI

Befolge diese Schritte:

1. In den Admin-Einstellungen wählst du **Apps und Integrationen** aus.
2. Wähle unter **Enterprise Integration** für **Eigene KI verwenden** **OpenAI** aus.
3. Für den **API-Schlüssel** gibst du deinen OpenAI-Schlüssel ein.
   > ⚠️ Für höchste Sicherheit kopierst du den API-Schlüssel und fügst ihn ein.
4. Wähle **Verbinden**.
5. Stelle sicher, dass du Miro AI für dein Unternehmen aktiviert hast.
   **Weitere Informationen:** Siehe Miro AI aktivieren für Eigene KI verwenden.

   Du hast die BYOAI mit OpenAI erfolgreich eingerichtet.

:::note
Miro verwendet ein Einweg-Speichersystem, um deinen API-Schlüssel sicher zu speichern und zu verschlüsseln, so dass er bei der Eingabe nie sichtbar ist. Weder Miro noch Admins können den API-Schlüssel abrufen, nachdem er aktualisiert und sicher gespeichert wurde.
:::

### Azure OpenAI

Befolge diese Schritte:

1. In den Admin-Einstellungen wählst du **Apps und Integrationen** aus.
2. Wähle unter **Enterprise Integration** für **Eigene KI verwenden** **Azure OpenAI** aus.
3. Gib deinen Azure-API-Schlüssel, den Verteilungsnamen und die Verteilungs-URL ein.
   > ⚠️ Für höchste Sicherheit kopierst du den API-Schlüssel und fügst ihn ein. Vergewissere dich, dass der Einsatz mit GPT-4o erfolgt.
4. Wähle **Verbinden**.
5. Stelle sicher, dass du Miro AI für dein Unternehmen aktiviert hast.
   **Weitere Informationen:** Siehe Miro AI aktivieren für Eigene KI verwenden.

   Du hast die BYOAI mit Azure OpenAI erfolgreich eingerichtet.

:::note
Miro verwendet ein Einweg-Speichersystem, um deinen API-Schlüssel sicher zu speichern und zu verschlüsseln, so dass er bei der Eingabe nie sichtbar ist. Weder Miro noch Admins können den API-Schlüssel abrufen, nachdem er aktualisiert und sicher gespeichert wurde.
:::

### Aktiviere Miro AI für Bring Your Own KI

Nachdem du Open AI oder Azure Open AI verbunden hast, stelle sicher, dass du Miro AI für dein Unternehmen aktiviert hast.

Befolge diese Schritte:

1. In den Admin-Einstellungen wählst du den **Zugriff auf Funktionen** aus.
2. Wähle unter **Funktionsaktivierung** für **Miro AI** eine der folgenden Optionen aus:
   - **Darf von allen verwendet werden**
   - **Darf von bestimmten Teams verwendet werden**
3. (Optional) **Aktiviere die Miro AI Beta-Funktionen**, indem du sie einschaltest.

   Du hast Miro AI erfolgreich für dein Unternehmen aktiviert.

:::note
Standardmäßig sind alle Miro AI-Funktionen verfügbar, wenn du Miro AI aktivierst. Um Miro AI-Funktionen zu deaktivieren, die von deinem KI-Anbieter nicht unterstützt werden, wende dich an den Miro-Support. Weitere Informationen findest du unter Deaktivieren von KI-Funktionen, die nicht von Bring Your Own KI verwendet werden.
:::

## Deaktivieren von KI-Funktionen, die nicht von Bring Your Own KI verwendet werden

Standardmäßig sind alle Miro AI-Funktionen verfügbar, wenn du Miro AI aktivierst. Bring Your Own KI (BYOAI) unterstützt nur LLM-Funktionen, die GPT nutzen. Um sicherzustellen, dass BYOAI nur LLM-Funktionen verwendet, die dein KI-Anbieter unterstützt, kannst du optional nicht-LLM Miro AI-Funktionen deaktivieren.

Wenn du Miro AI-Funktionen deaktivieren möchtest, die nicht zum LLM gehören, wende dich an deinen Miro Customer Success Manager oder an den [Miro-Support](../tools/troubleshooting/06-contacting-miro-support.md).

**Weitere Informationen:** Siehe [Miro AI Übersicht](18-miro-ai-reference.md).

## Häufige Fragen

**Wer ist für die Erstellung der KI-Ausgabe verantwortlich, wenn ich BYOAI verwende?**

Mit BYOAI übernimmst du die Kontrolle über die Erzeugung von Output mit KI, und zwar in der Qualität, die du mit deinem KI-Anbieter festgelegt hast.

**Wie wirkt sich die Nutzung meines eigenen KI-Anbieters auf die Input-Moderation aus?**

Mit BYOAI filtert Miro die Inhalte nicht, bevor dein KI-Anbieter die Ausgabe generiert. Wenn du die Moderation aktivieren möchtest, überprüfe bitte, ob dein Provider die Eingabemoderation aktiviert hat und kontaktiere dann deinen Customer Success Manager oder den [Miro-Support](../tools/troubleshooting/06-contacting-miro-support.md).

**Wie wirkt sich BYOAI auf den KI-Credit-Verbrauch aus?**

Mit BYOAI verbrauchst du Token von deinem eigenen KI-Anbieter, um Miro AI-Funktionen auszuführen. Du verbrauchst auch weiterhin Miro KI-Credits. Weitere Informationen findest du unter [Miro KI-Credit für Enterprise-Preispläne](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/03-miro-ai-credits-for-enterprise-plans.md).

**Was passiert, wenn mein API-Schlüssel abläuft oder ich keine Token mehr habe?**

Als Admin erhältst du eine Fehlermeldung und die Endnutzer können die KI-Funktionen von BYOAI nicht mehr nutzen.

**Wie erhalte ich Support, wenn ich Probleme mit meiner KI-Anbieter-Integration habe?**

Wende dich an deinen Customer Success Manager oder an den Support. Wir empfehlen, dass du dich auch an deinen KI-Anbieter wendest.

**Verwendet Miro irgendeinen Input oder Output, wenn ich BYOAI verwende?**

Nein, die Dateneingabe und -ausgabe unterliegt der Vereinbarung, die du mit deinem Anbieter hast.
