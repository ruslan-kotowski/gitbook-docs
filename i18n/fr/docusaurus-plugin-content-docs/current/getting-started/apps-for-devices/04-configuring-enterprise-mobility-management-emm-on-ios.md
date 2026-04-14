---
title: Configurer la gestion de la mobilité d’entreprise (EMM) sur iOS
article_id: 10183062016274
translation_id: 10183062016274
locale: fr
sidebar_position: 4
created_at: '2023-02-20T18:20:46Z'
updated_at: '2025-11-25T15:36:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: desktop-mobile-tablet-app
availability:
  notes: 'générales: de la configuration de la solution EMM/MDM de votre entreprise
    à l''aide de trois exemples de logiciels spécifiques : VMWare Workspace ONE, Ivanti
    Neurons (anciennement MobileIron Cloud) et Intune (Microsoft Endpoint Manager).
    Si vous utilisez une autre solution, nous vous recommandons de consulter la documentation
    de votre fournisseur EMM pour connaitre la marche à suivre.'
---

L’EMM permet aux admins d’entreprise de configurer et de distribuer Miro aux utilisateurs de leur organisation de manière centralisée et unifiée. Miro prend en charge le provisionnement des paramètres suivants sur les appareils des utilisateurs finaux :

- Désactivation du flux d’inscription.
- Restriction des fournisseurs d’authentification pris en charge (par exemple, réseaux sociaux, fournisseurs de services de messagerie électronique, etc.).
- Restriction du nom d’utilisateur à une valeur spécifique ou à une liste de domaines e-mail autorisés.
- Configuration avancée de l’authentification unique.

## Procédure de configuration

### Ajout de Miro au répertoire d’applications de votre organisation

Dans la plupart des cas, l’activation de la configuration EMM nécessitera l’ajout de Miro au catalogue d’applications de votre organisation. Ce processus peut varier d’un fournisseur EMM à l’autre. Toutefois, en règle générale, il vous faudra ajouter Miro à votre catalogue d’applications directement à partir de l’Apple Store et définir une politique de distribution basée sur des groupes d’appareils, des groupes d’utilisateurs, etc.

#### Exemples

**VMware Workspace ONE**

Le guide général de déploiement de VMware Workspace ONE est disponible [ici](https://techzone.vmware.com/managing-android-devices-workspace-one-operational-tutorial#deploying-android-applications) (uniquement en anglais).

1. Cliquez sur **Ajouter** puis sur **Application publique.**
2. Sélectionnez **Android** dans le menu déroulant de la plateforme puis **la source** Rechercher sur l’App Store.
3. Saisissez « **Miro** » dans la **zone de texte Nom** et cliquez sur Suivant.
4. Sélectionnez l’application Miro et appuyez sur **Approuver** dans l’invite qui s’affiche éventuellement.
5. Publiez l’application en cliquant sur **Enregistrer et affecter**.
6. Configurez les affectations et les paramètres de distribution en fonction des préférences de votre organisation.

Ivanti Neurons

1. Allez dans **Apps (Applications) > App Catalog (Catalogue d’applications)** et cliquez sur **Add (Ajouter)**.
2. Sélectionnez « **iOS store** », puis votre pays comme source.
3. Recherchez "**Miro**" et sélectionnez "**Miro : Tableau blanc en ligne**" dans la liste des applications disponibles.
4. Configurez les paramètres et les politiques de distribution en fonction des préférences de votre organisation.

Intune (Microsoft Endpoint Manager)

[Le guide général de déploiement d’Intune de MS est disponible](https://learn.microsoft.com/mem/intune/fundamentals/deployment-guide-platform-ios-ipados) ici.

1. Allez dans **Apps (Applications) > iOS/iPadOS** et cliquez sur **Add (Ajouter)**.
2. Sélectionnez **Store App (Application du Store) > iOS store app (Application du Store iOS)** comme **App type (Type d’application)**.
3. Cliquez sur **Search the App Store (Rechercher sur l’App Store)**.
4. Sélectionnez le pays de la boutique que vous préférez utiliser.
5. Recherchez "**Miro**" et sélectionnez "**Miro : Tableau blanc en ligne**" dans la liste des applications disponibles.
6. Configurez les paramètres et les politiques de distribution en fonction des préférences de votre organisation.

### Pré-remplissage des paramètres de l’application

Miro utilise AppConfig comme moyen unifié de configurer et de sécuriser les données des clients. De nombreuses solutions EMM prennent en charge le format AppConfig ou l’acceptent dans un « mode de compatibilité ». Pour connaitre les restrictions exactes qui s’appliquent à votre cas, consultez la documentation de votre fournisseur EMM.

#### Exemples

**VMWare Workspace ONE**

Le guide général de déploiement de VMware Workspace ONE est disponible [ici](https://techzone.vmware.com/managing-android-devices-workspace-one-operational-tutorial#deploying-android-applications) (uniquement en anglais).

1. Allez dans **Ressources > Applications**.
2. Cliquez sur **Attribuer** dans la fenêtre **État de l'installation** dans la colonne  Statut de  l'installation sur le site**Miro : Tableau blanc en ligne** application row.
3. Remplissez les champs **Nom, Groupes d’affectation** et **Méthode de livraison de l’application** de la distribution.
4. Activez les options **Accès géré** et **Envoyer la configuration**.
5. Définissez la configuration de l’application.

Ivanti Neurons

1. 1. Allez dans **Apps (Applications) > App Catalog (Catalogue d’applications)**.
   2. Naviguez vers "**Miro : Tableau blanc en ligne**" paramètres.
   3. Allez dans **App configurations (Configuration des applications) > Apple Managed App Configuration (Configuration des applications gérées par Apple)**.
   4. Cliquez sur **Add (Ajouter)** pour créer un nouveau profil de distribution.
   5. Définissez le nom de votre profil de configuration.
   6. Définissez **Apple Managed App Settings (Paramètres des applications gérées par Apple)**.
   7. Sélectionnez le profil de distribution dans la section **Distribute this App Config (Distribuer cette configuration d’application)**.

Intune (Microsoft Endpoint Manager)

[Le guide général de déploiement d’Intune de MS est disponible](https://learn.microsoft.com/mem/intune/fundamentals/deployment-guide-platform-ios-ipados) ici.

1. 1. Allez dans **Apps (Applications) > App configuration policies (Politiques de configuration des applications)**.
   2. Cliquez sur **Add (Ajouter) > Manager device (Appareil de gestion)** pour créer une nouvelle configuration d’application.
   3. Définissez le nom de votre profil de configuration.
   4. Sélectionnez **iOS/iPadOS** comme **Platform (Plateforme)**.
   5. Sélectionnez **Miro : Tableau blanc en ligne** comme **application cible** en cliquant sur **Select app.**
   6. Sélectionnez **Use configuration designer (Utiliser l’utilitaire de configuration)** comme **Configuration settings format (Format des paramètres de configuration)**.
   7. Définissez la configuration de l’application.
   8. Sélectionnez le profil de distribution pour la configuration.

## Liste complète des paramètres pris en charge

### Limitation des options « Se connecter avec... »/« S’inscrire »

Si l’option « S’inscrire » est activée, tous les paramètres « Se connecter avec... » affecteront le flux d’inscription.

:::warning
Toute clé qui n’est pas explicitement définie sur « vrai », ou qui est absente, est considérée comme étant définie sur « faux ». L’option d’authentification est donc disponible (comportement par défaut).
:::

| Clé | Type | Valeurs autorisées |
| --- | --- | --- |
| **Facebook** Miro.authentication.facebookRestricted | Booléen | vrai/faux |
| Google Miro.authentication.googleRestricted | vrai/faux |
| **Microsoft Office 365** Miro.authentication.office365Restricted | vrai/faux |
| **Slack**  miro.authentication.slackRestricted | vrai/faux |
| **AppleID** Miro.authentication.appleIdRestricted | vrai/faux *Disponible uniquement sur les appareils Apple |
| inscription miro.authentication.signUpRestricted | vrai/faux |
| **Connectez-vous avec le lien magique** Miro.authentication.magicLinkRestricted | vrai/faux |
| **Espace de travail Enterprise** Miro.authentication.enterpriseWorksSpaceDisabled | vrai/faux |

### Restrictions relatives aux noms d’utilisateur

Les clients qui souhaitent améliorer la sécurité tout en conservant l’authentification par mot de passe simple peuvent utiliser les options suivantes.

| Clé | Valeur | Description |
| --- | --- | --- |
| **Nom d'utilisateur prédéfini** Miro.policy.authentication.username | **Type de valeur :** chaine de caractères | Le champ est verrouillé et ne peut pas être modifié par l’utilisateur. |
| **Domaines sur liste blanche** Miro.policy.authentication.allowedDomains | **Type de valeur :** table  **Valeur :** @miro.com, @votredomaine.com  *Certains fournisseurs ne prennent pas en charge les données de type **table**.  Dans ce cas, veuillez utiliser le type **string** et le tableau JSON comme valeur. ["@miro.com", "@votredomaine.com"] | Seules les adresses e-mail correspondant à l’un des domaines répertoriés sont autorisées. |

### Configuration de l’authentification unique

Pour améliorer la sécurité de l’organisation et simplifier le processus d’authentification des utilisateurs finaux, les admins de l’organisation peuvent configurer la politique d’authentification unique à l’aide de l’exemple suivant.

:::warning
Assurez-vous que la politique d’authentification unique dans la configuration de l’application correspond aux paramètres d’authentification unique de l’organisation Miro. La non-concordance de ces politiques peut entrainer une situation de « verrouillage » qui empêche les utilisateurs de se connecter. Miro ne peut pas valider les paramètres avant de les appliquer aux appareils cibles.
:::

|  |  |
| --- | --- |
| Clé de configuration | miro.policy.sso |
| Type de valeur de configuration | chaîne de caractères |
| Objet de politique | \{ "authenticationRestricted" : false, "email" : "user@domain.com", "allowedDomains" : ["domain1.com", "domain2.com"], "forceSsoLogin" : true \} |

| Attributs de l’objet de politique | | | |
| --- | --- | --- | --- |
| Paramètre | Type | Description | Remarque |
| authenticationRestricted | booléen | Indique si le bouton « Se connecter via l’authentification unique » est activé sur la page principale. | **La clé est ignorée lorsque d’autres options de configuration sont fournies.** |
| e-mail | chaîne de caractères | Adresse e-mail prédéfinie pour la connexion par authentification unique. | Le champ est verrouillé et ne peut pas être modifié. |
| allowedDomains | booléen | Garde l’authentification unique comme seule méthode d’authentification disponible. | Un utilisateur final est immédiatement redirigé vers la page « Se connecter avec l’authentification unique ». Les options autres qu’**email** et **allowedDomains** sont ignorées. Aucune autre méthode d’authentification n’est disponible. |
