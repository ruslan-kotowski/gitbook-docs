---
title: Profilsperre
article_id: 360017571374
translation_id: 360017571374
locale: de
sidebar_position: 14
created_at: '2019-02-11T10:08:55Z'
updated_at: '2026-02-24T12:02:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Die Profilsperre ist füralle Miro-Nutzer und Preispläne standardmäßig aktiviert und kann nicht angepasst werden. Nutzer, die sich [über externe Identitätsanbieter authentifizieren](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), sind von dieser Funktion nicht betroffen.

Nach einer falschen Anmeldung bei deinem Profil hast du **10 Versuche**, um ein korrektes Passwort zu deiner E-Mail-Adresse einzugeben. Die ersten 5 Versuche erfolgen als standardmäßige Anmeldung ohne zusätzliche Komplexität.

Bei den nächsten Versuchen musst du ein Captcha lösen (nur in den Web- und Desktop-Apps). Wenn du **10 Mal hintereinander** ein falsches Passwort für deine E-Mail-Adresse eingibst, wird dein Nutzerprofil für**1 Stunde** gesperrt, in der alle Anmeldeversuche fehlschlagen, selbst wenn ein korrektes Passwort eingegeben wird.

:::tip
Während der Sperrstunde kannst du versuchen, dich mit Passwortlos- oder sozialen Anbietern anzumelden.
:::

Wenn dein Nutzerprofil gesperrt wurde, sendet Miro dir eine E-Mail mit einem sechsstelligen Code, um dein Profil zu entsperren. Der Link in der E-Mail leitet dich auf die Bestätigungsseite weiter, auf der du den sechsstelligen Code eingeben musst. Wenn der eingegebene Code korrekt ist, wird dein Profil freigeschaltet und alle Versuche zurückgesetzt. In der E-Mail wird dir außerdem empfohlen, dein Passwort zu ändern.

Das gesperrte Profil wird **automatisch** nach 1 Stunde freigeschaltet und alle fehlgeschlagenen Versuche zurückgesetzt.

### So gehst du vor, wenn du keinen Code erhalten hast

Wenn du die E-Mail in deinem Posteingang nicht findest, probiere folgende Schritte zur Fehlerbehebung:

- Vergewissere dich, dass in der von dir angegebenen E-Mail-Adresse keine Tippfehler vorhanden sind. Wenn du einen Tippfehler findest, versuche, dich mit der richtigen E-Mail-Adresse anzumelden.
- Öffne deine **Spam-, Werbe-, Junk-, Social**- und **Update**-Ordner und sieh nach, ob die Bestätigungs-E-Mail von Miro dort gelandet ist.
- Überprüfe, ob dein Posteingang voll ist, um sicherzustellen, dass du das Speicherlimit für deinen E-Mail-Posteingang nicht erreicht hast. Wenn er voll ist, musst du eventuell einige bestehende E-Mails löschen, um neue zu erhalten. Nachdem du die E-Mails gelöscht hast, klicke auf **Code erneut senden**, um eine Registrierungs-E-Mail zu erhalten.
- Es kann sein, dass eine Firewall verhindert, dass die E-Mail deinen Posteingang erreicht. Bitte deinen *Admin*, unsere Domains und Subdomains auf die Zulassungsliste zu setzen: [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) und [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/). [Hier ist ein Artikel](../../tools/troubleshooting/02-allowlist-miro-mailers.md) mit weiteren Informationen zu den Mailern, die du auf die Zulassungsliste setzen musst
- AOL/CompuServe-Nutzer: Vergewissere dich, dass deine E-Mail-Kontrollen so eingestellt sind, dass du E-Mails über das Internet empfangen kannst. Wenn du E-Mails aus dem Internet blockiert hast, ändere deine E-Mail-Kontrollen, indem du in AOL oder CompuServe **Mail Controls** eingibst. Kehre danach zu unserem Registrierungsformular zurück, um deinen Bestätigungscode erneut zu senden.
- Normalerweise sollte der Code sofort ankommen, doch je nach den besonderen Eigenschaften deines E-Mail-Systems musst du möglicherweise bis zu 24 Stunden warten.
- Wenn keine der Lösungen hilft, [melde das Problem an den Miro Support](../../tools/troubleshooting/06-contacting-miro-support.md).
