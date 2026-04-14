---
title: "Ajouter une mise en suspens juridique \xE0 une enqu\xEAte"
article_id: 22120471564946
translation_id: 22120471564946
locale: fr
sidebar_position: 7
created_at: '2024-10-21T23:29:24Z'
updated_at: '2025-11-25T16:22:33Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
---

Créer une mise en suspens juridique est un processus crucial pour les [admins eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) lorsque des litiges ou une enquête sont anticipés. Les mises en suspens juridiques garantissent que les tableaux Miro pertinents sont préservés et protégés contre toute altération, suppression ou retrait. Cela est essentiel pour maintenir la conformité aux exigences légales et réglementaires, prévenir la perte ou la modification de données critiques, et sauvegarder des preuves clés tout au long de la durée de l'affaire juridique. Une mise en suspens juridique permet aux admins de verrouiller les données, garantissant que tous les tableaux Miro pertinents sont disponibles pour examen chaque fois que nécessaire.

Créer une mise en suspens juridique implique d’identifier les utilisateurs et tableaux Miro pertinents associés à une enquête et d'appliquer la mise en suspens pour empêcher toute modification. Les admins peuvent gérer plusieurs mises en suspens au sein d'une enquête, s'assurant que toutes les données nécessaires sont regroupées et conservées de manière organisée. Ce processus permet de maintenir l'intégrité et la responsabilité des données, garantissant que l'organisation est pleinement conforme et prête pour le processus légal.

Les tableaux Miro sous mise en suspens juridique peuvent encore être accédés et modifiés, mais toutes les versions sont conservées. Si le contenu est supprimé, il restera disponible dans le cadre de la mise en suspens juridique. Le nombre d'éléments de contenu sous mise en suspens pourrait augmenter en fonction des actions futures des utilisateurs. Une fois un tableau placé sous mise en suspens juridique, toutes les versions du tableau sont conservées indéfiniment, jusqu'à ce que la mise en suspens juridique soit levée.

Pour créer une mise en suspens juridique, procédez comme suit :

:::note
Vous devez avoir le [rôle d’admin eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) pour effectuer cette tâche. Pour demander le rôle d’admin eDiscovery, contactez l’admin de votre entreprise.
:::

1. Accédez à vos paramètres Miro.
2. Dans le volet de gauche, sous **Enterprise Guard**, cliquez sur **eDiscovery**.
3. Sur la page **eDiscovery**, cliquez sur l'onglet **Enquêtes**.
4. Sur la page **Créer une enquête**, cliquez sur l'enquête dans laquelle vous souhaitez ajouter une mise en suspens juridique.
5. Cliquez sur **Ajouter une mise en suspens juridique**.
6. Sur la page **Ajouter une mise en suspens juridique**, saisissez ou sélectionnez les informations appropriées pour chaque champ. Le tableau suivant présente chaque champ et sa description.

   |  |  |
   | --- | --- |
   | **Champ** | **Description** |
   | Nom de la mise en suspens juridique  **(obligatoire)** | Nom de la mise en suspens.  Longueur maximale : 60 caractères. |
   | Critères  **(obligatoire)** | Type de contenu inclus pour cette mise en suspens juridique. Cette version prend uniquement en charge tout le contenu. |
   | **Personnes qui sont propriétaires, copropriétaires, ou qui ont consulté, modifié ou créé du contenu**  **(obligatoire)** | Ajoutez les utilisateurs que vous souhaitez mettre en suspens juridique. Cliquez sur le champ pour rechercher par nom ou adresse e-mail. Vous pouvez ajouter jusqu'à 200 utilisateurs à la fois.    **Remarques :**  - Lorsqu'un utilisateur sous mise en suspens juridique ouvre, modifie ou interagit avec un tableau de quelque manière que ce soit (renommer ou ajouter du contenu), ce tableau est marqué et préservé. Par exemple, si le nom du tableau est modifié ou si le contenu est mis à jour, il sera automatiquement placé en suspens juridique. De plus, la propriété du tableau et sa création sont mises en attente.  - Lorsqu'une mise en suspens juridique est créée, elle s'applique aux tableaux que les propriétaires ont créés, possédés ou co-posédés au moment de la mise en suspens. De plus, tous les tableaux auxquels les propriétaires accèdent et modifient après la mise en place de la mise en suspens sont également inclus. Les détails historiques d'accès et de mise à jour des tableaux ne sont pas disponibles dans cette version. |
7. Cliquez sur **Suivant**. La page **Examiner l’impact** s’affiche.
8. Examinez l'impact de cette mise en suspens juridique, comme le nombre de tableaux existants qui seront mis en suspens et les utilisateurs qui possédaient, co-possédaient, accédaient, modifiaient ou créaient les tableaux.

   **Notes :**
   - Les tableaux en suspens peuvent toujours être consultés et modifiés, mais toutes les versions seront conservées. Si le contenu est supprimé, il restera disponible dans la conservation légale. Le nombre d'éléments de contenu sous mise en suspens juridique pourrait augmenter en fonction des actions futures des utilisateurs.

   - Lorsqu’un utilisateur sous mise en suspens juridique ouvre, modifie ou interagit avec un tableau de quelque manière que ce soit (changement de nom ou ajout de contenu), ce tableau est signalé et préservé. Par exemple, si le nom du tableau est changé ou que le contenu est mis à jour, il sera automatiquement placé en mise en suspens juridique. De plus, la propriété du tableau et sa création sont mises en suspens.

   - Lorsqu'une mise en suspens juridique est créée, elle s'applique aux tableaux que les dépositaires ont créés, possédés ou co-dirigés au moment de la mise en suspens. De plus, tous les tableaux auxquels les dépositaires accèdent et qu'ils modifient après la mise en suspens sont également inclus. Les détails de l'accès et de la mise à jour historiques des tableaux ne sont pas disponibles dans cette version.
9. Après avoir examiné l'impact de la mise en suspens juridique que vous créez, cliquez sur **Ajouter une mise en suspens juridique**.
   La page de l'enquête apparaît affichant la mise en suspens juridique qu'elle contient et les informations sur chaque mise en suspens juridique, telles que le nom de la mise en suspens juridique, le type de contenu affecté par la mise en suspens juridique, le nombre d'utilisateurs concernés par cette mise en suspens, la date de création de la mise en suspens, l'état de la mise en suspens, et le nombre de tableaux concernés par la mise en suspens juridique.
