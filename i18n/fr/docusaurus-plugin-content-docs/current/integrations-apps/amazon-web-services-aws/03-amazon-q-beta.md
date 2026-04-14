---
title: Amazon Q (bêta)
article_id: 31347586131346
translation_id: 31347586131346
locale: fr
sidebar_position: 3
created_at: '2025-11-25T13:35:45Z'
updated_at: '2025-12-29T15:25:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: bring-your-own-ai
availability:
  notes: 'Qui peut le faire: Propriétaires de tableau, copropriétaires de tableau,
    éditeurs de tableau, membres de l’équipe, admins d’équipe, admins utilisateurs,
    admins de contenu, admins d’entreprise (installation) ; admin Amazon Q Quels forfaits:
    Business, Enterprise Quelles plateformes: Navigateur, Bureau'
---

L'intégration Amazon Q permet aux équipes de récupérer les connaissances de l'entreprise dans la plateforme Miro IA via les partenaires d’IA et les flux. L'intelligence d'entreprise est fournie et visualisée directement au sein de Miro.

:::note
Vous ne pouvez utiliser l'intégration Amazon Q qu'avec la plateforme Miro IA. [Inscrivez-vous ici](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb) pour obtenir un accès.  Vous serez informé lorsque la plateforme Miro IA sera activée pour votre organisation.
:::

La connaissance d'entreprise est souvent éparpillée à travers de nombreux outils comme Slack, Confluence, Salesforce, Google Drive, et des dépôts internes, ce qui oblige les chefs de produit, les leaders techniques et les équipes technologiques à consacrer un temps précieux à la recherche de détails cruciaux et à l'unification des insights.

Les fonctionnalités suivantes de Miro et Miro IA prennent en charge l'intégration Amazon Q :

- [**Flows**](../../using-miro/miro-ai/04-flows-overview.md)
  Visualisez des workflows qui transforment les informations éparpillées en livrables clairs, aidant les équipes à automatiser et à standardiser la manière dont elles transforment les insights en actions.
- [**Sidekicks**](../../using-miro/miro-ai/06-sidekicks-overview.md)
  Travaillez en tandem avec des agents IA qui utilisent le contenu du tableau et les données d'entreprise pour générer de nouveaux artefacts, fournir des insights instantanés et accélérer l'idéation, la documentation et le design.

## Configurer l'intégration Amazon Q

Assurez-vous que vous vous êtes [inscrit ici](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb) et avez reçu la confirmation de Miro que la plateforme Miro IA est activée pour votre organisation, puis complétez les deux procédures suivantes.

Pour configurer l'intégration d'Amazon Q avec Miro, vous devez ajouter Miro en tant qu’accès aux données dans Amazon Q Business, puis connecter l'index Amazon Q à la console d’admin de Miro.

### Ajouter Miro en tant qu’accès aux données dans Amazon Q Business

1. Dans la console Amazon Q Business, dans le volet de navigation, cliquez sur **Applications**.
2. Cliquez sur l'application où vous souhaitez ajouter un "data accessor".
3. Dans le volet de navigation, cliquez sur **Data accessors**.
4. Cliquez sur **Ajouter un data accessor**.
5. Sous **Data accessors**, pour **Miro**, cliquez sur l'icône plus (**+**).
6. Pour l'**ID externe**, ajoutez l'ID de votre organisation Miro.
   Pour obtenir l'ID de votre organisation Miro, allez dans Miro dans la console d’admin. Copiez l'ID de l'organisation depuis la barre d'URL du navigateur.
   ![](../../../../../../docs/integrations-apps/amazon-web-services-aws/images/31367058137746_image.png)
   *Trouvez votre ID d'organisation dans la console d’admin. Vous pouvez copier l'ID depuis la barre d'URL du navigateur.*
7. Cliquez sur **Ajouter un gestionnaire de données**.
8. Notez les détails suivants. Vous aurez besoin de chaque valeur pour compléter la configuration dans la console d’admin de Miro :
   - ID de l’application
   - ARN de l’application IdC
   - ID de récupérateur
   - Région de l’application
   - Région de l’application IdC

### Connecter un index Amazon Q à la console d’admin de Miro

1. Dans Miro, allez à **Console administrateur** > **Applications & intégrations** > **Applications** > **Ajouter des applications**.
2. Cherchez et localisez Amazon Q.

   > ✏️ Si vous ne parvenez pas à trouver Amazon Q par nom, recherchez par l'ID client suivant : `1601842442647206821`.
3. Dans le profil de l'application, choisissez d'ajouter l'application pour **Toutes les équipes** ou **Équipes spécifiques**.
4. Examinez la page des autorisations.

   > ✏️ L'application Amazon Q est développée et maintenue par Miro, et ne nécessite pas d'autorisations spécifiques.
5. Cliquez sur **Ajouter**.
6. Allez dans **Applications** > **Gérer les applications**.
7. Recherchez et localisez Amazon Q.
8. Cliquez sur **Paramètres**.
9. Ajoutez les détails de l'accès aux données d'Amazon Q. Voir l'étape finale dans Ajouter Miro comme accès aux données dans Amazon Q Business.
10. Cliquez sur **Enregistrer**.
    Votre configuration est appliquée.
