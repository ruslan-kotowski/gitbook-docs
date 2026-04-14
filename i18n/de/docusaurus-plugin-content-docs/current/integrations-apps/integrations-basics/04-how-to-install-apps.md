---
title: So installierst du Apps
article_id: 360017731093
translation_id: 360017731093
locale: de
sidebar_position: 4
created_at: '2019-02-11T10:12:46Z'
updated_at: '2025-08-05T07:54:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
availability:
  notes: 'Personen: Alle Nutzer Preispläne: Alle Preispläne Plattformen: Browser,
    Desktop-App Team-Admins können die Installation für Nicht-Admins einschränken.
    Unternehmens-Admins im Enterprise-Preisplan können die Nutzung weiter einschränken,
    sodass nur genehmigte Apps verwendet werden.'
---

Du kannst die Funktionalität von Miro erweitern, indem du Apps aus dem Miro Marketplace installierst. Dieser Artikel führt dich durch die Installation und Deinstallation von Apps, das Verstehen von App-Berechtigungen und gibt einen Überblick über die Erstellung von benutzerdefinierten Integrationen.

## Apps vom Miro Marketplace installieren

Der [Miro Marketplace](https://miro.com/marketplace/) ist dein zentraler Anlaufpunkt, um Apps zu entdecken und hinzuzufügen und so deine Miro-Erfahrung zu verbessern. Du kannst Apps direkt von deinem Board aus oder auf der Marketplace-Website installieren.

![Miro_marketplace.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021611044242_Miro%20marketplace.jpg)*Miro Marketplace*

Es gibt zwei Hauptmöglichkeiten für Nutzer, um Apps hinzuzufügen:

1. **Von deinem Board aus:** Klicke auf das Symbol **Tools, Medien und Integrationen (+)** in der Erstellungssymbolleiste und verwende das Suchfeld „Integrationen suchen“ im Marketplace-Tab. Wenn du deine App bereits aufgeführt siehst, klicke einfach darauf, um sie hinzuzufügen. Du kannst auch durch die verfügbaren Apps in diesem Feld stöbern.
   ![marketplace-add-apps.png](../../../../../../docs/integrations-apps/integrations-basics/images/21260776452626_marketplace-add-apps.png)*Marketplace in der Erstellungssymbolleiste*
2. **Von der Marketplace-Website aus:** Du kannst auch direkt zur [Miro Marketplace](https://miro.com/marketplace/)-Website gehen, um Apps aus ihren jeweiligen Auflistungen zu durchsuchen und zu installieren.

**Für Unternehmens-Admins:**
Unternehmens-Admins in den entsprechenden Preisplänen können über die Teameinstellungen auch Apps für ihr gesamtes Team installieren. Um dies zu tun, navigiere zu **Teameinstellungen** > **Apps & Integrationen** > **Apps installieren**. Dieser Abschnitt ermöglicht die zentrale Verwaltung und Bereitstellung von Apps im gesamten Team.

![apps_and_integrations_page.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021832338450_apps%20and%20integrations%20page.jpg)*Abschnitt für installierte Apps in den Teameinstellungen für Admins*

## Apps deinstallieren

Du kannst Apps über deine Teameinstellungen verwalten und deinstallieren. Beachte, dass Nicht-Admin-Nutzer je nach Teamkonfiguration Einschränkungen beim Deinstallieren von Apps haben können.

:::warning
Nicht-Admin-Nutzer können Apps nicht deinstallieren, wenn sie sie in den Teameinstellungen nicht von einem Admin installieren dürfen.
:::

Um deine Team-Apps zu verwalten, gehe zu **Teameinstellungen > Apps & Integrationen**. Diese Seite listet alle Apps auf, die derzeit für dein Team oder von dir persönlich installiert sind.

![apps_settings.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021898097682_apps%20settings.jpg)*Apps & Integrationen in den Teameinstellungen*

Gehe wie folgt vor, um eine App zu deinstallieren:

1. Wähle aus der Liste **Apps & Integrationen** die App aus, die du entfernen möchtest.
2. Klicke entweder auf **Für das Team deinstallieren** oder **Für mich deinstallieren**. Die verfügbare Option hängt davon ab, wie die App installiert wurde und welche Administratorrechte du hast.

![uninstall_an_app.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021797466258_uninstall%20an%20app.jpg)*Die Option zum Deinstallieren einer App*

## App-Installationsberechtigungen

Team- und Unternehmens-Admins haben verschiedene Kontrollmöglichkeiten, um zu verwalten, wer Apps installieren kann und welche Apps ihrer Organisation zur Verfügung stehen, um Sicherheit und Compliance zu gewährleisten.

Team-Admins können konfigurieren, ob Teammitglieder ohne Admin-Rechte Apps installieren dürfen. Diese Einstellung findest du unter **Teameinstellungen > Apps & Integrationen** unter den Optionen zur App-Verwaltung.

![allow_non-admins_to_install_apps.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021903025170_allow%20non-admins%20to%20install%20apps.jpg)*Option "Nicht-Admins das Installieren von Apps erlauben" in den Teameinstellungen*

Für Nutzer im [Enterprise-Preisplan](../../plans-billing/miro-plans/04-enterprise-plan.md) haben Unternehmens-Admins Zugang zu detaillierteren Kontrollmöglichkeiten. Sie können **Genehmigte Apps** über **Unternehmenseinstellungen** > **Apps** verwalten. Dieses Feature ermöglicht es Admins, eine Liste von Unternehmens-überprüften Apps zu pflegen und zu verhindern, dass Nutzer Apps installieren, die nicht auf dieser genehmigten Liste stehen. [Erfahre mehr über die Verwaltung von App-Discovery- und Installationseinstellungen für Enterprise-Preispläne](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).

![Enterprise_apps.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021890162962_Enterprise%20apps.jpg)*Verwalten genehmigter Apps in den Unternehmenseinstellungen des Enterprise-Preisplans*

## Benutzerdefinierte Integrationen und Entwicklerplattform

Solltest du spezielle Funktionen benötigen, die im Miro Marketplace nicht verfügbar sind, kannst du mit der [Miro Developer Platform](https://miro.com/api/) eigene maßgeschneiderte Lösungen erstellen. Diese Plattform bietet robuste Tools, darunter REST APIs, Web-Plugins und Einbettungen, um dir zu helfen, leistungsstarke Integrationen zu erstellen, die auf deine Bedürfnisse zugeschnitten sind.

Hier sind einige wichtige Punkte, die du bei der Entwicklung benutzerdefinierter Integrationen beachten solltest:

- **Erste Schritte:** Du kannst deine App entwickeln, indem du ein [Entwicklerteam erstellst](https://developers.miro.com/). Standard-Entwicklerteams sind für Entwicklungs- und Testzwecke gedacht und unterliegen bestimmten Einschränkungen:
  - Bis zu 5 Nutzer im Team.
  - Bis zu 3 Boards im Team.
  - Ein Wasserzeichen wird auf den Boards angezeigt.
  - Die Exportfunktion für Boards ist nicht verfügbar.
- **Enterprise-Preisplan-Entwickler:** Wenn sich deine Organisation im [Enterprise-Preisplan](../../plans-billing/miro-plans/04-enterprise-plan.md) befindet, kannst du im Rahmen deines Abos ein Entwicklerteam erstellen. Diese Entwicklerteams unterliegen nicht den Einschränkungen der Standardteams und profitieren von allen Sicherheitsfunktionen auf Enterprise-Niveau. [Erfahre mehr über Entwicklerteams für Enterprise-Preispläne](../../enterprise-administration/managing-apps-on-enterprise-plan/04-enterprise-developer-teams.md).

Weitere Informationen, Support und um dich mit anderen Entwicklern zu vernetzen, kannst du das [Developer Platform Forum](https://community.miro.com/developer-platform-forum-57) erkunden.
