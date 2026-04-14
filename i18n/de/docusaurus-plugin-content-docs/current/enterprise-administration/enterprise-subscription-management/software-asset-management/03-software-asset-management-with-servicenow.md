---
title: Software-Asset-Management mit ServiceNow
article_id: 360021758459
translation_id: 360021758459
locale: de
sidebar_position: 3
created_at: '2021-05-20T05:00:32Z'
updated_at: '2025-02-26T11:53:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Analysiere und passe deine Abo-Nutzung mithilfe der ServiceNow- und Miro-Integration passend zu eurer Größe an. Die Integration gibt dir die Möglichkeit, eine Liste der inaktiven Nutzern zu erhalten und sie über die Asset-Management-App zu deaktivieren.

> **Verfügbar für**: [Enterprise-Preisplan](../../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Einrichtung durch:** Unternehmens-Admin

## Unterstützte Funktionen

Mit der Integration hast du Zugriff auf folgende Funktionen:

- **Abos herunterladen**
  - Erhalte eine Liste der Abo-Nutzung und der Anzahl der über dein Miro Enterprise-Abo zugewiesenen Lizenzen.
- **Abos zurückholen**
  - Deaktiviere Nutzer in deinem Miro Enterprise-Preisplan je nach Abo-Nutzung.

## Konfigurationsschritte

### Integration

1. Gehe in ServiceNow zum Modul **SaaS-Lizenz** und wähle **Direct Integration Profiles** (Integrationsprofile zuweisen) und klicke auf **Neu**:

   saas_license_module.jpg
   SaaS-Lizenzmodul

   > ✏️ Falls das **Saas-Lizenzmodul** nicht in deiner ServiceNow-Instanz vorhanden ist, musst du es wie folgt installieren:
2. Suche nach **Miro Enterprise Integrationsprofil**:

   Miro_Enterprise_integration_profile.jpg
   Miro Enterprise Integrationsprofil
3. Du siehst zwei vordefinierte Subflows: **Abos herunterladen** und **Abos zurückfordern:**
   download_subscription_sybflow.jpg
   *Abo Subflow herunterladen*

   reclaim.jpg
   *Abo-Subflow zurückfordern*

### So stellst du eine neue Verbindung her

1. Um eine neue Verbindung zu erstellen, gehe zu **Anmeldeinformationen & Verbindungen** > **Verbindung & Anmeldeinformations-Aliase** und klicke auf **Neu**.
   new_alias.jpg
   *Die Option zum Erstellen eines neuen Alias für Verbindungen und Anmeldeinformationen*

  Klicke auf den Link **Neue Verbindung & Zugangsdaten**:

create_connection.jpg
Verbindungs- und Zugangsdaten-Aliase

Für den Unterschritt **Abos herunterladen** musst du die **Client-ID** und das **Client Secret** (Passphrase) eingeben.

create_connection_modal.jpg
Verbindung und Zugangsdaten herstellen

2. Um die **Client ID** und das **Client Secret**  zu erhalten**,** gehst du auf der Miro-Seite zu **Einstellungen > Profileinstellungen > Deine Apps** und wählst **Neue App erstellen.**

![](../../../../../../../docs/enterprise-administration/enterprise-subscription-management/software-asset-management/images/23921803379090_image.png)*Erstelle eine neue App in den Einstellungen deines Profils*

3. Lege den **Namen der App** fest, wähle ein Team aus und klicke auf **App erstellen.** Beachte, dass du ein [Team von Entwicklern](../../managing-apps-on-enterprise-plan/04-enterprise-developer-teams.md) haben musst.

4. 4. Auf der App-Seite im Abschnitt **Berechtigungen** musst du die Option **organizations:read** prüfen und auf **App installieren und OAuth Token anfordern** klicken.

5. 5. Wähle ein Team aus, das Teil der Enterprise-Organisation ist, und installiere die App.

6. Kopiere die **Client ID** und das **Client Secret**.

Für den Subflow **Abos zurückfordern** musst du ein **SCIM-API-Token** angeben. Um ein SCIM-API-Token zu erhalten, greifst du in Miro auf die Admin-Konsole zu und gehst zu **Apps und Integrationen** > **Unternehmensintegrationen** > **SCIM Provisioning** und kopierst das Token unter **API Token**.

## Anpassung der Abo-Nutzung

Standardmäßig ist die **Schwelle der letzten Aktivität** auf 60 Tage gesetzt.  Navigiere zu den Reklamationsregeln, um sie zu ändern und wähle die Miro-Regel, dann kannst du die Schwelle der letzten Aktivität wie folgt ändern:

last_activity_treshold.jpg
Schwelle der letzten Aktivität

## Mögliche Probleme und wie man sie löst

Wenn du versuchst, die App für ein Team zu installieren, siehst du die Fehlermeldung "Diese App konnte nicht installiert werden. Du kannst diese App nicht installieren. Seine Geltungsbereiche sind in deinem aktuellen Preisplan nicht verfügbar".
- Dies ist das erwartete Verhalten, wenn die App in einem Dev Team installiert wird, da das Dev Team keinen Zugriff auf die Geltungsbereiche auf Organisationsebene hat. Du wirst die App in einem der Enterprise-Teams installieren müssen, wo sie Zugriff auf die Organisationsbereiche der ServiceNow-Integration hat.

install_app_error.jpg
Fehler bei der Installation der App für ein Dev-Team
