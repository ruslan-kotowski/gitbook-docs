---
title: "Einrichten von Microsoft Purview DSPM f\xFCr Miro AI (Beta)"
article_id: 28698434922386
translation_id: 28698434922386
locale: de
sidebar_position: 8
created_at: '2025-08-11T19:20:50Z'
updated_at: '2026-01-12T11:28:20Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Verwende diese Anleitung, um Microsoft Purview Data Security Posture Management (DSPM) für Miro AI einzurichten, sodass AI-Prompts und -Antworten aus Miro in Microsoft Purviews DSPM für KI angezeigt werden. Nach der Einrichtung validierst du Ereignisse und lernst, wie du die Integration verwaltest.

## **Voraussetzungen**

### **Miro**

- Enterprise-Preisplan mit aktiviertem **Enterprise Guard**.
- Du bist ein **Company Admin**.
- **Microsoft Entra ID** ist als **SSO-Anbieter** in Miro konfiguriert.
- Um diese Funktion in der Beta-Version zu aktivieren, kontaktiere deinen Customer Success Manager.

### **Microsoft**

- Aktive Microsoft Purview-Lizenz mit Support für DSPM für KI.
- Microsoft Entra ID-Mandanten-ID, die für Miro Single Sign-On verwendet wird (die GUID, die Ihre Microsoft-Organisation/Ihren Mandanten identifiziert).
- Eine Entra-Rolle, die eine mandantenweite Admin-Zustimmung für eine App erteilen kann.

## **Integration in Miro einrichten**

1. Öffne in Miro die **Enterprise-Einstellungen → Enterprise-Integrationen**.
2. Scrolle nach unten und klicke dann, um **Microsoft Purview DSPM für AI** zu aktivieren.
3. Gib im Feld "Tenant ID" deine **Microsoft Entra Tenant ID** ein.
4. Klicke auf **Verbinden**.
5. Melde dich bei Microsoft Entra mit einem Konto an, das **tenant-weite Admin-Zustimmung** erteilen kann, wenn du dazu aufgefordert wirst.
6. Überprüfe die Zustimmung für die **Miro AI Governance** App und klicke auf **Akzeptieren**.
7. Kehre zu Miro zurück und bestätige, dass die Integration als **Verbunden** angezeigt wird.

## **Aktivität in Microsoft Purview validieren**

1. Führe in Miro eine einfache KI-Aktion aus (zum Beispiel, **fasse** Haftnotizen auf einem Board zusammen).
2. Warte **bis zu 10–30 Minuten** auf die Übertragung.
3. Gehe in Microsoft Purview zu **Microsoft Purview → DSPM für AI → Aktivitäts-Explorer** (die Purview-Ansicht, die KI-Aktivitäten auflistet). Du kannst auch Informationen in den Audit-Protokollen einsehen.
   Hinweis: Alle textbasierten Prompts und Antworten in den Miro AI-Funktionen werden an Purview weitergeleitet. Derzeit werden Bildinhalte nicht an Microsoft Purview weitergeleitet.
4. Filtere nach **aktuellen** Ereignissen und finde Aktivitäten von Miro (zum Beispiel, Prompt und Antwort).

## **Integration verwalten**

- **Trennen**: Gehe in Miro zu **Enterprise-Integrationen → Microsoft Purview für AI → Trennen**.
- **Mandant wechseln**: Zuerst **trennen**, dann erneut **verbinden** mit einer anderen **Mandanten-ID**.

## **Fehlerbehebung**

- **Integrationsoption fehlt**: Stelle sicher, dass deine Organisation **Enterprise Guard** hat und dein Konto Zugriff auf **Enterprise-Integrationen** hat. Bitte einen **Company Admin**, dir Zugriff zu gewähren.
- **Mandanten-ID stimmt nicht überein oder Verbindungsfehler**: Die Mandanten-ID muss **exakt mit** dem Microsoft Entra-Mandanten übereinstimmen, der für Miro **SSO** verwendet wird.
- **Zustimmung fehlgeschlagen oder Anmeldeschleife**: Melde dich mit einem Konto an, das **Mandantenweite Admin-Zustimmung** erteilen kann (arbeite mit deinem Microsoft-Admin zusammen).
- **Keine Aktivitäten sichtbar**: Bestätige, dass eine Test-AI-Aktion von einem Nutzer durchgeführt wurde, der sich über den **konfigurierten Mandanten** bei Miro anmeldet; erlaube **10-30 Minuten**; überprüfe deine **Purview-Lizenz**; und überprüfe **DSPM für AI → Aktivitäts-Explorer**.
- **Mehrere Mandanten/IdPs**: Es kann nur **ein Mandant** in Miro konfiguriert werden. Aktivitäten von Nutzern, die sich über Single Sign-on für andere Mandanten/Identitätsanbieter anmelden, werden **nicht** weitergeleitet.

## **Bekannte Einschränkungen**

Weitere Informationen findest du im [Abschnitt zu bekannten Einschränkungen in der Übersichts-Dokumentation](../../enterprise-subscription-management/integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).
