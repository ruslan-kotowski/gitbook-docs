---
title: "\xDCbersicht und Szenarien zur automatischen Klassifizierung"
article_id: 15431302000914
translation_id: 15431302000914
locale: de
sidebar_position: 2
created_at: '2023-11-29T16:42:42Z'
updated_at: '2025-11-25T15:39:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Um dich beim Schutz deiner sensiblen Inhalte zu unterstützen, gibt es im Enterprise Guard die automatische Klassifizierung. Dabei handelt es sich um einen automatisierten Datenklassifizierungsprozess, der Miro-Boards nach der Stufe ihrer sensiblen Inhalte kategorisiert. Die automatische Klassifizierung stellt einen wesentlichen Fortschritt bei der Verwaltung und dem Schutz deiner sensiblen Daten dar, denn die Automatisierung dieses Prozesses hilft deiner Organisation, ein höheres Maß an Datensicherheit zu gewährleisten, die regulatorischen Anforderungen einzuhalten und die Sicherheit besser zu verwalten. Der Übergang von der manuellen zur automatischen Klassifizierung ist ein strategischer Schritt in Richtung eines genaueren, sichereren und effizienteren Frameworks für die Datensicherheit.

## Szenarien für die automatische Klassifizierung

### Voraussetzungen

Um die automatische Klassifizierung zu nutzen, musst du:

- [die Datenerkennung aktivieren](../data-discovery/13-activate-privacy-related-data-discovery.md)
- [die Klassifizierungsstufen definieren](07-define-classification-levels.md)

### Beispiel für die Konfiguration der automatischen Klassifizierung und der Vorgaben

Du musst die [automatische Klassifizierung und die Vorgaben](https://help.miro.com/hc/articles/15853672236946) entsprechend deinen Sicherheits- und Governance-Vorgaben konfigurieren. Die folgende Tabelle listet die Konfiguration auf, die für alle Beispielszenarien auf dieser Seite verwendet wird. Sie dient nur zur Erläuterung.

|  |  |  |  |
| --- | --- | --- | --- |
| **Board-Klassifizierung** | **Anordnung nach Sensibilität** | **Kriterien für die automatische Klassifizierung** | **Vorgaben** |
| ÖFFENTLICH | 1  (am wenigsten sensibel) | kein Status | kein Status |
| INTERN (Standard) | 2 | TELEKOMM | - Öffentliche Freigabe blockieren |
| VERTRAULICH | 3 | DSGVO  PCI DSS | - Öffentliche Freigabe blockieren  - Freigabe für Teams blockieren |
| EINGESCHRÄNKT | 4 (am sensibelsten) | HIPAA  ANMELDEINFORMATIONEN | - Öffentliche Freigabe blockieren  - Freigabe für Teams blockieren  - Freigabe für die Organisation blockieren |

*Tabelle 1: Diese Beispielkonfiguration dient nur zur Erläuterung.*

## Manuelle Aktualisierung der Board-Klassifizierung, um die automatische Klassifizierung zu überschreiben

Nur Board-Eigentümer, Miteigentümer oder Bearbeiter des Boards können die Board-Klassifizierung ändern, um die automatische Klassifizierungsstufe außer Kraft zu setzen. Wenn der Board-Eigentümer, die Miteigentümer oder die Bearbeiter die Board-Klassifizierung auf eine weniger sensible Klassifizierungsstufe heruntersetzen, müssen sie einen Grund für die Änderung auswählen oder angeben. Diese Informationen werden in den Audit-Protokollen erfasst.

### Manuelle Änderung auf eine weniger sensible Klassifizierungsstufe

**Szenario**
Schauen wir uns ein Szenario an, in dem John Smith der Eigentümer eines Boards ist, das automatisch als **vertraulich** klassifiziert wurde und in unserer Konfiguration die Sensibilitätsstufe **3** hat.

John sieht sich die Informationen an und beschließt, die Klassifizierungsstufe auf **Intern** zu ändern, was die Sensibilitätsstufe **2** hat. Dies ist eine niedrigere Klassifizierungsstufe als die automatische Klassifizierungsstufe des Boards **Vertraulich**, Stufe **3**.

:::note
Nur Board-Eigentümer, Miteigentümer oder Bearbeiter des Boards können die Klassifizierungsstufe manuell ändern.
:::

**Ergebnis**

Da John der Board-Eigentümer ist, kann er die Board-Klassifizierung auf eine weniger sensible Klassifizierungsstufe ändern, **Intern**, Stufe **2**. In diesem Szenario wird John aufgefordert, den Grund anzugeben, warum er die Board-Klassifizierungsstufe in eine niedrigere Klassifizierungsstufe ändern möchte (Abbildung 1). John muss einen Grund auswählen und auf **Aktualisieren** klicken.

Die Board-Klassifizierungsstufe wird aktualisiert, und die Informationen zu diesem Update werden den Audit-Protokollen hinzugefügt.

### Manuelle Änderung auf eine sensiblere Klassifizierungsstufe

**Szenario**

Schauen wir uns ein Szenario an, in dem John Smith der Eigentümer eines Boards ist, das automatisch als **vertraulich** klassifiziert wurde und in unserer Konfiguration die Sensibilitätsstufe **3** hat.

John sieht sich die Informationen an und beschließt, die Klassifizierungsstufe auf **Eingeschränkt** zu ändern, was die höchste Sensibilitätsstufe **4** hat. Dies ist eine höhere Klassifizierungsstufe als die automatische Klassifizierungsstufe des Boards **Vertraulich**, Stufe **3**.

:::note
Nur Board-Eigentümer, Miteigentümer oder Bearbeiter des Boards können die Klassifizierungsstufe manuell ändern.
:::

**Ergebnis**

Da John der Board-Eigentümer ist, kann er die Board-Klassifizierung auf eine sensiblere Klassifizierungsstufe ändern.

Die folgende Tabelle fasst verschiedene Szenarien und ihre Ergebnisse zusammen – unter der Voraussetzung, dass das Board zu einem früheren Zeitpunkt bereits automatisch klassifiziert wurde und dann ein Board-Eigentümer, ein Miteigentümer oder ein Bearbeiter die Board-Klassifizierung manuell ändert.

|  |  |  |
| --- | --- | --- |
| **Einstufung der automatischen Klassifizierung** | **Änderung durch den Board-Eigentümer** | **Neue Klassifizierungsstufe** |
| VERTRAULICH | **Änderung auf eine niedrigere Klassifizierungsstufe**  John, der Board-Eigentümer, ändert die Board-Klassifizierung manuell auf  **INTERN**, das die Sensibilitätsstufe 2 hat, eine niedrigere Klassifizierungsstufe als die automatische Klassifizierungsstufe des Boards VERTRAULICH, Stufe 3. | Da John der Board-Eigentümer ist, kann er die Board-Klassifizierung auf eine weniger sensible Klassifizierungsstufe ändern: **INTERN**.  In diesem Szenario wird der Board-Eigentümer aufgefordert, den Grund anzugeben, warum er die Board-Klassifizierungsstufe in eine weniger sensible Klassifizierungsstufe ändern möchte. John muss einen Grund auswählen und auf **Aktualisieren** klicken.  Die Board-Klassifizierungsstufe wird auf **INTERN** geändert und die Informationen zu diesem Update werden den Audit-Protokollen hinzugefügt. |
| VERTRAULICH | **Änderung auf eine höhere Klassifizierungsstufe**  John, der Board-Eigentümer, beschließt, die Board-Klassifizierung auf **EINGESCHRÄNKT** zu ändern, was die höchste Sensibilitätsstufe 4 hat. Dies ist eine höhere Klassifizierungsstufe als die automatische Klassifizierungsstufe des Boards VERTRAULICH, Stufe 3. | Da John der Board-Eigentümer ist, kann er die Board-Klassifizierung auf eine sensiblere Klassifizierungsstufe ändern. |

*Tabelle 2: Szenarien und die daraus resultierenden automatischen Klassifizierungsstufen*

## Automatische Änderung der Board-Klassifizierung

Jede Stunde wird eine Datenerkennung durchgeführt. Wenn sich der Board-Inhalt ändert oder hochsensible Daten hinzugefügt oder entfernt werden, werden die Boards, an denen Änderungen vorgenommen wurden, erneut automatisch klassifiziert. Diese Klassifizierung basiert auf den aktualisierten Inhalten des Boards und der letzten nicht-automatischen Klassifizierungsstufe. Die folgenden Abschnitte enthalten Beispielszenarien für eine automatische Änderung der Klassifizierungsstufe.

### Hochsensible Daten wurden vom Board entfernt

Nachdem die Datenerkennung abgeschlossen ist, ändert sich die Board-Klassifizierung automatisch auf die entsprechende Sensibilitätsstufe.

**Beispielszenario: Board-Inhalte**

Das Board enthält hochsensible Daten, die Informationen enthalten, die zu den folgenden Sensibilitätslabels gehören: ANMELDEINFORMATIONEN, HIPPA, DSGVO, PCI DSS Nachdem die Datenerkennung abgeschlossen ist, wurde dieses Board durch die automatische Klassifizierung als **EINGESCHRÄNKT**, Stufe 4 klassifiziert. Dies ist die höchste Sensibilitätsstufe, basierend auf unserer Beispielkonfiguration für die automatische Klassifizierung. In dieser Tabelle werden folgende Informationen beschrieben:

- **Letzte nicht automatische Klassifizierung:** Dies ist die letzte nicht-automatische Klassifizierung des Boards, die entweder [manuell](03-auto-classification-overview-and-scenarios.md) über eine [standardmäßige Board-Klassifizierung](../data-security/02-data-classification.md) oder die APIs für die [Änderung der Board-Klassifizierung](https://developers.miro.com/reference/enterprise-dataclassification-board-set) bzw. die [Änderung der Board-Klassifizierung als Massenaktion](https://developers.miro.com/reference/enterprise-dataclassification-team-boards-bulk) vorgenommen wurde.

- **Automatische Klassifizierung:** Die Klassifizierungsstufe, die die automatische Klassifizierung nach Abschluss der Datenerkennung auf das Board angewendet hat.

- **Vorgenommene Änderungen:** Änderungen an den Board-Inhalten, die nach der automatischen Klassifizierung durchgeführt wurden

- **Neue Klassifizierung:** Die neue Klassifizierung berücksichtigt die vorgenommenen Änderungen und alle anderen Aspekte, wie die Board-Inhalte und die letzte nicht-automatische Klassifizierung.

|  |  |  |  |
| --- | --- | --- | --- |
| **Letzte nicht-automatische Klassifizierung** | **Automatische Klassifizierung** | **Nutzeraktion** | **Neue automatische Klassifizierungsstufe** |
| INTERN (über die standardmäßige Board-Klassifizierung) | EINGESCHRÄNKT | Alle sensiblen Daten wurden vom Board entfernt | Nachdem die Datenerkennung abgeschlossen ist, ändert sich die Board-Klassifizierung automatisch auf die Stufe **INTERN**, da das Board keine sensiblen Informationen mehr enthält. Die frühere nicht-automatische Klassifizierung war INTERN, was über die standardmäßige Board-Klassifizierung klassifiziert wurde. |
| VERTRAULICH | EINGESCHRÄNKT | Alle sensiblen Daten wurden vom Board entfernt | Nachdem der nächste Datenerkennung abgeschlossen ist, ändert sich die Board-Klassifizierung automatisch auf die Stufe **VERTRAULICH**. Das ist die Sensibilitätsstufe 3. Dies gilt auch dann, wenn das Board keine sensiblen Informationen mehr enthält, weil die frühere nicht-automatische Klassifizierungsstufe VERTRAULICH, Stufe 3 war. |
| NICHT KLASSIFIZIERT | EINGESCHRÄNKT | Inhalte, die ANMELDEINFORMATIONEN und HIPAA enthalten, was die Stufe EINGESCHRÄNKT hat, die Sensibilitätsstufe 4 hat, werden vom Board entfernt. | Nachdem die Datenerkennung abgeschlossen ist, ändert sich die Board-Klassifizierung automatisch auf **VERTRAULICH**, was die Sensibilitätsstufe 3 hat:. - Das Board enthält keine ANMELDEINFORMATIONEN und HIPAA-Gesundheitsdaten, aber es enthält sensible PCI-DSS-Daten, wodurch es in **VERTRAULICH** eingestuft wurde. - Das Board wurde vor der automatischen Klassifizierung noch nicht klassifiziert. |
| Eingeschränkt | Eingeschränkt | Inhalte, die ANMELDEINFORMATIONEN und HIPAA enthalten, was die Stufe EINGESCHRÄNKT hat, die Sensibilitätsstufe 4 hat, werden vom Board entfernt. | Nachdem die Datenerkennung abgeschlossen ist, bleibt das Board in der Stufe **EINGESCHRÄNKT**, was die Sensibilitätsstufe 4 hat, auch wenn das Board keine ANMELDEINFORMATIONEN und HIPAA-Daten mehr enthält, aber die frühere nicht-automatische Klassifizierungsstufe war EINGESCHRÄNKT (Stufe 4). |
| NICHT KLASSIFIZIERT | EINGESCHRÄNKT | Alle sensiblen Daten wurden vom Board entfernt | Nachdem die Datenerkennung abgeschlossen ist, ändert sich die Board-Klassifizierung automatisch auf **NICHT KLASSIFIZIERT**, da das Board keine sensiblen Informationen mehr enthält und das Board vor der automatischen Klassifizierung noch nicht klassifiziert wurde. |

*Tabelle 3: Szenarien und die daraus resultierenden automatischen Klassifizierungsstufen*

### Hochsensible Daten wurden zum Board hinzugefügt

Nachdem die Datenerkennung abgeschlossen ist, ändert sich die Board-Klassifizierung automatisch auf die entsprechende Sensibilitätsstufe, basierend auf der höchsten Stufe der gefundenen sensiblen Daten.

|  |  |  |
| --- | --- | --- |
| **Letzte automatische Klassifizerungsstufe** | **Nutzeraktion** | **Neue automatische Klassifizierungsstufe** |
| ÖFFENTLICH | Mitwirkende haben eine Kreditkartennummer hinzugefügt | **VERTRAULICH** PCI DSS |
| Intern | Mitwirkende haben ein Authentifizierungstoken hinzugefügt | **EINGESCHRÄNKT** ANMELDEINFORMATIONEN |
| Eingeschränkt | Mitwirkende haben ein Authentifizierungstoken hinzugefügt | **EINGESCHRÄNKT** Bleibt unverändert |
| Intern | Mitwirkende haben eine deutsche Führerscheinnummer hinzugefügt | **VERTRAULICH**  DSGVO |
| VERTRAULICH | Mitwirkende haben eine MAC-Adresse hinzugefügt | **EINGESCHRÄNKT**  Anmeldeinformationen |

*Tabelle 4: Szenarien und die daraus resultierenden automatischen Klassifizierungsstufen*
