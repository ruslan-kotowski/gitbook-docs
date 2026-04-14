---
title: Intégrer un tableau Miro
article_id: 360016335640
translation_id: 360016335640
locale: fr
sidebar_position: 2
created_at: '2020-09-09T07:54:13Z'
updated_at: '2025-09-19T09:07:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: comments
availability:
  notes: 'Personnes : Éditeurs du tableau Forfaits : Tous les forfaits Plateformes
    : Web, Bureau, Mobile'
---

Vous pouvez intégrer n'importe quel tableau Miro ou un élément spécifique (cadre ou format) du tableau dans les applications et sites web pris en charge, afin que vos coéquipiers puissent travailler dans leur contexte sans changer d'outils.

Les intégrations héritent des [paramètres de partage](../../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) du tableau :

- **Lien public activé** — toute personne ayant le lien peut consulter (ou, sur les forfaits payants et Education, commenter ou modifier).
- **Lien public désactivé** — seuls les collaborateurs invités peuvent ouvrir l'intégration après s'être connectés.

Les [administrateurs Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md) peuvent gérer la disponibilité du lien public dans les [paramètres de sécurité](../../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

## Choisissez votre méthode d'intégration

Miro propose deux méthodes pour intégrer des tableaux :

- **En utilisant des applications prises en charge** :

  - Travailler sur des plateformes comme Zoom, Teams, Confluence, Jira ou Notion.
  - Vous souhaitez des fonctionnalités d'intégration natives et un workflow fluide.
  - Les utilisateurs interagiront principalement via cette plateforme spécifique.
  - Vous avez besoin du processus de configuration le plus simple.
- **En utilisant du code d'intégration** :

  - Intégrer dans des sites web, blogs ou plateformes personnalisées.
  - Travailler avec WordPress, Webflow, ou d'autres créateurs de sites web.
  - Vous avez besoin de plus de contrôle sur la taille et l'apparence.
  - La plateforme prend en charge les iFrames mais n'a pas d'intégration native avec Miro.

## Intégrer un tableau dans des applications prises en charge

Miro est pris en charge par plusieurs applications dans lesquelles vous pouvez facilement partager vos tableaux. Les applications prises en charge incluent :

- [Zoom](../../../integrations-apps/zoom/02-miro-app-for-zoom-user-guide.md)
- [Webex](../../../integrations-apps/more-integrations/10-miro-for-webex.md)
- [Microsoft Teams](../../../integrations-apps/microsoft/microsoft-teams/02-miro-for-microsoft-teams-user-guide.md)
- [Jira](../../../integrations-apps/atlassian/02-miro-for-jira-cloud.md)
- [Confluence](../../../integrations-apps/atlassian/01-miro-for-confluence.md)
- [Notion](https://miro.com/marketplace/notion-embed/)
- [Coda](https://miro.com/marketplace/coda-embed/)
- [Productboard](https://miro.com/marketplace/productboard-embed/)
- Moyenne

Lorsque vous intégrez un tableau Miro dans une autre application, vous pouvez définir les droits d’accès spécifiques aux utilisateurs de l’application et leur permettre de consulter, commenter ou modifier le tableau à partir de l’application. L’accès au tableau du côté Miro ne sera pas affecté. Découvrez comment [fonctionnent le partage et les autorisations pour les tableaux intégrés](../../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).

Pour intégrer un tableau dans l’une des applications supportées :

1. Dans l'application cible, tapez **/miro** ou choisissez **Miro** dans le menu d'insertion.
2. Sélectionnez le tableau.
3. Sélectionnez la **Vue de départ** :
   - **Canevas complet** — l'ensemble du canevas.
   - **Élément spécifique**, tel qu'un cadre ou un format (Document, Diagramme, Table, Planning ou Diapositives).
4. Activez le **mode immersif** pour une intégration sans distractions. Laissez-le désactivé pour permettre une interaction complète.
5. Sélectionnez les **paramètres d'accès** pour tous les visiteurs :
   - **Peut consulter** — toute personne visionnant l'intégration peut voir le tableau.
   - **Nécessite un accès** — toute personne visionnant l'intégration doit avoir l'accès pour consulter, commenter ou modifier le tableau.
6. Sélectionnez **Intégrer le tableau**.

L'intégration respecte les paramètres de partage du tableau. Sur les appareils mobiles, toutes les intégrations sont en lecture seule.

## Intégrer un tableau avec un code d'intégration

Utilisez cette option pour toute plateforme qui prend en charge iFrame, comme **WordPress** ou **Webflow**.

1. Ouvrez le panneau **Partager** en utilisant l'une des méthodes suivantes :
   - Dans le coin supérieur droit, sélectionnez **Partager** > **Intégrer**, ou
   - Dans le menu principal du tableau, sélectionnez **Tableau** > **Exporter** > **Intégrer**, ou
   - Sur le canevas, sélectionnez l'élément que vous souhaitez intégrer (cadre ou format). Par exemple, un Doc. Ouvrez le menu contextuel à trois points, et sélectionnez **Intégrer ce doc**.
2. Sélectionnez la **vue de départ** :
   - **Tableau** — l'ensemble du canevas.
   - **Élément spécifique**, tel que cadre ou format (Doc, Diagramme, Table, Chronologie, ou Diapositives).
3. (Optionnel) **Définir la zone de départ** — déplacez pour délimiter une région précise du tableau.
4. Décider de l'interaction :
   - Sélectionnez **Visualisation uniquement** pour verrouiller la vue.
   - Décochez **Visualisation uniquement** pour permettre aux lecteurs de naviguer, de zoomer, de commenter ou de modifier (s'ils ont l'autorisation).
5. Sélectionnez **Copier le code** et collez-le où vous en avez besoin.
   Si la destination n'accepte que les URL, sélectionnez **Copier le lien** à la place.

Vous pouvez créer plusieurs intégrations pour le même tableau, chacune avec sa propre vue de départ, sa propre zone de départ ou son propre objet de focalisation.

### Lecture automatique des diapositives

Pour lire automatiquement une intégration de Diapositives, réglez l'intervalle de **Diapositive automatique** de 1 à 30 secondes dans l'onglet **Intégrer**. La lecture automatique est ignorée lorsque vous intégrez un tableau dans un autre tableau.

## Comment les intégrations apparaissent

- Le nom du tableau n'est pas cliquable.
- La mini-carte, [les notes](../../essential-tools/17-visual-notes.md) et les pop-ups sont fermés par défaut.
- Certaines options de menu, telles que **Définir la vue de départ**, sont masquées.
- Tous les intégrations sont en lecture seule sur mobile.
- Les bloqueurs de cookies tiers peuvent empêcher le chargement correct des intégrations.

## Foire aux questions

**Quelle est la différence entre une vue de départ et le mode immersif ?**
Une vue de départ définit la position initiale, mais les lecteurs peuvent toujours explorer le tableau. Le mode immersif masque tout sauf l'objet sélectionné et est toujours en lecture seule.

**Puis-je rendre une intégration en mode immersif modifiable ?**
Non. Pour activer la collaboration, désactivez **Lecture seule** et accordez les droits de modification dans les paramètres de partage du tableau.

**Quels widgets sont pris en charge ?**
Documents, Diagrammes, Tables, Plannings, Diapositives et tout cadre.

**Puis-je supprimer le logo Miro ?**
Non. La suppression du logo n'est pas disponible.

**Puis-je intégrer un tableau dans un autre tableau ?**
Oui. Copiez le code d'intégration et collez-le dans le tableau cible avec **Coller le code iFrame**.
