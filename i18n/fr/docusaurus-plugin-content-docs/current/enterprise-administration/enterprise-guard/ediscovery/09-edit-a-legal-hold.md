---
title: Modifier une mise en suspens juridique
article_id: 27968005251090
translation_id: 27968005251090
locale: fr
sidebar_position: 8
created_at: '2025-07-09T17:31:49Z'
updated_at: '2025-11-25T15:52:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
---

Modifier une mise en suspens juridique permet aux admins eDiscovery d'ajuster et de peaufiner les efforts de préservation juridique en cours à mesure que les besoins de l'enquête évoluent. Que de nouveaux responsables soient identifiés, que des tableaux Miro supplémentaires deviennent pertinents ou que des tableaux ou utilisateurs existants ne soient plus concernés, modifier une mise en suspens juridique garantit que les données correctes restent préservées et défendables tout au long du processus judiciaire.

Les admins peuvent mettre à jour le nom ou la description de la mise en suspens juridique et ajouter ou supprimer des utilisateurs et des tableaux selon les besoins. Cette flexibilité soutient des workflows juridiques dynamiques et garantit que la conservation reste précise, à jour et conforme à l'étendue de la question juridique, maintenant ainsi la conformité tout en évitant la conservation inutile des données.

Lorsque la mise en suspens juridique est modifiée :

- Les tableaux nouvellement ajoutés à la réserve commenceront à conserver leurs versions à partir de ce moment.
- Les tableaux ou utilisateurs retirés de la mise en suspens juridique cesseront d'être conservés, et leurs versions ne seront plus préservées dans le cadre de cette mise en suspens juridique.
- Les tableaux toujours mis en suspens continueront de voir toutes leurs versions préservées, y compris toute suppression survenant après l'application de la suspension.

Cette approche garantit que les organisations peuvent répondre aux demandes légales avec précision et responsabilité à mesure qu'une enquête progresse.

Pour modifier une mise en suspens juridique, procédez comme suit :

:::note
Vous devez avoir le rôle d'[administrateur eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) pour effectuer cette tâche. Pour demander le rôle d'admin eDiscovery, contactez l'admin d'entreprise.
:::

1. Accédez à vos paramètres Miro.
2. Dans le volet de gauche, sous **Enterprise Guard**, cliquez sur **eDiscovery**.
3. Sur la page **eDiscovery**, cliquez sur l'onglet **Enquêtes**.
4. Cliquez sur l'enquête dans laquelle vous souhaitez modifier une mise en suspens juridique.
   La liste des mises en suspens juridiques dans l'enquête apparaît.
5. Cliquez sur les trois points à la ligne de la mise en suspens juridique que vous souhaitez modifier, puis cliquez sur **Modifier la mise en suspens juridique**.
6. Sur la page **Modifier la mise en suspens juridique**, saisissez ou sélectionnez les informations appropriées pour chaque champ. Le tableau suivant présente chaque champ et sa description.

   |  |  |
   | --- | --- |
   | **Champ** | **Description** |
   | Nom de la mise en suspens  **(obligatoire)** | Nom de la mise en suspens juridique.  Longueur maximale : 60 caractères. |
   | Critères  **(obligatoire)** | Type de contenu inclus pour cette mise en suspens juridique. Cette version ne prend en charge que tout le contenu. |
   | **Personnes qui sont propriétaires, copropriétaires, ou qui ont consulté, modifié ou créé du contenu**  **(obligatoire)** | Ajoutez les utilisateurs que vous souhaitez placer en mise en suspens juridique. Cliquez sur le champ pour rechercher par nom ou par adresse e-mail. Vous pouvez avoir jusqu'à 200 utilisateurs par mise en suspens juridique, y compris ceux ajoutés lors des mises à jour de mise en suspens juridique.  **Notes :**  Lorsqu'un utilisateur sous mise en suspens juridique ouvre, modifie ou interagit avec un tableau de quelque manière que ce soit (en le renommant ou en ajoutant du contenu), ce tableau est marqué et préservé. Par exemple, si le nom du tableau est modifié ou si le contenu est mis à jour, il sera automatiquement placé en mise en suspens juridique. En outre, la propriété et la création de tableaux sont mises en attente.  - Lorsqu’une mise en suspens juridique est modifiée, elle s'applique aux tableaux que les dépositaires ont créés, possédés ou copossédés au moment de la suspension. De plus, tous les tableaux auxquels les administrateurs accèdent et qu'ils modifient après la mise en place de la rétention sont également inclus. Les détails d'accès et de mise à jour des tableaux historiques ne sont pas disponibles dans cette version.  - Les tableaux nouvellement ajoutés à la mise en suspens commenceront à avoir leurs versions préservées à partir du moment où vous enregistrez les mises à jour de la mise en suspens juridique à l'étape 9.  Les tableaux ou utilisateurs retirés de la mise en suspens juridique cesseront d'être préservés, et leurs versions ne seront plus conservées dans le cadre de cette mise en suspens juridique.  Les tableaux toujours mis en suspens continueront à conserver toutes les versions, y compris les suppressions qui surviennent après l'application de la suspension. |
7. Cliquez sur **Suivant**. La page **Examiner l’impact** s’affiche.
8. Examinez l’impact de cette mise en suspens juridique, comme :
   - Le nombre de tableaux qui restent en suspens, seront libérés de la suspension, et ajoutés à la suspension.
   - Les utilisateurs qui possédaient, copropriétaires, consultaient, modifiaient ou créaient les tableaux.
   - Les critères pour la suspension.
   - La liste des tableaux toujours mis en suspens.

   **Remarques :**
   Les tableaux sous conservation légale peuvent toujours être accessibles et modifiables, mais toutes les versions seront préservées. Tout contenu supprimé reste disponible dans la conservation légale. Le nombre d’éléments de contenu inclus dans la conservation légale pourrait augmenter en fonction des actions ultérieures des utilisateurs.

   - Lorsqu'un utilisateur sous mise en suspens juridique ouvre, modifie ou interagit avec un tableau de quelque manière que ce soit (renommage ou ajout de contenu), ce tableau est signalé et conservé. Par exemple, si le nom du tableau est modifié ou si le contenu est mis à jour, il sera automatiquement mis en suspens juridique. De plus, la propriété et la création de tableaux sont mises en attente.

   Lorsqu'une mise en suspens juridique est créée, elle s'applique aux tableaux que les dépositaires ont créés, possédés ou copossédés au moment de la mise en suspens. De plus, tous les tableaux auxquels les responsables accèdent et qu'ils modifient après la mise en place de la restriction sont également inclus. Les détails d'accès et de mise à jour des tableaux historiques ne sont pas disponibles dans cette version.
9. Après avoir examiné l'impact de la mise en suspens juridique que vous créez, cliquez sur **Enregistrer la mise en suspens juridique**.
   La page d'enquête apparaît, affichant la mise à jour de la mise en suspens juridique, comme le nom de la mise en suspens juridique, le type de contenu affecté par la mise en suspens juridique, le nombre d'utilisateurs dans cette mise en suspens juridique, la date de création de la mise en suspens juridique, l'état de la mise en suspens juridique, et le nombre de tableaux en mise en suspens juridique.
