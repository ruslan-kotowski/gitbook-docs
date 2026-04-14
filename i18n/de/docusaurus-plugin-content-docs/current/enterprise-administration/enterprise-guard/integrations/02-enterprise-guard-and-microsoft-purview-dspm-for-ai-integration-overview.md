---
title: "Enterprise Guard und Microsoft Purview DSPM f\xFCr KI Integration \xDCbersicht\
  \ (Beta)"
article_id: 28617278171154
translation_id: 28617278171154
locale: de
sidebar_position: 0
created_at: '2025-08-07T15:17:38Z'
updated_at: '2026-01-12T11:27:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Für Organisationen, die Microsoft Entra ID (vormals Azure AD) als ihren Identitätsanbieter nutzen, leitet Enterprise Guard AI-Prompts und -Antworten sicher an Microsoft Purview Data Security Posture Management (DSPM) weiter. Sicherheits- und Compliance-Teams können dann die Nutzung generativer KI von einer einzigen vertrauenswürdigen Plattform aus überwachen, prüfen und kontrollieren, um den Betriebsaufwand zu reduzieren, Risiken wie Datenlecks und Missbrauch zu mindern und die KI-Governance von Miro in Unternehmensqualität zu stärken.

:::note
Die Beta-Version unterstützt Miro AI-Formate wie Diagramme, Mindmaps, Dokumente, Prototypen, Notizen und Tabellen, jedoch keine Bilder. Wir arbeiten daran, Unterstützung für Bilder und weitere AI-Funktionen in künftigen Versionen hinzuzufügen.
:::

## **Für wen das ist**

Diese Funktion ist in der Beta-Version für Enterprise Guard-Kunden verfügbar, die Miro und Microsoft Entra ID (vormals Azure AD)/Microsoft Purview verwalten.

## **Was du erhältst**

- **Zentralisierte Transparenz:** Die Nutzung von Miro AI im AI Hub von Microsoft Purview ansehen.
- **Prüfbarkeit:** Prompts (Nutzereingaben) und Antworten (KI-Ausgaben) werden zur Überprüfung protokolliert.
- **Governance-Ausrichtung:** Verwende deine bestehenden Purview-Workflows für Überwachung, Benachrichtigung und Aufbewahrung.

## **Anforderungen**

### **Miro**

- Enterprise-Preisplan mit **Enterprise Guard** aktiviert.
- Du bist ein **Unternehmens-Admin**.
- Microsoft **Entra ID** als Single Sign-on-Anbieter in Miro konfiguriert.
- Zugriff auf die Seite **Enterprise Integrations** (wenn du sie nicht sehen kannst, bitte einen **Unternehmens-Admin**, dir Zugriff zu gewähren).
- Um dieses Feature in der Beta zu aktivieren, wende dich an deinen Customer Success Manager.

### **Microsoft**

- Aktive **Microsoft Purview**-Lizenz.
- Deine **Microsoft Entra ID Tenant-ID** (derselbe Tenant, der für Miro Single Sign-on verwendet wird; die GUID, die deine Microsoft-Organisation/Tenant identifiziert).
- Eine Entra-Rolle, die **eine tenantweite Admin-Zustimmung** zu einer App erteilen kann.

## **So funktioniert's**

1. Ein Miro-Admin verbindet deinen Microsoft Entra-Tenant von der Seite **Enterprise Integrations** in Miro.
2. Dies installiert die **Miro AI Governance**-App in deinem Microsoft-Tenant (über tenantweite Admin-Zustimmung).
3. Wenn Nutzer sich über diesen Tenant bei Miro anmelden und Miro AI verwenden, leitet Miro die Aufforderung/Antwort an Microsoft Purview weiter.
4. Aktivitäten erscheinen im **DSPM für KI → Aktivitätsexplorer** (Purview-Ansicht, die KI-Aktivitäten auflistet) in Microsoft Purview (Einführungszeit berücksichtigen).

## **Datentransparenz & Latenz**

- Protokollierte Daten: **AI-Prompts und -Antworten**, die in Miro von Nutzern generiert werden, die sich über Single Sign-on (SSO) beim konfigurierten Mandanten anmelden.
- Wo kann man es sehen: **Microsoft Purview → DSPM für KI → Aktivitätsexplorer** (die Purview-Ansicht, die KI-Aktivitäten auflistet). Du kannst auch Informationen in den Audit-Protokollen ansehen.
  **Hinweis:** Alle textbasierten Prompts und Antworten über Miro AI-Funktionen hinweg werden an Purview weitergeleitet. Derzeit wird Bildinhalt nicht an Microsoft Purview weitergeleitet.
- Latenz: Aufzeichnungen erscheinen in der Regel **innerhalb von 10–30 Minuten** nach der AI-Aktion in Miro.

## **Bekannte Einschränkungen**

- Die Beta-Version unterstützt Miro AI-Formate, darunter Diagramme, Mindmaps, Dokumente, Prototypen, Notizen und Tabellen, aber keine Bilder. Wir arbeiten daran, Unterstützung für Bilder und weitere AI-Funktionen in zukünftigen Versionen hinzuzufügen.
- Du kannst jeweils **eine Microsoft Entra Tenant-ID** in Miro konfigurieren.
- In Multi-IdP- oder Multi-Tenant-Umgebungen werden **nur** Aktivitäten von Nutzern, die sich über den **konfigurierten Mandanten** bei Miro anmelden, an Microsoft Purview protokolliert.

## **Sicherheit und Datenschutz**

Miro leitet AI-Prompts und -Antworten an **deinen Microsoft-Mandanten** weiter, damit sie in Purview überwacht werden können. **Governance, Aufbewahrung und Zugriffskontrollen** werden in deiner Microsoft-Umgebung verwaltet.

##

## **FAQs**

- **F: Welche Miro AI-Funktionen werden protokolliert?**
  **A:** Alle textbasierten Prompts und Antworten über Miro AI-Funktionen werden an Purview weitergeleitet. Derzeit werden Bildinhalte nicht an Microsoft Purview weitergeleitet.
- **F: Deckt dies alle Nutzer ab?**
  **A:** Nur Nutzer, die sich mithilfe des konfigurierten Microsoft-Entra-Mandanten bei Miro authentifizieren, sind abgedeckt.
- **F: Kann ich Protokolle aus Miro exportieren?**
  **A:** Microsoft Purview für Export und Aufbewahrung verwenden. Miro leitet Aktivitätsdaten an deinen Microsoft-Tenant weiter, wo sie durch deine Richtlinien verwaltet werden.
- **F: Wie steht es mit Sicherheit und Datenschutz?**
  **A:** Miro leitet AI-Prompts und -Antworten an **deinen Microsoft-Tenant** weiter, damit sie in Purview überwacht werden können. **Governance, Aufbewahrung und Zugriffskontrollen** werden in deiner Microsoft-Umgebung verwaltet.

## **Support und Ressourcen**

- Informationen zu den Voraussetzungen für die Entra-Zustimmung findest du in der Microsoft-Dokumentation zu **gewähren der Mandantenweiten Admin-Zustimmung** für eine App.
- Anweisungen zur Einrichtung von Enterprise Guard findest du in [dieser Dokumentation](../../enterprise-subscription-management/integrations/03-set-up-microsoft-purview-dspm-for-miro-ai.md).
