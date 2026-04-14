---
title: 'Guide de déploiement d''Enterprise Guard, partie 2 : Déployer la sécurité
  des données'
article_id: 17121026396690
translation_id: 17121026396690
locale: fr
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
  notes: 'Équipes concernées: Les équipes avec lesquelles vous devrez peut-être vous
    associer pour déployer les fonctionnalités de sécurité des données sont par exemple
    la protection des données, la prévention de la perte de données, la gouvernance
    et le risque, la sécurité des applications, l''information et la sécurité numériques,
    et/ou les menaces d''initiés.'
---

## Aperçu de la sécurité des données

Recherchez, classez et sécurisez les contenus sensibles à l'aide des fonctions de sécurité des données d'Enterprise Guard.

- **Découverte de données :** Découvrez les données sensibles telles que les informations personnelles identifiables (PII), les informations personnelles de santé (PHI) et les données de l'industrie des cartes de paiement (PCI) en quelques clics.
- **Classification automatique :** Définissez des critères permettant à Miro de classer automatiquement vos tableaux en fonction du contenu sensible qui s’y trouve.
- **Garde-fous intelligents :** Appliquez des règles de sécurité en temps réel et limitez ce que les utilisateurs peuvent faire avec un tableau en fonction de sa classification manuelle ou automatisée.
- **Explorateur de contenu :** Obtenez une vue unifiée de tous les tableaux Miro à contenu sensible et de la classification de chaque tableau.

![Enterprise Guard-Sécurité des données.png](images/21016928916242_Enterprise-Guard-Data-Security.png)*Trouvez, classez et sécurisez les données sensibles*

## Vue d'ensemble du déploiement

Cette approche de déploiement donne la priorité à la sécurisation des données sensibles trouvées par la découverte de données d'Enterprise Guard tout en minimisant la perturbation de l'activité de l'utilisateur final.

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="390" scrolling="no" src="https://miro.com/app/live-embed/uXjVNrjv8h8=/?moveToViewport=-3966,-1331,10269,3273&amp;embedId=881755370090" width="690"></iframe> *Vue d'ensemble du déploiement d'Enterprise Guard*

#### Étapes de configuration

1. Audit des données sensibles
2. Configurer la classification
3. Publier la classification
4. Déployer des garde-fous
5. Assouplir les restrictions générales

#### Communication avec l'utilisateur final et étapes d'habilitation

1. Créer un plan de déploiement
2. Annonce initiale de l'Enterprise Guard
3. Annonce du déploiement des classifications
4. Résoudre les occurrences inutiles de données sensibles
5. Annonce du déploiement des garde-fous

## Audit des données sensibles

Effectuez l'audit décrit dans cette section le plus tôt possible dans le déploiement d'Enterprise Guard. Elle n'a aucun impact sur les utilisateurs finaux, mais vous permettra d'évaluer la portée et la gravité des occurrences de données sensibles dans votre instance Miro.

Utilisez les résultats de l'audit pour créer un plan de déploiement qui concilie la gestion des changements pour l'utilisateur final et les politiques de sécurité de votre organisation.

### Activer la découverte de données

La première étape de la configuration de votre cadre de classification des données consiste à activer la découverte de données dans votre compte Miro. Miro analysera ensuite tous vos tableaux à la recherche de données sensibles en fonction de la région et/ou des politiques de confidentialité (labels) activées.

[Comment activer la découverte de données dans votre environnement Miro ?](../../canvas-25-admin-features/data-discovery/13-activate-privacy-related-data-discovery.md)

La détection des contenus sensibles peut prendre jusqu'à 24 heures. Une fois que Miro a identifié le contenu sensible correspondant à ces étiquettes de sensibilité (c'est-à-dire GDPR, PCI), l'explorateur de contenu peut être utilisé pour examiner les résultats plus en détail.

### Audit avec l'explorateur de contenu

Content Explorer permet aux administrateurs de contenu sensible d'examiner les occurrences de données sensibles découvertes par Miro Enterprise Guard, en révélant où les occurrences ont eu lieu (nom du tableau), qui est l'acteur (propriétaire du tableau), pourquoi l'occurrence a été signalée (étiquette) et quel en est le contenu.

Utilisez les filtres de l'explorateur de contenu, tels que "Classification = Confidentiel", pour vous concentrer sur les occurrences les plus importantes de données sensibles.

## Créer un plan de déploiement

Une fois que la découverte de données est activée et que les occurrences de contenu sensible sont révélées, il est temps de créer un plan de déploiement pour les classifications et les garde-fous en fonction des politiques de votre organisation, des exigences, de la gravité des résultats et de vos ressources disponibles. Les sections ci-dessous proposent des bonnes pratiques de communication pour informer les utilisateurs finaux et soutenir votre processus de gestion du changement.

### Annoncez les changements à venir

Avant de publier votre cadre de classification dans Miro, il est recommandé d'informer les utilisateurs de la décision de votre organisation d'activer Enterprise Guard pour l'ensemble du contenu Miro, et de fournir un contexte conforme aux politiques et pratiques de votre organisation en matière de sécurité des données.

Pensez à inclure les informations suivantes :

- Qu'est-ce qu'Enterprise Guard ?
- Pourquoi c'est important pour votre organisation
- Aperçu des aspects de l'expérience de l'utilisateur final qui seront affectés
- Explication du cadre de classification de votre organisation
- Quelles politiques de réglementation des données seront incluses dans la découverte des données ?
- Planning des changements à venir
- Où poser vos questions et demander un retour d'information ?

## Configurer la classification

### Ajouter un cadre de classification

L'établissement de classifications de données dans Miro est conçu pour être flexible et adaptable à tout cadre de classification de données existant au sein de votre organisation.

Les niveaux de classification dans Miro affichent leur ordre de sensibilité actuel. Faites correspondre l'ordre de sensibilité à la hiérarchie de classification de votre organisation, l'ordre de sensibilité 1 étant le niveau de classification le moins sensible.

[Comment configurer les classifications ?](../../canvas-25-admin-features/data-classification/07-define-classification-levels.md)

### Aplanir les cadres de classification

La structure de classification de Miro Enterprise Guard est conçue pour s'adapter à votre politique de classification des données existante.

Si le cadre de classification existant de votre organisation comporte plus d'une couche de hiérarchie (comme des niveaux de sous-classification ou des étiquettes), il peut être nécessaire d'aplanir votre cadre de classification. L'exemple ci-dessous illustre un cadre de classification avec 3 balises qui nécessiterait 3 niveaux de classification distincts par balise et par niveau.

Il est recommandé de limiter au maximum les niveaux de classification.

![Enterprise Guard-Aplatir la classification-hiérarchie.pngAplatir les](images/21016928917010_Enterprise-Guard-Flatten-Classification-Hierarchy.png)
*cadres de classification*

### Lier la documentation et rédiger des descriptions

Des descriptions et des lignes directrices claires en matière de classification informeront vos utilisateurs finaux de la politique de classification, à l'échelle. Lorsque les utilisateurs finaux sont sur le tableau, les descriptions de classification apparaissent à côté de l'étiquette de classification. Les utilisateurs finaux verront un point d'interrogation "en savoir plus" dans chaque panneau qui renvoie à la documentation sur la classification.

|  |  |
| --- | --- |
| **Description de la classification** | Lorsque les utilisateurs cliquent sur l'insigne de classification du tableau, la description du niveau de classification actuel apparaît.  Ajoutez une description significative qui informe vos utilisateurs de la sensibilité de ce tableau et des précautions ou actions recommandées.  Classification-description.png |
| **Lien vers les lignes directrices** | Lorsque l'utilisateur clique sur l'icône "En savoir plus" (icône en forme de point d'interrogation) située à côté du badge de classification du tableau, cette URL est chargée dans un nouvel onglet du navigateur.  Fournissez à vos utilisateurs davantage d'informations sur les niveaux de classification de vos tableaux et sur la manière de les utiliser.  Envisagez d'inclure :   - Qu'est-ce qu'Enterprise Guard ? - Pourquoi c'est important pour votre organisation - Aperçu des aspects de l'expérience de l'utilisateur final qui seront affectés - Explication du cadre de classification de votre organisation - Quelles politiques de réglementation des données seront incluses dans la découverte des données ? - Où poser vos questions et demander un retour d'information ? |

### Définir les critères d'auto-classification

Miro appliquera automatiquement des classifications aux tableaux où un contenu correspondant à la réglementation correspondante en matière de protection de la vie privée est détecté. Chaque niveau de classification peut être lié à plusieurs [étiquettes de sensibilité](../../canvas-25-admin-features/data-discovery/06-sensitivity-labels-and-infotypes-reference.md), mais chaque étiquette de sensibilité ne peut être liée qu'à un seul niveau de classification.

Si plusieurs critères sont remplis, le niveau de classification le plus sensible sera appliqué.

[Comment définir les classifications automatiques ?](../../canvas-25-admin-features/data-classification/09-define-auto-classification.md)

### Sauter la configuration des garde-fous

Comme indiqué précédemment, ce guide vise à donner la priorité à la gestion des changements pour l'utilisateur final, en plus du déploiement d'Enterprise Guard. Nous recommandons de publier les classifications sans garde-fou. Dans cette configuration, la classification des tableaux sera un indicateur visuel mais n'aura pas d'impact sur l'expérience de l'utilisateur final.

Avant d'ajouter des garde-fous aux classifications, résolvez les occurrences inutiles de données sensibles et faites passer les utilisateurs à la classification manuelle pour assurer une transition en douceur sans interférer avec le travail critique qui se déroule sur les tableaux.

### Configurer les garde-fous pour les classifications les plus élevées

Sur la base des conclusions de votre audit initial, vous pouvez décider de déployer les garde-fous sans délai. Envisagez d'appliquer les garde-fous uniquement aux classifications les plus sensibles. Cela permet de concilier l'urgence de sécuriser les données sensibles et l'absence d'impact sur la grande majorité des utilisateurs finaux.

## Publier la classification

Avant de publier les classifications automatiques, vous aurez l'occasion d'examiner leur impact sur vos utilisateurs finaux. Si vous avez configuré les niveaux de classification sans garde-fou, il n'y aura pas d'impact substantiel pour les utilisateurs finaux lors de la publication.

[Comment publier les classifications ?](https://help.miro.com/hc/articles/16494764223378-Review-impact)

### Annonce de classification

Après avoir publié les classifications, envoyez une annonce à vos utilisateurs finaux.

Pensez à inclure les informations suivantes :

- Un bref aperçu d'Enterprise Guard ou une référence à l'annonce précédente
- Aperçu des aspects de l'expérience de l'utilisateur final qui seront affectés
- Explication du cadre de classification de votre organisation
- Quelles politiques de réglementation des données seront incluses dans la découverte des données ?
- Planning des changements à venir
- Où poser vos questions et demander un retour d'information ?

## Résoudre les occurrences inutiles de données sensibles

Avant de diffuser les garde-fous intelligents, nous vous recommandons de communiquer avec les propriétaires de tableaux contenant des informations sensibles. Il est possible que les données sensibles ne soient pas intentionnelles et qu'elles puissent être supprimées.

Informez les utilisateurs que des garde-fous intelligents seront bientôt mis en œuvre conformément aux politiques de sécurité de votre organisation. Vos utilisateurs finaux peuvent en profiter pour supprimer les données sensibles inutiles de leurs tableaux et éviter ainsi de perturber leur travail.

## Les utilisateurs embarqués à la classification manuelle

Même si la classification automatique est activée, de nombreux tableaux resteront non classifiés ou dans la classification par défaut s'ils ne sont pas reclassés manuellement par les utilisateurs finaux.

### Classification manuelle Expérience de l'utilisateur final

[Le propriétaire du tableau, les](../../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md) [copropriétaires du tableau](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md), les éditeurs membres de l’équipe et les admins d’entreprise dotés des autorisations d’admins de contenu peuvent mettre à jour le badge de classification soit en cliquant dessus, soit à partir des détails du tableau. Sélectionnez une nouvelle étiquette et cliquez sur mettre à jour.

Lors de l'ajustement des classifications à un niveau inférieur dans l'ordre de sensibilité (par exemple, de Confidentiel à Public), les utilisateurs devront fournir une justification qui sera enregistrée dans les journaux d'audit de votre compte Miro.

### Communication avec l'utilisateur final

Lors du déploiement initial d'Enterprise Guard, il est recommandé d'envoyer des communications régulières aux utilisateurs finaux afin de les encourager à utiliser les classifications sur chaque tableau. Cela garantira l'utilisation de l'ensemble des garde-fous et des classifications et renforcera donc la sécurité de votre instance Miro.

Pensez à inclure les informations suivantes :

- Un rappel pour classer régulièrement les tableaux
- Instructions sur la manière de classer les tableaux
- Informations sur la fourniture d'une justification
- Vidéo | Classification du tableau des utilisateurs finaux (liens disponibles ci-dessous)

<iframe allowfullscreen="" frameborder="0" height="315" src="//fast.wistia.com/embed/iframe/3ado2k4f6c" width="560"></iframe>
*Classification des tableaux à Miro*

### Ressources

- Classification des tableaux vidéo pour les utilisateurs finaux
  - [Lien Wistia](https://mirohq.wistia.com/medias/3ado2k4f6c)
  - Intégrer le code
    - ```
      <script src="https://fast.wistia.com/embed/medias/3ado2k4f6c.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative ;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100% ;"><div class="wistia_embed wistia_async_3ado2k4f6c seo=false videoFoam=true" style="height :100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100% ;"><img src="https://fast.wistia.com/embed/medias/3ado2k4f6c/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100% ;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1 ;" /></div></div></div></div></div>
      ```

## Déploiement des garde-fous restants

À ce stade, les utilisateurs finaux auraient dû avoir suffisamment de temps pour vérifier que leurs tableaux ne contiennent pas de données sensibles inutiles et pour ajuster manuellement la classification de leurs tableaux.

[Comment déployer des garde-fous intelligents ?](../../canvas-25-admin-features/data-classification/05-define-guardrails.md)

> ⚠️ Soyez prudent lorsque vous appliquez des garde-fous à la classification par défaut du tableau. L'application de garde-fous à la classification par défaut aura un impact significatif sur les utilisateurs finaux , car de nombreux tableaux auront la classification par défaut.

### Annonce des garde-fous

Après avoir publié les garde-fous, envoyez une annonce à vos utilisateurs finaux.

Pensez à inclure les informations suivantes :

- Une référence aux annonces précédentes concernant Enterprise Guard
- Qu'est-ce qu'un garde-fou ?
- Un aperçu des classifications et des garde-fous qui leur sont associés
- Comment ajuster manuellement les classifications ?
- Où poser vos questions et demander un retour d'information ?

## Assouplir les restrictions à la collaboration générale

Enterprise Guard vous permet de déployer des contrôles ciblés. Toutefois, avant Enterprise Guard, il n'existait pas autant d'options permettant d'adapter les contrôles à des cas spécifiques. Il en résulte très probablement des "contrôles généraux", c'est-à-dire des paramètres préventivement stricts qui s'appliquent à la plupart des tableaux et qui, par conséquent, entravent la collaboration de vos utilisateurs Miro.

L'application de contrôles généraux, tels que le verrouillage de la collaboration externe pour tous les utilisateurs et tableaux, manque de précision. Les utilisateurs peuvent subir des frictions lorsque le contenu sur lequel ils collaborent n'est pas sensible et cela peut bloquer des cas d'utilisation entiers de Miro.

Dans l'ensemble, les contrôles de couverture peuvent avoir un impact sur le retour sur investissement que vous obtenez de Miro, mais maintenant avec Enterprise Guard, vos utilisateurs finaux peuvent tirer plus de valeur de Miro tout en s'assurant que le contenu sensible est protégé. Vous devrez réévaluer quelques paramètres de votre compte pour profiter pleinement d'Enterprise Guard.

Assouplissement des restrictions applicables aux tableaux

### Autres paramètres vs Enterprise Guard

Dans Miro, il y a trois zones de réglage qui travaillent ensemble pour déterminer l'expérience réelle de l'utilisateur.

- Paramètres de l’entreprise
- Paramètres de l’équipe
- Enterprise Guard

Lorsqu'il existe des paramètres concurrents, c'est le paramètre le plus strict qui est mis en œuvre. Pour plus d'informations, cliquez ici.

### Paramètres pertinents et où les trouver

Vous devrez réévaluer quelques paramètres pour vous assurer que Miro est configuré de manière holistique. Voici une liste des paramètres pertinents et de l'endroit où les trouver dans votre compte Miro. Certains paramètres peuvent être contrôlés à la fois au niveau de l'entreprise et au niveau de l'équipe.

N'oubliez pas que si deux paramètres s'appliquent à la même partie de l'expérience Miro, c'est le paramètre le plus strict qui dictera l'expérience.

|  |  |  |
| --- | --- | --- |
| **Paramètres** | **Description** | **Où il est disponible** |
| Liens publics | Un lien public permet d'accéder à un tableau sans se connecter. Il peut être configuré pour un accès en vue, en commentaire ou en édition et nécessiter un mot de passe. | Les rôles relatifs à l’entreprise  Niveau équipe  Enterprise Guard |
| Intégration | Contrôle si et comment les utilisateurs peuvent intégrer les tableaux Miro dans d'autres logiciels ou sites web. | Les rôles relatifs à l’entreprise |
| Paramètres de l'invité | Un invité est un utilisateur qui n'est invité qu'à un seul tableau plutôt qu'à une équipe ou un compte entier. | Les rôles relatifs à l’entreprise  Niveau équipe |
| Partage de tableau | Contrôle la manière dont les tableaux peuvent être partagés avec d'autres utilisateurs du compte, au sein des équipes et entre elles. | Niveau équipe  Enterprise Guard |
