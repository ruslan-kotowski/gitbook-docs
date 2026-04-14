---
title: Comment autoriser ou restreindre la copie et l’exportation de tableaux et de
  contenu
article_id: 360018350399
translation_id: 360018350399
locale: fr
sidebar_position: 14
created_at: '2020-12-14T06:10:03Z'
updated_at: '2026-01-22T14:23:08Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: export-pdf-canvas
availability:
  notes: 'Qui peut le faire: Membres de l''équipe, admins d''équipe (Configuration),
    admins d''entreprise (Configuration) Quels forfaits: Starter, Business, Enterprise,
    Education Quelles plateformes: Navigateur, Bureau, Mobile'
---

Les admins d’entreprise et les admins d'équipe peuvent spécifier si les membres de l'équipe et les non-membres peuvent copier le contenu des tableaux, et définir le paramètre de copie par défaut pour les nouveaux tableaux.

Les propriétaires et copropriétaires de tableaux peuvent spécifier les paramètres de copie pour les autres membres de l'équipe sur un tableau donné. Si les admins permettent aux non-membres de copier les tableaux, ce qui inclut les visiteurs et les invités, alors les propriétaires et copropriétaires peuvent autoriser les non-membres à copier.

Si les admins n'autorisent pas les non-membres à copier le contenu, alors l'option du tableau permettant aux non-membres de copier un tableau est supprimée.

:::note
Sur les forfaits Free, la copie des tableaux est activée par défaut et ne peut pas être modifiée.
:::

## Comment définir les autorisations de copie de tableau pour une équipe

Pour une équipe donnée, un admin d’entreprise ou un admin d’équipe peut spécifier si des personnes externes à l'équipe peuvent copier et exporter les tableaux et le contenu, et définir les autorisations de copie par défaut pour les nouveaux tableaux créés.

Suivez les étapes suivantes :

1. Allez à **Admin Console**.
2. Cliquez sur **Équipes**.
3. Cliquez sur la ligne pour **\{Team name\}**.
   Le panneau **\{Team name\}** s'ouvre.
4. Cliquez pour ouvrir l'onglet **Paramètres**.
5. Faites défiler jusqu'à **Sécurité du contenu**.
6. Pour **Copier le contenu**, spécifiez si seuls les membres de l'équipe ou toute personne de l'organisation peut copier le contenu du tableau.
7. Spécifiez le **Paramètre par défaut pour copier le contenu**. Les propriétaires de tableaux peuvent modifier ce paramètre pour les tableaux individuels.
   Vos paramètres sont enregistrés automatiquement.

:::note
Si le contenu du tableau ne peut pas être copié par les personnes extérieures à l’équipe, alors l’option **Toute personne ayant accès au tableau** est supprimée des paramètres des tableaux. Par exemple, les visiteurs et les invités ne sont pas autorisés à copier du contenu.
:::

:::note
La copie d’images entre des tableaux privés reliés à différentes équipes n’est pas possible. Contactez votre admin d’entreprise Miro pour lui demander l’autorisation d’accéder à l’autre tableau afin de copier des images.
:::

## Comment définir les autorisations de copie pour un tableau

Pour un tableau donné, un propriétaire ou copropriétaire de tableau peut spécifier qui peut copier le tableau.

Suivez les étapes suivantes :

1. Sur un tableau que vous possédez, co-possédez ou avez créé, cliquez en haut à droite sur **Partager**.
   La fenêtre modale de partage s’ouvre.
2. En bas à droite, cliquez sur **Paramètres de partage**.
3. Sous **Qui peut copier le contenu du tableau**, spécifiez une option.

   > ✏️ Si votre admin d’entreprise ou admin d’équipe désactive l'option **Toute personne ayant accès au tableau**, alors cette option est indisponible.
4. Cliquez sur **Terminé**.
   Vos modifications sont enregistrées automatiquement et s'appliquent à toute personne ayant accès au tableau.

## Options de copie du tableau en fonction du type d’utilisateur

En supposant que **Tout utilisateur ayant accès au tableau** puisse copier le contenu, le tableau suivant montre les autorisations par type d'utilisateur.

|  | Enregistrer le tableau comme modèle | Copier le contenu du tableau | Exporter | Dupliquer | Télécharger les fichiers du tableau |
| --- | --- | --- | --- | --- | --- |
| Membres de l'équipe | ✔ | ✔ | ✔ | ✔ | ✔ |
| Invités | ✘ | ✔ | ✔ | ✔ | ✔ |
| Visiteurs avec un compte Miro | ✘ | ✔ | ✔ | ✔ | ✔ |
| Visiteurs sans compte Miro | ✘ | (Avec accès de modification) ✔ | ✘ | ✘ | ✔ |

:::note
(Enterprise) Si [le déplacement des tableaux entre équipes n'est pas autorisé](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md), alors l'option de dupliquer un tableau est indisponible.
:::

:::note
Notez que certaines options ne sont pas disponibles pour certaines catégories d’utilisateurs, même si le propriétaire du tableau autorise toute personne disposant du lien à en copier le contenu
:::

## Foire aux questions

*Pourquoi est-ce que je ne peux pas copier et coller du contenu sur un tableau Miro ?*

Le propriétaire ou le copropriétaire du tableau peut ne pas autoriser la copie pour votre rôle. Vous pouvez consulter votre rôle dans la barre de collaboration, en haut à droite d'un tableau Miro. Contactez le propriétaire ou le copropriétaire du tableau pour demander les permissions de copie pour votre rôle.

Vous devez également vous assurer que vous êtes connecté à Miro. Si votre rôle dispose des permissions de copie et que vous êtes connecté, connectez-vous et ouvrez le tableau dans un autre navigateur et essayez de copier.

*Pourquoi l’option **Tout le monde avec l'accès au tableau** n’est-elle pas disponible pour moi ?*

Votre/vos admin(s) d’entreprise ou admin(s) d’équipe ont désactivé cette option. Si vous êtes admin d’entreprise ou admin d’équipe, consultez Comment définir les permissions de copie de tableau pour une équipe.

*Comment puis-je permettre aux visiteurs de télécharger des fichiers tout en limitant leur capacité à copier ou dupliquer le tableau ?*

Créez un tableau séparé avec seulement les fichiers, puis activez la copie du contenu du tableau pour toute personne disposant du lien du tableau. Partagez le lien du tableau avec les visiteurs.

Alternativement, vous pouvez intégrer le nouveau tableau avec les fichiers, et activer la copie pour toute personne disposant du lien, dans le tableau d'origine. Pour plus d'informations sur l'intégration, [Intégrer un tableau Miro](../import-and-export/export/02-embed-a-miro-board.md).

*Pourquoi ne puis-je pas trouver **Autorisations** dans le menu **Partager** du tableau ?*

(Payant) Seuls le propriétaire et le copropriétaire du tableau peuvent spécifier les autorisations du contenu. (Gratuit) Les autorisations du contenu ne peuvent pas être modifiées par défaut, ce qui permet la copie pour tous les utilisateurs.

*Puis-je spécifier qui peut charger du contenu sur mon tableau ?*

Toute personne ayant les droits de **Modification** peut charger du contenu sur votre tableau.
