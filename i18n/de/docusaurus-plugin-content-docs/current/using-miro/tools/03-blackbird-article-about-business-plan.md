---
title: "Testartikel \xFCber Blackbird zu SCIM"
article_id: 25902000474898
translation_id: 25902000474898
locale: de
sidebar_position: 3
created_at: '2025-04-08T15:00:21Z'
updated_at: '2025-05-07T11:29:05Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

!!!Testartikel!!!

Das System für domainübergreifendes Identitätsmanagement (SCIM) ermöglicht es dir, das Nutzer-Provisioning und die Nutzerverwaltung zwischen Miro und deinem Identitätsanbieter (IdP) zu automatisieren.

> **Erhältlich für:**[Enterprise-Plan](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Eingerichtet von:** Unternehmens-Admins

## Wichtig zu wissen

- **SAML-basiertes SSO muss in deinem Enterprise-Preisplan ordnungsgemäß eingerichtet und funktionell sein, bevor du mit der Konfiguration der automatisierten Bereitstellung beginnen kannst.**
  Sieh dir [den Leitfaden](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) zur Konfiguration von SAML SSO an.
- **Das Synchronisieren von Gruppen mit Miro-Teams ist optional.**
  Du kannst optional deine IdP-Gruppen mit Teams in Miro synchronisieren. Um jedoch Probleme zu vermeiden, bei denen eine IdP-Gruppe versehentlich oder vorübergehend gelöscht wird, was dazu führt, dass alle Nutzer in dieser Gruppe in Miro deaktiviert werden und eine Neuzuweisung von Boards und Bereichen ausgelöst wird, synchronisiere keine IdP-Gruppen mit Miro-Teams. Teams können über die [Teams API](https://developers.miro.com/reference/enterprise-create-team) erstellt und verwaltet werden. Weitere Informationen darüber, wie die SCIM API das Verwalten von Gruppen ermöglicht, findest du unter [Miro Developers](https://developers.miro.com/docs/groups).
- **Änderungen der E-Mail-Adresse in SCIM umfassen die folgenden Validierungsregeln:**
  - **Verwalteter Benutzer-Check:** Wenn die aktuelle Domain des Nutzers nicht von der Organisation beansprucht wird, die die SCIM-Anfrage initiiert, wird die E-Mail-Aktualisierung blockiert und es wird ein Fehler 400 ausgelöst.
  - **Ziel-E-Mail-Domain-Verifizierung:** Wenn die Ziel-E-Mail-Domain von einer anderen Organisation als derjenigen beansprucht wird, die die SCIM-Anfrage initiiert, wird die E-Mail-Aktualisierung blockiert und ein 400-Fehler ausgegeben. Wenn die Ziel-E-Mail-Domain von der Organisation, die die SCIM-Anfrage initiiert, beansprucht wird, ist die E-Mail-Aktualisierung ohne E-Mail-Bestätigung möglich. Auditprotokolle zeichnen die Aktualisierungen in jeder Organisation auf, in der der Nutzer ein Mitglied ist.
  - **Domänensteuerung und SSO:** E-Mail-Updates sind erlaubt, basierend auf der Domain-Verifizierung durch Domainsteuerung (IDC) oder Single Sign-On (SSO). Falls die Ziel-E-Mail-Domain durch CD oder SSO von der initiierten Organisation verifiziert ist, kann die Aktualisierung fortgesetzt werden.
    ![scim-diagram-2.png](images/26547016509586_scim-diagram-2.png)
    *Ein Diagramm des SCIM-Arbeitsablaufs zur Validierung von E-Mail-Änderungen*

### Regeln, die Miro-SCIM zugrunde liegen

- Die mit SCIM synchronisierten Änderungen werden in erster Linie auf neu zugewiesene Nutzer angewendet. Der Status derjenigen, die bereits unter deinem Abo sind, wird ergänzt, aber möglicherweise nicht überschrieben, da die Änderungen auf Gruppen-/Teamebene vorgenommen werden. Zum Beispiel:
  a) Wenn ein Nutzer Mitglied von Team1 auf der Miro-Seite ist und dein IDP ein Update sendet, um ihn zu Team2 hinzuzufügen, bleibt sein Status in Team1 unberührt.
  b) Wenn dein IDP ein Update mit Änderungen an User1 sendet, sind die anderen Teammitglieder davon nicht betroffen. Wie unter **Unterstützte Funktionen** > **Sync und Push-Gruppen** erwähnt, kannst du den Teamstatus überschreiben und alle Nutzer auf einmal neu synchronisieren sowie einen neuen Push initiieren.
- Allen unter SCIM eingerichteten Benutzern wird die *Standardlizenz* deines Abonnements zugewiesen:
  a) Bei Enterprise-Abos ohne flexibles Lizenzmodell: eine Volllizenz. Wenn in deinem Abonnement keine Lizenzen mehr vorhanden sind, werden die Nutzer unter der [kostenlosen eingeschränkten](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) Lizenz bereitgestellt.
  b) Bei Enterprise-Abos mit aktiviertem [>flexiblen Lizenzprogramm](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md): Kostenlose oder kostenlose eingeschränkte Lizenz, abhängig von der [Standardlizenz für das Abo](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).
  *- Wenn du möchtest, dass einige Nutzer eine andere Lizenz als die Standardlizenz erhalten:*
  *Wie oben beschrieben, erhalten alle Nutzer eine Standardlizenz. Du kannst jedoch alle oder einige von ihnen sofort aktualisieren, indem du das Attribut **UserType** mit dem Wert „Full“ verwendest. <em>Nutzer, die mit dem Attribut aktualisiert wurden, werden ohne zeitliche Verzögerung auf eine Volllizenz hochgestuft.*
- Alle unter SCIM eingerichteten Benutzer sind auch von der [Domänensteuerung](../../enterprise-administration/canvas-25-admin-features/domain-control/01-domain-control.md)-Funktion betroffen. Das bedeutet, dass ein Nutzer, der in deinem Identitätsanbieter nur einer Sicherheitsgruppe angehört, aber deine Domainsteuerungseinstellungen 3 Teams als die vorgesehenen Teams festlegen, auch zu diesen 3 Teams hinzugefügt wird.
- Um den Dienst zu schützen, begrenzt Miro die Anzahl der verfügbaren API-Aufrufe alle 30 Sekunden:

  | Art der Anfrage | Limit Level |
  | --- | --- |
  | GET scim/users    GET scim/users/\{userId\} | 1. Rate Limit Level 1 |
  | POST scim/users/\{userId\}    PUT scim/users/\{userId\}    PATCH scim/users/\{userId\}    DELETE scim/users/\{userId\} | 3. Rate Limit Level 3 |
  | GET scim/Groups    PATCH scim/Groups/\{groupId\} | 4. Rate Limit Level 4 |
  | GET scim/Groups/\{groupId\} | 3. Rate Limit Level 4 |

  Einzelheiten zu den Limit Level findest du [**hier.**](https://developers.miro.com/reference#ratelimiting)Wenn die Anzahl der Anfragen das Limit überschreitet, gibt Miro die Standardmeldung **429 zu viele Anfragen** zurück.

## Unterstützte Funktionen

Das detaillierte Miro SCIM-Schema findest du [**hier**](https://developers.miro.com/docs/scim).

Miro unterstützt die folgenden Bereitstellungsfunktionen:

- **Neue Nutzer anlegen**
  Neue Nutzer, die der Miro-Anwendung im IdP zugewiesen werden, werden in deinem Miro Enterprise-Abo als Enterprise-Mitglieder erstellt. <span>Nutzer, die zu einer Nutzergruppe hinzugefügt werden, die mit einem Miro-Team mit demselben Namen synchronisiert ist, werden dem Team als Teammitglieder hinzugefügt
- **Aktualisierungen des Nutzerprofils pushen**
  Siehe unten für die unterstützten Attribute und Änderungen
- **Gruppen synchronisieren und pushen**
  Synchronisiere deine IDP-Gruppen und deren Mitglieder mit den Teams innerhalb deines Miro Enterprise-Abos, um die Nutzer-Mitgliedschaft automatisch zu verwalten. Bei einer laufenden Synchronisierung werden bestimmte Aktualisierungen bezüglich der Nutzer deiner Gruppe an das synchronisierte Miro-Team gesendet, während ein Push den Status des Teams überschreibt, wobei die Gruppe als Quelle der Wahrheit behandelt wird (falls es manuelle Änderungen durch deine Unternehmens-Admins auf der Miro-Seite gab)
- **Namen der Gruppe/des Teams entkoppeln**
  Miro synchronisiert Gruppen und Teams nach ihrem Namen, daher müssen sie exakt denselben Namen haben. Nach der ersten Synchronisierung kannst du jedoch einem oder sogar beiden einen Namen geben, der dir am besten passt. Ein Beispiel für die Entkopplung findest du [hier](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).
- **Nutzer aus Gruppe/Team entfernen (nicht aus dem Enterprise-Abo, siehe unten)**
  Wenn du einen Nutzer aus einer Gruppe entfernst, wird er aus dem synchronisierten Miro-Team entfernt (beim nächsten Gruppen-Push).
- **Nutzer deaktivieren**
  Das Deaktivieren/Löschen eines Nutzers oder das Deaktivieren des Zugriffs eines Nutzers auf die Anwendung im IDP wird *den Nutzer deaktivieren* in deinem Miro Enterprise-Plan.</span> Je nach den Umständen kann die Deaktivierung eines Nutzers dazu führen, dass seine Inhalte den ältesten Team-Admins zugewiesen werden:
  - Wenn du den Nutzer auf der IDP-Seite deaktivierst, ihn aber weiterhin der Miro-App zuordnest, wird seine Team-Mitgliedschaft auf der Miro-Seite nicht geändert und seine Inhalte werden nicht neu zugewiesen - er wird einfach von einem **aktiven** in einen **deaktivierten** Status (bzw. in den entsprechenden Nutzerbereich) verschoben und verbraucht keine Lizenz mehr.
  – Wenn du die Deaktivierung auslöst, indem du den Benutzer im IDP löschst oder ihm die Zuweisung der Miro-App entziehst, während der Benutzer Mitglied einiger *synchronisierter* Teams ist, wird der Benutzer zusätzlich aus *diesen* Miro-Teams entfernt und seine Inhalte in den genannten Teams werden den ältesten Team-Admins neu zugewiesen.
  - Wenn du die Deaktivierung auslöst, indem du den Nutzer im IDP *löschst* oder ihm die Zuweisung zur Miro-App *entziehst*, wird die Team-Mitgliedschaft des Nutzers nicht geändert und seine Inhalte werden nicht neu zugewiesen, wenn er kein Mitglied eines *synchronisierten* Teams ist.
  **Das Entfernen eines Nutzers** aus dem Enterprise-Abo wird standardmäßig *nicht unterstützt.* Dennoch kannst du [die Funktionalität mit der API manuell hinzufügen](https://developers.miro.com/docs/scim#section-delete-user-by-id), um den Benutzer vollständig aus dem Abonnement zu entfernen, anstatt ihn auf den Status **Deaktiviert** zu setzen. In diesem Szenario werden die Inhalte den jeweiligen Team-Mitgliedern neu zugewiesen. Es ist nicht möglich, festzulegen, welche Admins das Eigentum an automatisch neu zugewiesenen Inhalten erhalten. Aber das kann eingestellt werden, wenn du einen Nutzer in den Miro-Einstellungen manuell [deaktivierst.](../../enterprise-administration/user-management/01-deactivated-users.md)
- **Nutzer reaktivieren**
  Die erneute Zuweisung eines Nutzers zur Anwendung oder die Reaktivierung des Nutzerprofils im IDP reaktiviert den Nutzer in deinem Miro Enterprise-Abo, wenn er zuvor bereitgestellt und deaktiviert wurde.
- **Die Zuordnung zu Abrechnungsgruppen automatisieren**
  Neue Nutzer automatisch [billing groups](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/01-billing-groups.md) mittels SCIM zuweisen. Sobald dein Identitätsanbieter (IdP) eingerichtet ist, verknüpfst du deine Kostenstellen mit deinen Abrechnungsgruppen. Dadurch wird sichergestellt, dass jeder aktuelle und zukünftige Nutzer aus diesen Kostenstellen automatisch in die richtige Abrechnungskategorie einsortiert wird.

Du kannst Nutzer auch aus deinem Enterprise-Plan entfernen, indem du einen direkten **Löschen**-API-Aufruf sendest – siehe die Dokumentation [hier](https://developers.miro.com/docs/scim#section-delete-user-by-id). Beachte, dass nur *direkte* Anrufe die Nutzer entfernen werden. **Löschvorgänge**, die *von deiner Identitätslösung* initiiert werden, werden als Anfrage zur **Deaktivierung** behandelt.

### Unterstützte Attribute

:::warning
Beachte Folgendes:
- **E-Mail** / Der primäre Parameter / Eindeutige Kennung / **Benutzername**) ist der einzige Wert, der von Miro benötigt wird und muss in Form einer E-Mail-Adresse vorliegen.
- Die Aktualisierung der E-Mail-Adresse ist nur für bereits synchronisierte Nutzer möglich. <span>Mit anderen Worten, die erste Synchronisierung muss erfolgen, wenn ihre E-Mail-Adresse im IdP und Miro die gleiche ist, andernfalls erkennt Miro die Person nicht und es wird ein doppeltes Miro-Profil unter der neuen E-Mail-Adresse erstellt.
- Die Aktualisierung der E-Mail-Adresse muss im Identitätsanbieter-Profil des Nutzers erfolgen, nicht in der Zuweisungsliste.
- Anders als bei anderen Attributen wird bei der Aktualisierung der **E-Mail-Adresse** der Person eine Benachrichtigung gesendet: Sowohl die alte als auch die neue E-Mail-Adresse erhalten einen Hinweis darüber, dass der Nutzer sich künftig mit der neuen E-Mail-Adresse bei Miro anmelden soll.
:::

| Name des Attributs | SCIM-Attribut (Anspruch) |
| --- | --- |
| E-Mail | Benutzername.  **Muss vorhanden und im E-Mail-Format sein** |
| *Die unten aufgeführten Attribute sind nicht erforderlich und werden von Miro akzeptiert, wenn sie vorhanden sind (andere an Miro gesendete Attribute werden ignoriert).* | |
| Name und Vorname | displayName;      formatiert;      givenName + " " + familyName;      userName |
| Nutzertyp | userType       unterstützter Wert: „Voll“ |
| Aktiv | aktiv  unterstützter Wert: „wahr“ oder „falsch“ |
| Profilbild | **photos.^[type=='photo'].value** oder     **photos.^[type==photo].value** (Okta)     **photos[type eq "photo"].value** (Entra)        Muss eine Text-URL zum Bild sein.  Unterstützte Dateitypen: jpg, jpeg, bmp, png, gif  Um den Dateityp zu definieren, solltest du die Dateierweiterung in der URL angeben (z. B. `https://host.com/avatar_user1.jpg`) oder die Anfrage an die URL sollte zusammen mit dem Dateiinhalt einen Header Content-Type zurückgeben (z. B. Content-Type = 'image/jpeg')  Die maximale Dateigröße zum Herunterladen ist: 31457280 Bytes |
| Nutzerrolle | roles.^[primary==true].value (Okta)      roles[primary eq "True"].value (Eintritt)        unterstützte Werte:  **ORGANISATION_INTERNER_ADMIN** **ORGANISATION_INTERNE_NUTZER** |
| Mitarbeiternummer | Mitarbeiternummer |
| Kostenstelle | costCenter |
| Organisation | Organisation |
| Bereich | Bereich |
| Abteilung | Abteilung |
| Managername | manager.displayName |
| Manager-ID | manager.value  Das Feld "Value" hat im SCIM-Standard den Typ "String", aber managerId  Das interne Miro-Feld hat den Typ "Long". Wenn das Attribut „Value“ kein      Zahlenwert ignorieren wir diesen |

:::warning
Passwortänderungen werden nicht unterstützt und es gibt keine unmittelbaren Pläne, diese Änderung zu unterstützen.
⚠️ **Username**, **UserType** und **roles.value** können für [deaktivierte Nutzer](../../enterprise-administration/user-management/01-deactivated-users.md) nicht aktualisiert werden.
:::

Alle Attribute werden in der exportierten CSV-Nutzerliste angezeigt, die im [Abschnitt Aktive Nutzer](../../enterprise-administration/user-management/12-user-management-overview-on-enterprise-plan.md) heruntergeladen werden kann.

![download_as_CSV_in_company_settings.jpg](images/26547058752786_download%20as%20CSV%20in%20company%20settings.jpg)
*Die Option, eine Liste der Nutzer herunterzuladen*

![mceclip3.png](images/26547058758802_mceclip3.png)

## Konfiguration von SCIM

### Schritt 1: Aktiviere die SCIM-Option in Miro

Um SCIM für deinen Miro Enterprise-Plan zu aktivieren, gehe zu den **Unternehmenseinstellungen** > **Enterprise-Integrationen,** und aktiviere die Funktion SCIM-Provisioning**.</strong>** Dort erhältst du die Basis-URL und das API-Token zur Konfiguration deines IdP.

![scim.png](images/26547058760466_scim.png)
*SCIM in den Miro-Einstellungen*

### Schritt 2: Konfiguriere deinen Identitätsanbieter

Die Einrichtung hängt von dem Identitätsanbieter ab, den du verwendest. Miro unterstützt vorkonfiguriertes Okta und Entra ID, du kannst jedoch jeden Identitätsanbieter deiner Wahl verwenden, solange er die Einrichtung von SCIM ermöglicht.

OKTA: Die Anleitung zur Einrichtung findest du [hier](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md).

Entra ID – die Anleitung zur Einrichtung findest du [hier](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).

## Neues Token generieren

1. Gehe zu den **Unternehmenseinstellungen** > **Enterprise-Integrationen.**

2. Klicke im **SCIM-Provisioning**-Abschnitt auf **Neues Token generieren**.

![scim.png](images/26547058760466_scim.png)
*SCIM in den Miro-Einstellungen*

2. Klicke im Fenster **Neues SCIM-Token generieren** auf **Generieren**.

![generate_token.png](images/26547016527122_generate_token.png)

3. Nachdem du ein neues Token erstellt hast, musst du das neue Token in deinem Identitätsanbieter konfigurieren.

## Mögliche Probleme und wie man sie löst

*1. <em>Nutzer werden aufgrund eines Fehlers in der Zulassungsliste nicht bereitgestellt.*
![mceclip0.png](images/26547016528530_mceclip0.png)
*Ein Beispiel für eine Fehlermeldung des Identitätsanbieters Okta*

Bitte stelle sicher, dass die Domainadresse des Nutzers zu deiner Zulassungsliste [in den **Sicherheitseinstellungen**](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md) hinzugefügt wurde.

*2. Wenn du deine Endnutzer mit einer Identitätslösung (IDP1) authentifizierst, SCIM aber über eine andere Lösung (IDP2) aktivieren möchtest, ist dies unter zwei Bedingungen möglich:*

1. Der IDP2 kann API-Aufrufe mit dem Bearer-Token durchführen.
2. Beide Identitätsanbieter sind synchronisiert (d. h. SCIM-Nutzer sind auch im IDP1 vorhanden und können sich daher bei Miro authentifizieren).

Für weitere Informationen wende dich bitte [an das Miro-Support-Team](https://help.miro.com/hc/en-us/requests/new?referer=help-center-article).
