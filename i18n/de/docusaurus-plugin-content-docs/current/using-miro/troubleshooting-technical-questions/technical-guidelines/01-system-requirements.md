---
title: Systemanforderungen
article_id: 360017731553
translation_id: 360017731553
locale: de
sidebar_position: 1
created_at: '2019-02-11T10:14:54Z'
updated_at: '2026-03-06T14:57:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Dieser Artikel skizziert die Systemanforderungen für die Nutzung von Miro, einschließlich Gerät, GPU und WebAssembly.

Für die Arbeit in Miro stelle bitte sicher, dass dein Gerät die folgenden Mindest- oder empfohlenen Systemanforderungen erfüllt.

Bitte beachte jedoch, dass die unten genannten Parameter nicht endgültig sind, da die Miro-Leistung von mehreren anderen Faktoren abhängen kann, wie:

- Aufgaben im Hintergrund
- Anzahl der Tabs im Browser und wie oft du zwischen ihnen wechselst
- Die Auflösung des Monitors, auf dem du Miro öffnest
- Stabilität der WLAN-Verbindung
- Anzahl der Nutzer auf dem Board
- Gerätekühlsystem

Bei Leistungs- oder Zugangsproblemen bitte die [Fehlerbehebung](../troubleshooting) und die [Tipps zur Optimierung der Board-Leistung](../../tools/troubleshooting/04-board-performance-and-loading-issues.md) prüfen.

|  |  |  |
| --- | --- | --- |
|  | **Minimum** | **Empfohlen** |
| **CPU** | 3 GHz (2 Prozessorkerne/4 Threads) | 2,8 GHz (4 Prozessorkerne/8 Threads) |
| **RAM-Speicher** | 8 GB | 16 GB (DDR4) |
| **Netzwerkbandbreite** | 8 Mb/s | 32 Mb/s |

**Bitte beachte, dass die Ausführung von Miro auf High-End-Hardware, die weit über den empfohlenen Spezifikationen liegt, möglicherweise nicht den erwarteten Leistungsschub bringt, da Miro eine Web-App ist, die mit einer Browser-Web-Engine arbeitet. Die Web-Engine ist nicht in der Lage, das volle Potenzial des Geräts auszuschöpfen, da die Software lokal auf deinem Computer installiert ist und für ein bestimmtes Betriebssystem und eine bestimmte CPU-Architektur ausgelegt ist.*

Minimale Systemanforderungen für eine komfortable Nutzung von Miro auf [Tablets](../../../getting-started/apps-for-devices/11-tablet-app.md) sind 6 GB RAM.

Miro kann auf verschiedenen Gerätetypen verwendet werden. Du kannst Miro in einem Browser öffnen, die [Desktop](../../../getting-started/apps-for-devices/05-desktop-app.md)-, [Tablet](../../../getting-started/apps-for-devices/11-tablet-app.md)-, [mobile App](../../../getting-started/apps-for-devices/08-mobile-app.md) herunterladen oder [Miro auf einem interaktiven Display verwenden](../../../getting-started/apps-for-devices/07-interactive-displays.md).

**Offline-Modus**

Da sich Miro auf die Vision einer nahtlosen Cloud-Lösung für *Online*-Zusammenarbeit stützt, steht der *Offline*-Modus des Tools derzeit nicht auf unserem Plan. Wir bieten jedoch mehrere Exportoptionen an. [Mehr erfahren](../../import-and-export/export/03-how-to-export-your-board.md).

## GPU- und WebAssembly-Anforderungen

Miro nutzt die GPU-Hardwarebeschleunigung und WebAssembly (WASM) für eine flüssige Darstellung und zur Unterstützung bestimmter erweiterter Funktionen.

### Miro ohne GPU nutzen

Für optimale Leistung erfordert Miro GPU-Hardwarebeschleunigung.

Wenn die GPU-Hardwarebeschleunigung nicht verfügbar ist, beispielsweise auf einigen virtuellen Maschinen oder wenn die Hardwarebeschleunigung deaktiviert ist, wechselt Miro automatisch zu einem CPU-basierten Renderer.

:::tip
Halte die Hardwarebeschleunigung wenn möglich aktiviert, um das bestmögliche Miro-Erlebnis zu gewährleisten.
:::

Ohne GPU-Hardwarebeschleunigung kannst du folgende Leistungsänderungen feststellen:

- Einige GPU-abhängige Funktionen stehen möglicherweise nicht zur Verfügung oder werden als Platzhalter angezeigt
- Langsameres Verschieben und Zoomen, insbesondere bei großen Boards oder Boards mit vielen Medien
- Kernfunktionen des Boards funktionieren möglicherweise nicht wie erwartet
- Höherer CPU-Verbrauch

### Nutzung von Miro ohne WebAssembly (WASM)

Einige Miro-Funktionen basieren auf WebAssembly (WASM)-Modulen.

Die meisten modernen Browser aktivieren WASM standardmäßig. Ist WASM nicht verfügbar, etwa weil es aufgrund von Compliance-Vorgaben blockiert, im Browser deaktiviert oder in älteren Umgebungen nicht unterstützt wird, wechselt Miro, wo möglich, automatisch zu Rendering-Pfaden auf JavaScript-Basis.

**Mehr Informationen:** Siehe [Wie überprüft man, ob WASM in Ihrem Browser unterstützt wird](https://help.miro.com/hc/articles/33769132852498).

:::tip
Um die beste Miro-Erfahrung zu gewährleisten, halten Sie WebAssembly aktiviert. Wenn Sie in einer verwalteten Umgebung vermuten, dass WASM blockiert ist, kontaktieren Sie Ihr IT-Team.
:::

Ohne WASM kann es zu folgenden Leistungsänderungen kommen:

- Funktionen, die WASM erfordern, können möglicherweise nicht initialisiert werden und werden verborgen oder als Platzhalter angezeigt
- Boards, die auf WASM-basierte Funktionalität angewiesen sind, können möglicherweise nicht vollständig geladen werden oder gar nicht laden
