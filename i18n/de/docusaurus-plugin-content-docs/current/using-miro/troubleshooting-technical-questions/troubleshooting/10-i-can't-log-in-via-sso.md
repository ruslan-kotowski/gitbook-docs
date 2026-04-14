---
title: "Ich kann mich nicht \xFCber SSO anmelden"
article_id: 360019271654
translation_id: 360019271654
locale: de
sidebar_position: 10
created_at: '2019-03-07T15:50:03Z'
updated_at: '2025-11-25T16:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Hier erhältst du Ratschläge zur Fehlerbehebung für dich und deine IT-Admins bei Problemen im Zusammenhang mit Single Sign-On (SSO).

> **✏️** Erfahre mehr über die [Konfiguration von SSO für Miro](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) und [Miro SCIM](https://developers.miro.com/docs/scim).

## SSO-Fehlermeldungen bei Miro

Wenn du eine dieser SSO-Fehlermeldungen siehst, kannst du die folgenden Lösungen ausprobieren. Möglicherweise brauchst du die Hilfe deiner IT-Abteilung oder deines Unternehmens-Admins.

Deine E-Mail-Adresse ist mit keinem SSO-Konto verknüpft

Dies geschieht, wenn die E-Mail-Adresse, die du in Miro eingegeben hast, dich nicht als jemanden erkennt, der sich über SSO authentifizieren muss.

Mögliche Ursachen:

- **Du bist kein Mitglied eines Abos, das SSO als Anmeldevoraussetzung festgelegt hat**. Melde dich über die Standardoptionen (E-Mail und Passwort) an oder wende dich an deinen Admin, um zum Abo deines Unternehmens eingeladen zu werden.
- **Du sollst dich eigentlich über SSO anmelden, aber es gibt eine Verwechslung mit deiner E-Mail-Adresse**. Vielleicht hast du mehrere E-Mails (oder Aliase), und die Einladung zum Preisplan mit eingerichteter SSO wurde an deine andere Adresse geschickt. Melde dich mit einer anderen E-Mail-Adresse an.

Deine E-Mail-Adresse ist mit keinem SSO-Konto verknüpft. Bitte den Unternehmens-Admin um Zugriff.

Dies geschieht in der Regel in zwei Fällen:

- **Deinem Nutzer-Profil im Identitätsanbieter-System wird nicht die Erlaubnis erteilt, sich bei Miro anzumelden (dir ist keine Rolle zugewiesen)**. Wenn das der Fall ist, wirst du Miro wahrscheinlich nicht als Kachel im MyApps Dashboard deines Anbieters finden. Setz dich mit dem Admin deines Anbieters in Verbindung, um die nötigen Genehmigungen zu erhalten.
- **Du hast vor kurzem deine E-Mail** **geändert**  (z.B. aufgrund einer Heirat) und die Änderung wurde nicht in allen Systemen korrekt übernommen, wodurch Konflikte entstanden sind. Setz dich mit deinem Admin in Verbindung, um die Situation zu klären, und wenn nötig, wird er sich mit uns in Verbindung setzen, um die notwendigen Änderungen zu genehmigen.

Wenn du nicht in der Lage bist, dich über SSO bei Miro anzumelden, kannst du den Zugang bei den Unternehmens-Admins beantragen, indem du auf die entsprechende Schaltfläche auf der [Miro SSO-Anmeldeseite](https://miro.com/sso/login/) klickst.

![sso-new-sign-in.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/20463017477778_sso-new-sign-in.png)*Die Option, den Zugriff von Unternehmens-Admins anzufordern*

Du musst den Bestätigungscode eingeben, der an deine E-Mail-Adresse geschickt wurde. Sobald du den Code eingibst, wird eine Benachrichtigung an die Admins des Abos deines Unternehmens gesendet, um sie darüber zu informieren, dass du Hilfe benötigst.

Etwas ist schief gelaufen: Signatur für Antwort validieren war nicht erfolgreich

Das bedeutet, dass entweder in deinen Miro SSO-Einstellungen oder auf Seiten deines Identitätsanbieters eine Fehlkonfiguration vorliegt. Es ist wahrscheinlich, dass sich keiner deiner Kollegen anmelden kann. Bitte wende dich an deine IT-Abteilung oder den Admin des Identitätsanbieters, damit sie die folgenden Punkte überprüfen können:

- Die SAML-Antwort muss die signierte *Assertion enthalten.*. Das ist eine Voraussetzung für Miro.
- Dein Identitätsanbieter behandelt unterschriebene Antworten möglicherweise auf eine bestimmte Weise. Google SSO zum Beispiel *unsigniert* die Assertion, wenn die *Antwort* signiert wird. Wenn das der Fall ist, kannst du die Antwort abbestellen.
- Die SAML-Antwort enthält die erforderliche signierte Assertion, aber der X.509-Zertifikatswert, der sie validieren soll, ist nicht vorhanden (kann auch passieren, wenn Ihre VPN/Firewall [Teile der Datenübertragung unterbricht](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)). Stelle sicher, dass der Wert des X.509-Zertifikats im SAML-Datenverkehr an Miro weitergegeben wird.
- Die SAML-Antwort enthält eine *anderen* X.509-Zertifikatswert als der, der in den [Miro-Einstellungen](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) hinzugefügt wurde, so dass es eine Abweichung gibt und die Validierung fehlschlägt. Überprüfe, ob die Zertifikatwerte auf der IDP-Seite und auf der Miro-Seite übereinstimmen.

Etwas ist schief gelaufen: Der Nutzer wurde in der SAML-Antwort nicht angegeben

Das bedeutet, dass dein Identitätsanbieter eine falsche Konfiguration vorgenommen hat - entweder in der allgemeinen Einrichtung oder für dein spezielles Nutzerprofil. Bitte wende dich an deine IT-Abteilung oder den Admin des Identitätsanbieters, damit sie die folgenden Punkte überprüfen können.

- Das Format des Benutzernamens (NameID, Unique user ID) in deiner SSO-Konfiguration ist nicht spezifiziert oder auf ein Nicht-E-Mail-Attribut gesetzt, sodass der an Miro gesendete Wert des Nutzers nicht erkannt werden kann. Gib den Benutzernamen aufder Seite des Identitätsanbieters auf **EmailAddress**  an(oder auf ein anderes Attribut, das im E-Mail-Format vorliegt).
- Die SAML-Antwort enthält nicht den E-Mail-Wert des Nutzers, so dass der Nutzer nicht erkannt werden kann (dies kann auch passieren, wenn deine VPN/Firewall [Teile der Datenübertragung unterbricht](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)). Stelle sicher, dass die E-Mail im SAML-Datenverkehr an Miro weitergegeben wird.
- Die SAML-Antwort wird verschlüsselt. Bitte verwende keine Verschlüsselung, da Miro-Support diese nicht unterstützt.

Etwas ist schief gelaufen: SAML-Antwort ist nicht korrekt

Das passiert in der Regel, wenn es Probleme mit deinem Profil auf Seiten des Identitätsanbieters gibt.
Mögliche Ursachen:

- **Dein Nutzerprofil im Identitätsanbieter-System ist falsch konfiguriert**. Zum Beispiel hast du nicht die Erlaubnis, dich bei Miro anzumelden (du hast keine zugewiesene Rolle). Wenn das der Fall ist, wirst du Miro wahrscheinlich nicht als Kachel im MyApps Dashboard deines Anbieters finden. Setz dich mit dem Admin deines Anbieters in Verbindung, um die nötigen Genehmigungen zu erhalten.
- **Dein Nutzerprofil im System des Identitätsanbieters ist korrekt konfiguriert, aber es bestehen Einschränkungen**. Es gibt zum Beispiel IP-Beschränkungen, sodass du dich nur von bestimmten Orten aus anmelden darfst. Wende dich an den Admin deines Identitätsanbieters und frage ihn nach deinen Berechtigungen.

Um dich über SSO zu autorisieren, verwende bitte den von deinem Arbeitgeber bereitgestellten URL-Link.

Das bedeutet, dass du von dieser Seite aus nicht auf Miro zugreifen darfst oder dass die SSO-Konfiguration in deinem Miro Enterprise-Preisplan nicht vollständig ist. In diesem Fall kannst du dich möglicherweise über dein MyApps Dashboard anmelden.
Mögliche Ursachen:

- **Ihr IDP ist konfiguriert für** [IdP-vermittelte Anmeldung](https://blogs.oracle.com/dcarru/sp-vs-idp-initiated-sso) **konfiguriert, und du solltest dich nicht über die Miro-Anmeldeseite anmelden können.** Melde dich über den Link in deinem MyApps Dashboard an oder wende dich an deinen Unternehmens-Admin, um Anweisungen zu erhalten.
- **SSO ist in deinem Miro Enterprise-Preisplan aktiviert, aber die Konfiguration ist noch nicht abgeschlossen**. Setz dich mit deiner IT-Abteilung oder dem Admin deines Identitätsanbieters in Verbindung, damit sie die Konfiguration gemäß [dieser Anleitung](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) abschließen.

## Entra- oder ADFS-Fehler

Die SSO-Konfiguration ist für diese App nicht in den Enterprise-Apps verfügbar.

Der gesamte Text der Nachricht: *Die Single Sign-On-Konfiguration ist für diese App in der Enterprise-Anwendung nicht verfügbar. Miro (früher RealtimeBoard) ist eine mandantenfähige Anwendung und die App gehört einem anderen Mandanten.**Um Eigenschaften wie die Antwort-URL und Kennungen zu ändern, wende dich an den Eigentümer der App.*Wende dich an deine IT-Abteilung und bitte sie, die SSO-Konfiguration zu überprüfen. Höchstwahrscheinlich gibt es bereits eine konfigurierte Miro App in deiner Entra ID, in der unsere Kennung (`https://miro.com/)` verwendet und daher übernommen wird. Entra ist mehr oder weniger einzigartig, da dieser Identitätsanbieter verlangt, dass der Identifikator (Entity ID) eindeutig ist.
Um das Problem möglicherweise zu klären, raten wir dir, die Enterprise Apps deiner Entra-Instanz zu überprüfen und diejenige zu verwenden, die du bereits für deine Miro-Einstellungen konfiguriert hast.
Wenn du dir sicher bist, dass es keine anderen Miro Apps in deinen Enterprise Apps gibt, versuche, eine neue Kopie der Miro App aus der Entra Galerie zu bekommen.

Ein Fehler ist aufgetreten. Wende dich an deinen Admin, um weitere Informationen zu erhalten

Teile diesen Community-Beitrag mit deiner IT-Abteilung: ["Ein Fehler ist aufgetreten. Wenden Sie sich für weitere Informationen an Ihren Admins"](https://blog.kloud.com.au/2015/07/22/adfs-sign-in-error-an-error-occurred-contact-your-administrator-for-more-information/)

Zugriff verweigert: Fehler AADSTS50105

![mceclip3.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044185746_mceclip3.png)
Gib diesen Community-Artikel für deine IT-Abteilung frei: [Fehler "Rolle nicht zugewiesen"](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50105-user-not-assigned-role)

Fehlkonfigurierte App: Fehler AADSTS650056

![mceclip2.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044184722_mceclip2.png)
Wir haben die [Microsoft-Dokumentation für den Fehler AADSTS650056](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) (sowie einige [Vorschläge aus der Community](https://blogs.aaddevsup.xyz/2019/11/aadsts650056-misconfigured-application/)) geprüft und es sieht so aus, als ob der Fehler durch die Änderungen verursacht wird, die du an den App-Berechtigungen vorgenommen hast. Dein Entra-Admin muss der Miro-App möglicherweise zustimmen, damit sich die Endnutzer in Miro authentifizieren können. [Dieses Microsoft-Tutorial](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) sollte in diesem Fall hilfreich sein.

Lies [den Artikel auf support.microsoft.com über andere mögliche SSO-Fehlermeldungen](https://support.office.com/article/how-to-troubleshoot-issues-that-you-encounter-when-you-sign-in-to-office-apps-for-mac-ipad-iphone-or-ipod-touch-when-using-active-directory-federation-services-e44357b4-c9c4-4580-a946-ef5dabdb98cd?ui=en-US&rs=en-US&ad=US).

## Google SAML Fehler

In [diesem Abschnitt der Google-Dokumentation](https://support.google.com/a/answer/6301076?hl=en) findest du eine Auflistung möglicher Fehler und Anweisungen zur Behebung des Problems.

## Probleme bei der Anmeldung in der Miro-App über SSO auf der Desktop-App, dem Tablet oder dem Mobiltelefon

Wenn du dich auf einem Desktop/Tablet/Handy nicht über SSO bei der Miro-App anmelden kannst, bei der [Browserversion](https://miro.com/app/) aber schon, gehe wie folgt vor:

1. Lösche die App von deinem Gerät und installiere sie neu. Für die Desktop-App musst du alle App-Ordner entfernen, indem du die folgenden[Anweisungen](../../../getting-started/apps-for-devices/05-desktop-app.md) befolgst[:](../../../getting-started/apps-for-devices/05-desktop-app.md) . Die häufigste Ursache für dieses Problem ist ein fehlerhafter Cache, also sollte es helfen, alles zu löschen und neu zu installieren.
2. Ändere testweise den Standardbrowser deines Geräts, um zu sehen, ob du den Vorgang mit einem anderen Browser abschließen kannst. Vergewissere dich, dass dein bevorzugter Browser [Cookies von Dritten](https://akohubteam.medium.com/how-to-enable-third-party-cookies-on-your-browsers-f9a8143b8cc5) zulässt.
3. Überprüfe, ob dein Identitätsanbieter den Parameter *RelayState* eventuell **nicht** verwaltet. Dies ist ein eindeutiges Token, das Miro generiert und verwendet, um zu erkennen, dass die Person an die App zurückgesendet werden soll, anstatt auf der Browser-Seite zu bleiben. Achte darauf, dass alle Felder in deiner IdP-Konfiguration, die **RelayState** verwalten, *leer* bleiben (das Feld kann anders benannt sein, z. B. in Okta wäre das **Default RelayState**, in Google SSO - **Start URL**).
4. Wenn das Problem weiterhin besteht, kann es sein, dass dieses bestimmte Gerät keinen Zugriff auf die SSO-Umgebung des Unternehmens hat. Erkundige dich bei deiner IT-Abteilung, ob es Einschränkungen für bestimmte Geräte gibt, die SSO nutzen dürfen. Bei MDM-Lösungen kann es zum Beispiel zu Problemen kommen, wenn Miro nicht ordnungsgemäß [Zulassungsliste](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md) ist.
5. Speziell für die Miro Desktop-App - überprüfe, ob das Schema unserer App bei dir erfolgreich funktioniert und nicht kaputt ist. Dazu gibst du **miroapp://** in die Adresszeile deines bevorzugten Browsers ein und klickst darauf, um sie *als Website*  zu öffnen (drücke nicht einfach die Eingabetaste, denn dann wird stattdessen die Suche gestartet).
   ![mceclip0.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695734034_mceclip0.png)
   In diesem Moment sollst du eine ​Popup, das dich auffordert, die Miro App zu öffnen. Wenn das nicht der Fall ist, kann das Schema kaputt sein. Um zu überprüfen, ob das Schema korrekt installiert ist, befolge die Anweisungen für Windows oder Mac (dies gilt nicht für die MS Store-Version der Miro App).

   Für Windows Für Mac

   1. Geh zur [Registry Editor App](https://support.microsoft.com/windows/how-to-open-registry-editor-in-windows-10-deab38e6-91d6-e0aa-4b7c-8878d9e07b11)
   2. Drücke Strg + F und suche **miroapp.** Deine Registry sollte so aussehen: *![registry_editor_map.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057554322_registry%20editor%20map.png)*

   1. Führe den folgenden Befehl in der Terminal-App aus:

      **sudo /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/LaunchServices.framework/Versions/A/Support/lsregister -dump URLSchemeBinding | grep miroapp**

      Das Ergebnis sollte etwa so aussehen:

      ![](/attachments/token/I53o1MUemZ9TqkRlz9dQ7ndsr/?name=image.png)

Wenn es bei dir anders aussieht (der Schema-Eintrag wird beispielsweise nicht im Registry oder auf einem anderen Pfad angezeigt), versuche die App [über unsere Website](https://miro.com/apps/) neu zu installieren.

Wenn dies nicht hilft, wende dich bitte an dein IT-Team und bitte es, nach einer Lösung für das Problem zu suchen und insbesondere folgende Fragen zu klären:

- ob eigene URI-Protokolle erlaubt sind. Wenn sie blockiert sind, kann es sein, dass unser Schema bei der App-Installation nicht installiert werden kann.
- Unterliegt die Registry sonstigen Einschränkungen oder Richtlinien, die eine standardmäßige Installation verhindern oder eine andere Vorgehensweise bei der Installation erfordern?

## Meine E-Mail-Adresse hat sich geändert und ich kann mich nicht über SSO bei meinem Profil anmelden.

Wenn dein Unternehmen SSO verwendet, muss die Änderung der E-Mail-Adresse auf der Miro-Seite und auf der Seite des Identitätsanbieters vorgenommen werden, bevor ein Nutzer versucht, sich mit seinen neuen Anmeldeinformationen bei Miro anzumelden. Wenn die Änderung nicht vor der nächsten Anmeldung vorgenommen wurde, wird deine E-Mail als neuer Nutzer erkannt, und du hast möglicherweise Probleme, dich bei Miro anzumelden.

Setz dich mit deinem Admin in Verbindung, um die Situation zu klären. Du und dein Admin müssen sich eventuell an den [Miro-Support](../../tools/troubleshooting/06-contacting-miro-support.md) damit wir dein neues leeres Profil löschen und die E-Mail-Adresse des bestehenden Profils ändern können. Bitte gib die folgenden Informationen an:

- Deine neue E-Mail-Adresse und deine alte E-Mail-Adresse
- Setze den oder die Miro-Admin deiner Firma in CC und bitte ihn oder sie, uns eine Bestätigung zu schicken, dass wir die Änderung vornehmen können (dies benötigen wir aus Sicherheitsgründen).

:::note
Wenn du oben keine Lösung finden konntest, [kontaktiere den Miro-Support](https://miro.com/contact/recover/).
:::
