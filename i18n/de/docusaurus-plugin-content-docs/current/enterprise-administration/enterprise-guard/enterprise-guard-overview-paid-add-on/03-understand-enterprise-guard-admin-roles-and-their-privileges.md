---
title: Enterprise Guard Admin-Rollen und deren Berechtigungen verstehen
article_id: 15695755655954
translation_id: 15695755655954
locale: de
sidebar_position: 1
created_at: '2023-12-11T18:33:53Z'
updated_at: '2026-03-12T22:21:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Die Funktionen von Enterprise Guard werden durch Admin-Berechtigungen gesteuert. Diese Berechtigungen können über vordefinierte Admin-Rollen oder über benutzerdefinierte Admin-Rollen mit den erforderlichen Berechtigungen gewährt werden.

Die folgende Tabelle listet die verfügbaren Berechtigungen für jede Funktion auf und zeigt, welche vordefinierten Admin-Rollen sie standardmäßig enthalten. Bei der Erstellung benutzerdefinierter Admin-Rollen können Unternehmens-Admins diese Berechtigungen zuweisen, um Zugriff auf bestimmte Enterprise Guard-Funktionen zu gewähren.

Die folgende Tabelle führt die detaillierten Berechtigungen und das Admin-Rollen-Matrix für jede Funktion  auf.

|  |  |  |  |
| --- | --- | --- | --- |
| **Content Lifecycle Management** | | | |
| **Berechtigung** | **Datenverwaltungs-Admin** | **Admin für sensible Inhalte** | **eDiscovery-Admin** |
| Papierkorbeinstellungen ansehen | ✅ | ❌ | ❌ |
| Papierkorbeinstellungen bearbeiten | ✅ | ❌ | ❌ |
| Aufbewahrungsrichtlinie hinzufügen | ✅ | ❌ | ❌ |
| Aufbewahrungsrichtlinie bearbeiten | ✅ | ❌ | ❌ |
| Löschungsrichtlinie löschen | ✅ | ❌ | ❌ |
| Löschungsrichtlinie hinzufügen | ✅ | ❌ | ❌ |
| Löschungsrichtlinie bearbeiten | ✅ | ❌ | ❌ |
| Löschungsrichtlinie löschen | ✅ | ❌ | ❌ |
| **Datenklassifizierung** | | | |
| **Berechtigung** | **Data Governance Admin** | **Content-Admin für sensible Inhalte** | **eDiscovery Admin** |
| Einstellungen zur Datenklassifizierung ansehen | ❌ | ✅ | ❌ |
| Klassifizierungsstufen bearbeiten | ❌ | ✅ | ❌ |
| Einstellungen für die automatische Klassifizierung bearbeiten | ❌ | ✅ | ❌ |
| Einstellungen für Klassifizierungsvorgaben bearbeiten | ❌ | ✅ | ❌ |
| Standardklassifizierungsstufe bearbeiten | ❌ | ✅ | ❌ |
| **Datenerkennung** | | | |
| **Berechtigung** | **Data Governance Admin** | **Content-Admin für sensible Inhalte** | **eDiscovery Admin** |
| Datenschutzlabel ansehen | ❌ | ✅ | ❌ |
| Erkennung datenschutzrelevanter Daten aktivieren/deaktivieren | ❌ | ✅ | ❌ |
| Anzahl der Übereinstimmungen aufrufen – Datenschutzlabels | ❌ | ✅ | ❌ |
| Zensierte Übereinstimmungen aufrufen – Datenschutzlabels | ❌ | ✅ | ❌ |
| Vollständige Übereinstimmungen aufrufen – Datenschutzlabels | ❌ | ✅ | ❌ |
| **eDiscovery** | | | |
| **Berechtigung** | **Data Governance Admin** | **Content-Admin für sensible Inhalte** | **eDiscovery Admin** |
| Verwaltung von Aufbewahrungsfrist-Einstellungen | ❌ | ❌ | ✅ |
| Einstellungen für Aufbewahrungsfristen anzeigen | ❌ | ❌ | ✅ |

*Detaillierte Berechtigungen und vordefinierte Admin-Rollenmatrix für jede Funktion*

> **HINWEIS:** Enterprise Guard-Funktionen können über vordefinierte Admin-Rollen oder über benutzerdefinierte Admin-Rollen mit den erforderlichen Berechtigungen zugewiesen werden.

## Eine Enterprise Guard-Admin-Rolle zuweisen

:::note
Um einem Nutzer eine Enterprise Guard-Admin-Rolle zuzuweisen, musst du ein **Unternehmens-Admin** sein.
:::

1. Gehe zu deinen **Profileinstellungen**:

   - Von einem Board aus: **Hauptmenü > Einstellungen > Profileinstellungen**.
   - Vom Dashboard aus: Klicke dein **Avatar** in der oberen rechten Ecke an und dann **Einstellungen**.
   - Von der URL: Gehe zu `https://miro.com/app/settings` und wähle dein **Unternehmen** aus der Liste in der oberen linken Ecke.
2. Unter **Nutzerverwaltung** klicke auf **Admin-Rollen**.
3. Im rechten Bereich suche die Admin-Rolle aus, die du zuweisen möchtest (zum Beispiel **Datenverwaltungs-Admin**, **Admin für sensible Inhalte** oder **eDiscovery-Admin**).
4. Klicke auf die **Ellipse (… )** neben der Rolle und wähle **Rolle zuweisen** aus.
5. Wähle den Nutzer aus, dem du die Rolle zuweisen möchtest.
6. Scrolle zum Ende des Fensters und klicke auf **Zuweisen**.

## Benutzerdefinierte Admin-Rollen für Enterprise Guard

Benutzerdefinierte Admin-Rollen ermöglichen es Unternehmens-Admins, den Zugriff auf einzelne Enterprise Guard-Funktionen zu gewähren, ohne breitere administrative Rollen zu vergeben. Dies ermöglicht es Organisationen, den Zugriff basierend auf internen Governance-, Sicherheits- oder Compliance-Verantwortlichkeiten anzupassen.

Beim Erstellen oder Bearbeiten einer benutzerdefinierten Admin-Rolle können Unternehmens-Admins die Berechtigungen auswählen, die bestimmen, auf welche Enterprise Guard-Funktionen die Rolle zugreifen und welche sie verwalten kann. Diese Berechtigungen erstrecken sich über mehrere Enterprise Guard-Domains wie Klassifizierung, Datenerkennung, Content Lifecycle Management, eDiscovery.

Indem nur die erforderlichen Berechtigungen zugewiesen werden, können Organisationen administrative Aufgaben wie das Überprüfen sensibler Inhalte, das Verwalten von Klassifizierungseinstellungen, das Konfigurieren von Lebenszyklusrichtlinien oder den Zugriff auf eDiscovery-Tools an die entsprechenden Teams delegieren. Die nachstehende Tabelle listet die Berechtigungen auf, die beim Konfigurieren benutzerdefinierter Admin-Rollen zugewiesen werden können.

|  |  |  |
| --- | --- | --- |
| **Fähigkeit** | **Berechtigung** | **Beschreibung** |
| **Datenklassifizierung** | Datenklassifizierungseinstellungen ansehen | Admin kann die Klassifizierungseinstellungen des Unternehmens aufrufen. |
| Einstellungen für die automatische Klassifizierung bearbeiten | Admin kann die Einstellungen des Unternehmens für die automatische Klassifizierung bearbeiten. |
| **Datenerkennung** | Einstellungen der Datenerkennung ansehen | Admin kann die Einstellungen der Datenerkennung des Unternehmens aufrufen. |
| Einstellungen zur Datenerkennung verwalten | Admin kann die Einstellungen der Datenerkennung des Unternehmens verwalten. |
| Ergebnisse der Datenerkennung ansehen | Admin kann die Ergebnisse der Datenerkennung ansehen. |
| Ergebnisse der Datenerkennung verwalten | Admin kann die Ergebnisse der Datenerkennung verwalten. |
| **eDiscovery** | Einstellungen zu Aufbewahrungsfristen ansehen | Admin kann Aufbewahrungsfristen auf der Seite der eDiscovery-Untersuchungseinstellungen aufrufen. |
| Einstellungen zu Aufbewahrungsfristen verwalten | Admin kann Aufbewahrungsfristen auf der Seite der eDiscovery-Untersuchungseinstellungen verwalten. |
| Exporte von Boards ansehen | Admin kann eDiscovery-Board-Exporte ansehen. |
| Exporte von Boards verwalten | Admin kann eDiscovery-Board-Exporte verwalten. |
| **Content Lifecycle Management** | Papierkorbeinstellungen ansehen | Admin kann die Papierkorbeinstellungen der Organisation ansehen. |
| Papierkorbeinstellungen verwalten | Admin kann die Papierkorb-Berechtigungen verwalten und festlegen, wie lange Boards im Papierkorb bleiben. |
| Aufbewahrungseinstellungen des Content Lifecycle ansehen | Admin kann die Seite mit den Aufbewahrungseinstellungen des Content Lifecycle aufrufen. |
| Content Lifecycle Aufbewahrungseinstellungen verwalten | Admin kann die Seite mit den Aufbewahrungseinstellungen für den Content Lifecycle verwalten. |
| Content Lifecycle Löschungseinstellungen ansehen | Admin kann die Seite mit den Löschungseinstellungen des Content Lifecycle aufrufen. |
| Content Lifecycle Löschungseinstellungen verwalten | Admin kann die Seite mit den Löschungseinstellungen für den Content Lifecycle verwalten. |
| Inhalte ansehen, die von Aufbewahrungs- oder Löschungsrichtlinien betroffen sind | Ermöglicht dem Nutzer, Inhalte aufzurufen, für die eine Aufbewahrungs- oder Löschungsrichtlinie gilt. |
