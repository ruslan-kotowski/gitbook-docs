---
title: 'Enterprise Guard Einführungshandbuch Teil 2: Datensicherheit bereitstellen'
article_id: 17121026396690
translation_id: 17121026396690
locale: de
sidebar_position: 2
created_at: '2024-02-19T09:32:48Z'
updated_at: '2025-11-25T15:41:10Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: api-security
availability:
  notes: 'Relevante Teams: Beispiele für Teams, mit denen du zusammenarbeiten musst,
    um Datensicherheitsfunktionen zu implementieren, sind Datenschutz, Data Loss Prevention,
    Governance und Risiko, Anwendungssicherheit, digitale Informationen und Sicherheit
    und/oder Insider-Bedrohungen.'
---

## Überblick über die Datensicherheit

Finde, klassifiziere und sichere sensible Inhalte mit den Datensicherheitsfunktionen von Enterprise Guard.

- **Datenerkennung:** Entdecke sensible Daten wie personenbezogene Daten (Personal Identifiable Information, PII), persönliche Gesundheitsinformationen (Personal Health Information, PHI) und PCI-Daten (Payment Card Industry) mit nur wenigen Klicks.
- **Automatische Klassifizierung** Lege Kriterien fest, anhand derer Miro deine Boards automatisch nach sensiblen Inhalten klassifizieren kann.
- **Intelligente Vorgaben:** Setze Sicherheitsregeln in Echtzeit durch und schränke ein, was Nutzer mit einem Board auf der Grundlage der manuellen oder automatischen Klassifizierung des Boards tun können.
- **Inhaltssuche:** Du kannst alle Miro-Boards mit sensiblen Inhalten und die Klassifizierung der einzelnen Boards einheitlich ansehen.

![Enterprise-Guard-Datensicherheit.png](images/17121265800338_Enterprise-Guard-Data-Security.png)*Sensible Daten finden, klassifizieren und sichern*

## Übersicht über die Einsätze

Bei diesem Bereitstellungsansatz liegt der Schwerpunkt auf der Sicherung sensibler Daten, die durch die Datenerkennung von Enterprise Guard gefunden wurden, während die Aktivitäten der Nutzer so wenig wie möglich gestört werden.

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="390" scrolling="no" src="https://miro.com/app/live-embed/uXjVNrjv8h8=/?moveToViewport=-3966,-1331,10269,3273&amp;embedId=881755370090" width="690"></iframe> *Überblick über den Einsatz von Enterprise Guard*

#### Konfigurationsschritte

1. Sensible Daten prüfen
2. Klassifizierung konfigurieren
3. Klassifizierung veröffentlichen
4. Einsatz von Vorgaben
5. Beschränkungen der Decke lockern

#### Endnutzer-Kommunikation und Befähigungsschritte

1. Erstelle einen Preisplan für die Einführung
2. Erste Ankündigung von Enterprise Guard
3. Ankündigung der Einführung von Klassifizierungen
4. Unnötiges Auftauchen sensibler Daten klären
5. Ankündigung der Einführung von Leitplanken

## Sensible Daten prüfen

Führe die in diesem Abschnitt beschriebene Prüfung so früh wie möglich in deinem Enterprise Guard-Einsatz durch. Sie hat keinerlei Auswirkungen auf die Nutzer, ermöglicht es dir aber, den Geltungsbereich und den Schweregrad des Auftretens sensibler Daten in deiner Miro-Instanz zu beurteilen.

Nutze die Prüfungsergebnisse, um einen Preisplan für die Einführung zu erstellen, der die Änderungsverwaltung für die Nutzer mit den Richtlinien deines Unternehmens in Einklang bringt.

### Datenerkennung einschalten

Der erste Schritt bei der Konfiguration deiner Datenklassifizierung besteht darin, die Datenerkennung in deinem Miro Konto zu aktivieren. Miro scannt dann all deine Boards nach sensiblen Daten gemäß den aktivierten Richtlinien (Labels) für die Region und/oder die Datenschutzbestimmungen.

[Wie du die Datenerkennung in deiner Miro-Umgebung aktivierst](../../canvas-25-admin-features/data-discovery/13-activate-privacy-related-data-discovery.md)

Es kann bis zu 24 Stunden dauern, bis sensible Inhalte entdeckt werden. Sobald Miro die sensiblen Inhalte identifiziert hat, die mit diesen Labels übereinstimmen (z. B. GDPR, PCI), kann die Inhaltssuche verwendet werden, um die Ergebnisse im Detail zu überprüfen.

### Prüfung mit der Inhaltssuche

Mit der Inhaltssuche können Admins für sensible Inhalte die von Miro Enterprise Guard entdeckten Vorkommnisse sensibler Daten überprüfen. Sie erfahren, wo die Vorkommnisse stattgefunden haben (Board-Name), wer der Akteur ist (Board-Eigentümer), warum das Vorkommnis gekennzeichnet wurde (Label) und um welchen Inhalt es sich handelt.

Nutze die Filter in der Inhaltssuche, wie z. B. "Klassifizierung = Vertraulich", um dich auf die wichtigsten Vorkommen sensibler Daten zu konzentrieren.

## Erstelle einen Preisplan für die Einführung

Sobald die Datenerkennung aktiviert ist und sensible Inhalte aufgedeckt wurden, ist es an der Zeit, einen Preisplan für die Klassifizierungen und Vorgaben zu erstellen, der den Richtlinien, Anforderungen, dem Schweregrad der Ergebnisse und den verfügbaren Ressourcen deines Unternehmens entspricht. In den folgenden Abschnitten findest du Empfehlungen für die Kommunikation, um die Nutzer zu informieren und deinen Change Management-Prozess zu unterstützen.

### Kommende Änderungen ankündigen

Bevor du dein Klassifizierungs-Framework in Miro veröffentlichst, solltest du die Nutzer über die Entscheidung deines Unternehmens informieren, Enterprise Guard für alle Miro-Inhalte zu aktivieren, und den Kontext entsprechend den Richtlinien und Praktiken deines Unternehmens für die Datensicherheit bereitstellen.

Ziehe in Erwägung, die folgenden Informationen aufzunehmen:

- Was ist Enterprise Guard?
- Warum es für deine Organisation wichtig ist
- Überblick darüber, welche Aspekte der Endnutzer-Erfahrung betroffen sein werden
- Erläuterung des Klassifizierungsrahmens deines Unternehmens
- Welche Richtlinien zur Datenregulierung werden in die Datenerkennung einbezogen?
- Zeitachse der kommenden Änderungen
- An wen du dich mit Fragen und Feedback wenden kannst

## Klassifizierung konfigurieren

### Klassifizierungen hinzufügen Rahmen

Die Einrichtung von Datenklassifizierungen in Miro ist so konzipiert, dass sie flexibel ist und sich an alle bestehenden Datenklassifizierungssysteme in deinem Unternehmen anpassen lässt.

Die Klassifizierungsstufen in Miro zeigen ihre aktuelle Sensibilitätsreihenfolge an. Passe die Sensibilitätsstufe an die Klassifizierungshierarchie deines Unternehmens an, wobei die Sensibilitätsstufe 1 die am wenigsten sensible Klassifizierungsstufe ist.

[So konfigurierst du Klassifizierungen](../../canvas-25-admin-features/data-classification/07-define-classification-levels.md)

### Abflachung des Rahmens für die Klassifizierung

Die Klassifizierungsstruktur von Miro Enterprise Guard ist so konzipiert, dass sie sich an deine bestehenden Richtlinien zur Datenklassifizierung anpasst.

Wenn das bestehende Klassifizierungssystem deines Unternehmens mehr als eine Hierarchieebene hat (z. B. Unterklassifizierungsstufen oder Tags), muss dein Klassifizierungssystem möglicherweise abgeflacht werden. Das folgende Beispiel zeigt einen Klassifizierungsrahmen mit 3 Tags, der 3 verschiedene Klassifizierungsstufen pro Tag und Ebene erfordert.

Es wird empfohlen, die Klassifizierungsstufen auf ein Minimum zu beschränken.

![Enterprise-Guard-Flatten-Klassifizierung-Hierarchy.pngFlattening](images/17121454964370_Enterprise-Guard-Flatten-Classification-Hierarchy.png)
*classification frameworks*

### Dokumentation verlinken und Beschreibungen schreiben

Klare Klassifizierungsbeschreibungen und -richtlinien informieren deine Nutzer über die Klassifizierungsrichtlinien, und zwar im großen Maßstab. Wenn sich die Nutzer auf dem Board befinden, werden die Beschreibungen der Klassifizierung neben dem Label der Klassifizierung angezeigt. Endnutzer sehen in jedem Feld ein Fragezeichen "Mehr erfahren", das auf die Dokumentation zur Klassifizierung verweist.

|  |  |
| --- | --- |
| **Beschreibung der Klassifizierung** | Wenn Nutzer auf das Abzeichen für die Klassifizierung des Boards klicken, wird die Beschreibung der aktuellen Klassifizierungsstufe angezeigt.  Füge eine aussagekräftige Beschreibung hinzu, die deine Nutzer über die Sensibilität dieses Boards und die empfohlenen Vorsichtsmaßnahmen oder Aktionen informiert.  Klassifizierung-beschreibung.png |
| **Link zu den Richtlinien** | Wenn der Nutzer auf das Symbol (Fragezeichen) neben dem Abzeichen zur Klassifizierung des Boards klickt, wird diese URL in einem neuen Tab des Browsers geladen.  Gib deinen Nutzern mehr Informationen über die Klassifizierungsstufen deines Boards und wie sie damit arbeiten können.  Ziehe in Erwägung, sie einzubeziehen:   - Was ist Enterprise Guard? - Warum es für deine Organisation wichtig ist - Überblick darüber, welche Aspekte der Endnutzer-Erfahrung betroffen sein werden - Erläuterung des Klassifizierungsrahmens deines Unternehmens - Welche Richtlinien zur Datenregulierung werden in die Datenerkennung einbezogen? - An wen du dich mit Fragen und Feedback wenden kannst |

### Kriterien für die automatische Klassifizierung festlegen

Miro wendet die Klassifizierungen automatisch auf Boards an, deren Inhalte den entsprechenden Datenschutzbestimmungen entsprechen. Jede Klassifizierungsstufe kann mit mehreren [Labels](../../canvas-25-admin-features/data-discovery/06-sensitivity-labels-and-infotypes-reference.md) verknüpft werden, aber jedes Label kann nur mit einer einzigen Klassifizierungsstufe verknüpft werden.

Wenn mehrere Kriterien erfüllt sind, wird die sensibelste Klassifizierungsstufe angewendet.

[Wie man Auto-Klassifizierungen definiert](../../canvas-25-admin-features/data-classification/09-define-auto-classification.md)

### Vorgaben überspringen Konfiguration

Wie bereits erwähnt, geht es in diesem Leitfaden darum, neben dem Einsatz von Enterprise Guard auch die Änderungsverwaltung für die Nutzer in den Vordergrund zu stellen. Wir empfehlen, Klassifizierungen ohne Vorgaben zu veröffentlichen. Die Klassifizierung der Boards in dieser Konfiguration ist ein visueller Indikator, hat aber keinen Einfluss auf die Erfahrung des Nutzers.

Bevor du Vorgaben zu den Klassifizierungen hinzufügst, klärst du unnötige Vorkommnisse von sensiblen Daten und schaltest die Nutzer auf manuelle Klassifizierung um, um einen reibungslosen Übergang zu gewährleisten, ohne die wichtige Arbeit auf den Boards zu beeinträchtigen.

### Konfiguriere die Vorgaben für höchste Klassifizierungen

Anhand der Schlussfolgerungen aus deiner ersten Prüfung kannst du beschließen, Guardrails unverzüglich einzusetzen. Erwäge die Anwendung von Vorgaben nur für die sensibelsten Klassifizierungen. So wird die Dringlichkeit der Sicherung sensibler Daten ausgeglichen, ohne dass die große Mehrheit der Nutzer davon betroffen ist.

## Klassifizierung veröffentlichen

Bevor du automatische Klassifizierungen veröffentlichst, hast du die Möglichkeit, die Auswirkungen auf deine Nutzer zu überprüfen. Wenn du die Klassifizierungsstufen ohne Guardrails konfiguriert hast, hat das keine wesentlichen Auswirkungen auf die Nutzer, wenn du sie veröffentlichst.

[Wie man Klassifizierungen veröffentlicht](https://help.miro.com/hc/articles/16494764223378-Review-impact)

### Ankündigung der Klassifizierung

Nach der Veröffentlichung der Klassifizierungen schickst du eine Mitteilung an deine Nutzer.

Ziehe in Erwägung, die folgenden Informationen aufzunehmen:

- Ein kurzer Überblick über Enterprise Guard oder ein Verweis auf die vorherige Ankündigung
- Überblick darüber, welche Aspekte der Endnutzer-Erfahrung betroffen sein werden
- Erläuterung des Klassifizierungsrahmens deines Unternehmens
- Welche Richtlinien zur Datenregulierung werden in die Datenerkennung einbezogen?
- Zeitachse der kommenden Änderungen
- An wen du dich mit Fragen und Feedback wenden kannst

## Unnötiges Auftauchen sensibler Daten klären

Vor der Freigabe von intelligenten Vorgaben empfehlen wir, mit den Eigentümern von Boards, deren Boards sensible Informationen enthalten, zu kommunizieren. Es ist möglich, dass die sensiblen Daten unbeabsichtigt sind und entfernt werden können.

Informiere die Nutzer darüber, dass die intelligenten Vorgaben bald gemäß den Richtlinien deines Unternehmens eingeführt werden. Deine Nutzer können die Gelegenheit nutzen, um unnötige sensible Daten von ihren Boards zu entfernen und eine Unterbrechung ihrer Arbeit zu verhindern.

## Nutzer zur manuellen Klassifizierung an Bord

Auch wenn die automatische Klassifizierung aktiviert ist, bleiben viele Boards unklassifiziert oder in der Standardklassifizierung, wenn sie nicht manuell von den Nutzern neu klassifiziert werden.

### Manuelle Klassifizierung Endnutzer-Erfahrung

[Board-Eigentümer,](../../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md) [Board-Miteigentümer](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md), Bearbeitende, die Mitglieder des Teams sind, und Unternehmens-Admins mit Berechtigungen als Inhalts-Admins können das Klassifizierungslabel entweder durch Klicken auf das Badge oder in den Board-Details aktualisieren. Wähle ein neues Label aus und klicke auf Aktualisieren.

Wenn du die Klassifizierungen in der Sensibilitätsreihenfolge nach unten anpasst (z. B. von Vertraulich auf Öffentlich), müssen Nutzer eine Begründung angeben, die in den Audit-Protokollen deines Miro-Kontos angemeldet wird.

### Kommunikation mit Endnutzern

Bei der erstmaligen Einführung von Enterprise Guard wird empfohlen, die Nutzer regelmäßig zu informieren und sie aufzufordern, die Klassifizierungen auf jedem Board zu verwenden. Dadurch wird sichergestellt, dass alle Vorgaben und Klassifizierungen genutzt werden und somit die Sicherheit deiner Miro-Instanz erhöht wird.

Ziehe in Erwägung, die folgenden Informationen aufzunehmen:

- Eine Erinnerung, Boards regelmäßig zu klassifizieren
- Anleitung zur Klassifizierung von Boards
- Informationen zur Rechtfertigung
- Video | Klassifizierung von Boards für Endnutzer (Links zum Einbetten unten verfügbar)

<iframe allowfullscreen="" frameborder="0" height="315" src="//fast.wistia.com/embed/iframe/3ado2k4f6c" width="560"></iframe>
*Klassifizierung von Boards in Miro*

### Ressourcen

- Video | Board Klassifizierungen für Endnutzer
  - [Wistia Link](https://mirohq.wistia.com/medias/3ado2k4f6c)
  - Code einbetten
    - ```
      <script src="https://fast.wistia.com/embed/medias/3ado2k4f6c.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_3ado2k4f6c seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/3ado2k4f6c/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>
      ```

## Verbleibende Vorgaben einsetzen

Zu diesem Zeitpunkt sollten die Nutzer ausreichend Zeit gehabt haben, ihre Boards auf unnötige sensible Daten zu überprüfen und ihre Board-Klassifizierungen manuell anzupassen.

[Wie man intelligente Vorgaben einsetzt](../../canvas-25-admin-features/data-classification/05-define-guardrails.md)

> ⚠️ Sei vorsichtig, wenn du die Vorgaben für die Klassifizierung von Boards anwendest. Die Anwendung von Vorgaben auf die Standardklassifizierung wird erhebliche Auswirkungen auf die Nutzer haben , da viele Boards die Standardklassifizierung haben werden.

### Vorgaben Ankündigung

Nachdem du die Vorgaben veröffentlicht hast, schickst du eine Mitteilung an deine Nutzerinnen und Nutzer.

Ziehe in Erwägung, die folgenden Informationen aufzunehmen:

- Ein Hinweis auf frühere Ankündigungen zu Enterprise Guard
- Was sind Leitplanken?
- Ein Überblick über Klassifizierungen und die damit verbundenen Vorgaben
- Wie man Klassifizierungen manuell anpasst
- An wen du dich mit Fragen und Feedback wenden kannst

## Lockere die Beschränkungen für die Zusammenarbeit in der Decke

Enterprise Guard ermöglicht es dir, gezielte Kontrollen durchzuführen. Vor Enterprise Guard gab es jedoch nicht so viele Möglichkeiten, die Kontrollen auf bestimmte Fälle zuzuschneiden. Das Ergebnis waren höchstwahrscheinlich "Pauschalkontrollen" - präventiv strenge Einstellungen, die für die meisten Boards gelten und daher die Zusammenarbeit deiner Miro-Nutzer erschweren.

Pauschale Kontrollen, wie z.B. die Sperrung der externen Zusammenarbeit für alle Nutzer und Boards, sind nicht präzise genug. Für Nutzer kann es zu Reibungsverlusten kommen, wenn der Inhalt, an dem sie zusammenarbeiten, nicht sensibel ist, und es kann ganze Anwendungsbeispiele von Miro blockieren.

Alles in allem können sich pauschale Kontrollen auf den ROI von Miro auswirken, aber mit Enterprise Guard können deine Nutzer jetzt noch mehr Nutzen aus Miro ziehen und gleichzeitig sicherstellen, dass sensible Inhalte geschützt sind. Um Enterprise Guard in vollem Umfang nutzen zu können, musst du ein paar Einstellungen in deinem Konto überarbeiten.

{
Lockerung der Board-Beschränkungen

### Andere Einstellungen gegenüber Enterprise Guard

In Miro gibt es 3 Einstellungsbereiche, die zusammenarbeiten, um die tatsächliche Erfahrung des Nutzers zu bestimmen.

- Einstellungen auf Unternehmensebene
- Einstellungen auf Teamebene
- Enterprise Guard

Wenn es konkurrierende Einstellungen gibt, wird die strengste Einstellung umgesetzt. Hier findest du weitere Informationen.

### Relevante Einstellungen und wo du sie findest

Du musst ein paar Einstellungen neu bewerten, um sicherzustellen, dass Miro ganzheitlich konfiguriert ist. Hier ist eine Liste der Einstellungen, die wichtig sind und wo du sie in deinem Miro Konto findest. Einige Einstellungen können sowohl von der Unternehmens- als auch von der Teamebene aus gesteuert werden.

Denke daran: Wenn zwei Einstellungen für denselben Teil des Miro-Erlebnisses gelten, ist die strengere Einstellung ausschlaggebend für das Erlebnis.

|  |  |  |
| --- | --- | --- |
| **Einstellung** | **Beschreibung** | **Erhältlich für:** |
| Öffentliche Links | Ein öffentlicher Link ermöglicht den Zugriff auf ein Board, ohne sich anzumelden. Es kann so konfiguriert werden, dass der Zugriff angesehen, kommentiert oder bearbeitet werden kann und ein Passwort erforderlich ist. | Unternehmensebene  Teamebene  Enterprise Guard |
| Einbetten | Steuert, ob und wie Nutzer Miro-Boards in andere Software oder Websites einbetten können. | Unternehmensebene |
| Einstellungen für Gäste | Ein Gast ist ein Nutzer, der nur in ein einzelnes Board eingeladen wird und nicht in ein ganzes Team oder Konto. | Unternehmensebene  Teamebene |
| Board-Freigabe | Steuert, wie Boards für andere Nutzer im Konto, in und zwischen Teams freigegeben werden können. | Teamebene  Enterprise Guard |
