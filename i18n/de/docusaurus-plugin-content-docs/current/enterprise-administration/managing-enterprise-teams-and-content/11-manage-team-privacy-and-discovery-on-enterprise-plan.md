---
title: Team-Datenschutz und -Auffindbarkeit im Enterprise-Plan verwalten
article_id: 360011821219
translation_id: 360011821219
locale: de
sidebar_position: 12
created_at: '2020-02-07T12:46:14Z'
updated_at: '2025-12-10T12:23:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: sharing-settings
availability:
  notes: 'Erhältlich für: Enterprise-Preisplan Erforderliche Rolle: Unternehmens-Admin'
---

Wer in großen Unternehmen arbeitet, weiß, dass Inhalte und Nutzer über zahlreiche Teams verteilt sind. Stelle sicher, dass alle Zugriff auf die benötigten Daten haben, indem du Abo-Mitgliedern das Recht gibst, relevante Teams zu sehen und ihnen beizutreten.

### Finden von Teams

**Finden von Teams ist eine Einstellung für Teams, die festlegt, wie Organisationsmitglieder das Team finden und ihm beitreten können.** Um die Erkennungseinstellungen für ein Team zu verwalten, gehst du zu **Unternehmenseinstellungen > Teams** und klickst dann auf das Team, für das du die Einstellungen ändern möchtest. Wähle dann den Tab " **Einstellungen"**.

![team-management-list.png](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921803038994_team-management-list.png) *Liste der Teams in den Einstellungen des Unternehmens*

> [⚠️](../../administration/user-management/02-invitation-settings.md)Das Finden von Teams kann von Unternehmens-Admins und Team-Admins eingerichtet werden, sofern die Team-Admins Nutzer zum Team einladen dürfen (sie erhalten Beitrittsanfragen von den Nutzern).

Team-Auffindbarkeit erfolgt auf drei Ebenen:

- **Ausgeblendet** – Mitglieder können das Team nur finden, wenn sie eingeladen wurden
- Mitglieder können nach Genehmigung beitreten – das Team ist sichtbar und Mitglieder können eine Beitrittsanfrage stellen
- **Für Mitglieder offen** – Das Team ist sichtbar und Mitglieder können ihm umgehend beitreten

Wenn ein Team über [Domain-Zulassungsliste Einschränkungen](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)hat, können nur Nutzer, deren E-Mail Domänen auf der Zulassungsliste des Teams stehen, das Team entdecken und eine Anfrage stellen, um dem Team beizutreten. Mit dieser Einstellung wird sichergestellt, dass die Auffindbarkeit des Teams den auf Teamebene festgelegten Domain-Einschränkungen folgt.

>  Aktiviere unsere Funktion zum Finden von Teams zusammen mit der [Just-in-Time-Bereitstellung](../user-management/13-user-provisioning-on-enterprise-plan.md)). Das Standardteam, das du für neu registrierte Personen festgelegt hast, ist auch für Personen sichtbar, die bereits Miro nutzen. Auch sie können diesen Teams beitreten.

![team-management-disiscovery-settings.png](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921780537234_team-management-discovery-settings.png)
*Einstellungen für das Finden von Teams*

Das Finden von Teams hat keinen Einfluss darauf, wie Mitglieder andere Nutzer im Abo sehen.  Die Mitglieder können also die gesamte Liste anderer Nutzer in den Einstellungen sehen, es sei denn, dies wurde im Vertraulichkeitsschutz für Teams außer Kraft gesetzt./span>

Mitglieder deines Enterprise-Preisplans können Teams finden, denen sie beitreten können, indem sie das Menü Teams oben links auf dem Dashboard öffnen und ![icon-zoom-in.svg](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921803048338_icon-zoom-in.svg) **Team beitreten**auswählen. Es wird eine Liste mit Teams angezeigt, in der du je nach den Sicherheitseinstellungen des jeweiligen Teams die Option **"Beitreten"** oder " **Beitrittsanfrage"** auswählen kannst.

![team-management-join.png](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921780544914_team-management-join.png) *Liste der auffindbaren Teams*

### Datenschutzeinstellungen für Teams

**Vertraulichkeitsschutz für Teams** ist eine Funktion auf Unternehmensebene, die die Sichtbarkeit von Teams wie auch Nutzern bestimmt. Du findest sie in den **Unternehmenseinstellungen** > **Sicherheit** > **Freigabe,** im Abschnitt **Vertraulichkeitsschutz für Teams**.

![team-management-privacy.pngDatenschutzeinstellungen für Teams](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921780547218_team-management-privacy.png)

- Wenn der Vertraulichkeitsschutz für Teams deaktiviert wurde, können Abo-Mitglieder in den Einstellungen die gesamte Liste der Nutzer und die Liste der auffindbaren Teams einsehen.  Das ist die Standardeinstellung im Enterprise-Preisplan, damit alle Mitglieder die passenden Inhalte finden und mit anderen zusammenarbeiten können, um einen Wissensaustausch und Transparenz zu fördern und die Duplizierung von Aufgaben zu reduzieren./span>
- Sofern der Team-Datenschutz aktiviert ist, können Abo-Mitglieder nur die Teams sehen, zu denen sie eingeladen wurden, sowie die Mitglieder dieser Teams.  Der Datenschutz kann bei der Arbeit mit verschiedenen Kunden in separaten Teams verwendet werden, um sicherzustellen, dass die Gruppen nichts übereinander erfahren. Bei aktiviertem Team-Datenschutz ist es nicht möglich, Boards per Klick mit dem gesamten Unternehmen zu teilen./span>

### Gleichzeitige Funktion von Team-Datenschutz und Team-Auffindbarkeit

Team-Datenschutz hat eine höhere Priorität als die Auffindbarkeit auf Teamebene. Du siehst eine Benachrichtigung, dass die Team-Auffindbarkeitseinstellungen nicht funktionieren. Die Optionen können weiterhin verwaltet werden und gelten, sobald der Team-Datenschutz deaktiviert wurde.

> [✏️](../user-management/13-user-provisioning-on-enterprise-plan.md) Die Einstellungen für Team-Datenschutz und Team-Auffindbarkeit wirken sich auf das Erlebnis der Abo-Mitglieder aus, haben allerdings keinen Einfluss auf die Art des Beitritts zum Abo.
