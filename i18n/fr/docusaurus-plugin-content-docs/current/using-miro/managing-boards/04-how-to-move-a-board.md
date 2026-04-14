---
title: "Comment d\xE9placer un tableau"
article_id: 360017730093
translation_id: 4428486878226
locale: fr
sidebar_position: 4
created_at: '2022-02-18T10:53:58Z'
updated_at: '2026-03-27T16:09:54Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
availability:
  roles: board_owner
  notes: 'Relevant for: All plans'
backstage_link:
  entity_kind: capability
  entity_id: move-board-to-space
---

> **Qui peut le faire :** Les propriétaires de tableau
> **Concerné par :** Tous les forfaits

Chaque utilisateur Miro peut être membre de plusieurs équipes. Votre profil Miro est votre adresse e-mail. Vous pouvez déplacer un tableau Miro d’une équipe à une autre, ou transférer votre tableau Miro vers un autre profil.

:::note
Sur les forfaits Enterprise, les copropriétaires de tableau et les admins de contenu peuvent déplacer des tableaux en utilisant l’[API REST de Miro](https://developers.miro.com/reference/update-board), qui diffère intentionnellement de l’expérience de l’interface utilisateur de Miro, où seuls les propriétaires peuvent déplacer leurs tableaux.
:::

:::note
Les admins d’entreprise du forfait Enterprise peuvent [restreindre l’option de déplacer des tableaux vers et depuis une équipe](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md) pour tous les utilisateurs non-admins et propriétaires de tableaux.
:::

## Scénarios courants

Voici plusieurs scénarios courants impliquant le déplacement de tableaux, ainsi que la section de cet article qui explique comment procéder :

- Vous avez **deux profils Miro** (adresses e-mail associées à Miro) et vous souhaitez déplacer des tableaux d’un profil à un autre.
  *Suivez les étapes décrites dans* [*cette section*](04-how-to-move-a-board.md)*, onglet **Forfait Free**.*
- Vous êtes **passé d’un forfait Free à un forfait payant** et vous souhaitez déplacer les tableaux vers le forfait payant.
  *Suivez les étapes décrites dans* [*cette section*](04-how-to-move-a-board.md)*, onglet **Forfait Free**.*
- Vous souhaitez **déplacer des tableaux entre deux équipes payantes**.
  *Suivez les étapes dans* [*cette section*](04-how-to-move-a-board.md)*, en utilisant l’onglet **Abonnements payants, Education**.*

## Déplacer des tableaux entre des équipes

:::warning
Lorsque vous déplacez un tableau vers une autre équipe, son [historique des versions](12-board-history-versions.md) sera perdu. Si vous souhaitez conserver l’historique des versions, nous vous recommandons de [copier le contenu du tableau](../working-on-the-board/09-copy-as-text-or-as-an-image.md) à la place.
:::

Pour déplacer un tableau entre des équipes, vous devez :

- Être le propriétaire du tableau
- Être membre des deux équipes

Il existe deux façons de déplacer un tableau vers une autre équipe : depuis le tableau de bord ou directement à partir du tableau.

### Comment déplacer un tableau directement à partir du tableau

1. Ouvrez votre tableau et cliquez sur l’icône des trois points (**...**) située à droite du nom de votre tableau (en haut à gauche).
2. Accédez à **Tableau > Déplacer vers > Autre équipe![moving-board-three-dots.png](../../../../../../docs/using-miro/managing-boards/images/21537437708306_moving-board-three-dots.png)**

### Comment déplacer un tableau à l’aide du tableau de bord

1. Allez sur votre tableau de bord pour voir tous les tableaux d’une équipe.
2. Passez votre souris au-dessus de la carte du tableau que vous souhaitez déplacer.
3. Cliquez sur les trois points, puis cliquez sur **Déplacer vers l’équipe**.
   Une boîte de dialogue s’ouvre.
4. Sélectionnez l’organisation vers laquelle vous voulez déplacer le tableau.
5. Sélectionnez une équipe dans cette organisation.
6. Cliquez sur **Déplacer**.

### Comment déplacer un tableau dans un autre espace ?

1. Ouvrez votre tableau et cliquez sur l’icône des trois points (**...**) située directement à droite du nom de votre tableau (coin supérieur gauche)
2. Accédez à **Tableau > Déplacer vers > Autre espace.** Vous pouvez également choisir de notifier les membres de l’équipe que le tableau a été déplacé vers un autre espace.![moving-boards-spaces.png](../../../../../../docs/using-miro/managing-boards/images/21537453797394_moving-boards-spaces.png)*Déplacement d’un tableau vers un autre espace*

### Accès refusé à un utilisateur

Si des collaborateurs du tableau ne font pas partie de l’équipe où le tableau est déplacé, vous verrez un message d’accès refusé.

Il existe deux façons de consulter les adresses e-mail des utilisateurs qui perdront l’accès au tableau après le déplacement. Si le nombre d’utilisateurs est inférieur à 10, vous pouvez consulter la liste des adresses e-mails en cliquant sur **Afficher les adresses e-mail des utilisateurs** dans le **message Accès refusé.** Si le nombre est supérieur à 10, un lien proposera de télécharger la liste des adresses e-mail.

Pour vous assurer que tous les collaborateurs conservent l’accès au tableau, vous pouvez [inviter des membres dans la nouvelle équipe](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) avant de déplacer le tableau.

Vous pouvez également choisir **Déplacer quand même** et ajouter à nouveau des collaborateurs au tableau une fois qu’il est déplacé.

![warning when moving a board.png](../../../../../../docs/using-miro/managing-boards/images/16759524012690_warning%20when%20moving%20a%20board.png)
*Message d’accès refusé lors du déplacement d’un tableau d’une équipe à l’autre*

**Si vous déplacez un tableau vers une équipe sur forfait Free**, il sera partagé avec tous les membres de l’équipe.

![private boards are not available in free teams.png](../../../../../../docs/using-miro/managing-boards/images/16759539790738_private%20boards%20are%20not%20available%20in%20free%20teams.png)
*Les tableaux privés ne sont pas disponibles dans les équipes gratuites*

## Déplacer des tableaux entre des profils

Dans Miro, votre profil correspond à l’adresse e-mail que vous avez utilisée pour votre inscription. Si vous avez employé deux adresses e-mail différentes, cela signifie que vous avez deux profils. Vous pouvez transférer un tableau d’un profil à un autre.

### Comment déplacer des tableaux entre des profils

Forfaits payant, Education Forfait Free

Si le tableau se trouve dans une équipe titulaire d’un forfait payant ou Education et que vous souhaitez le déplacer vers une autre équipe elle aussi titulaire d’un forfait payant ou Education, enregistrez simplement la sauvegarde du tableau et chargez-la dans cette équipe.

1. Ouvrez votre tableau de bord.
2. Passez votre souris au-dessus de la carte du tableau que vous souhaitez déplacer.
3. Cliquez sur les trois points.
4. Cliquez sur **Télécharger la sauvegarde du tableau**.
5. Le fichier .rtb sera enregistré sur votre appareil.

   ![board-backup.png](../../../../../../docs/using-miro/managing-boards/images/23122136352530_board-backup.png)
6. Connectez-vous à votre autre profil Miro.
7. Passez à l’équipe vers laquelle vous souhaitez déplacer le tableau.
8. Cliquez sur **+ Créer nouveau** > **Importer** > **Importer sauvegarde**.
9. Le sélecteur de fichiers s’ouvre.
10. Choisissez le fichier de sauvegarde .rtb que vous avez précédemment enregistré et cliquez sur **Ouvrir**. Le tableau sera alors disponible depuis votre tableau de bord.

    ![board-import-backup.png](../../../../../../docs/using-miro/managing-boards/images/23122136353682_board-import-backup.png)

Suivez ces étapes si votre tableau est situé dans une équipe titulaire du forfait Free ou si vous devez déplacer un tableau vers une équipe Free.

1. Connectez-vous à Miro sous votre premier profil.
2. Partagez le tableau avec le deuxième profil. Cliquez sur **Partager**.
   ![free-sharing-board.png](../../../../../../docs/using-miro/managing-boards/images/23122136354066_free-sharing-board.png)
3. Entrez l’e-mail pour le deuxième profil > cliquez sur **Envoyer les invitations**.

   ![free-sharing-board-dialog.png](../../../../../../docs/using-miro/managing-boards/images/23122136354706_free-sharing-board-dialog.png)
4. Transférez la propriété du tableau du profil #1 vers le profil #2. Cliquez sur le bouton **Partager** > **Paramètres de partage** > choisissez le profil #2 > sélectionnez **Propriétaire** dans le menu déroulant.
5. Connectez-vous à Miro avec votre profil #2 où vous verrez le tableau.
6. Déplacez le tableau vers une autre équipe.

:::warning
Si votre deuxième profil dispose d’un forfait Free et que vous invitez votre profil Free sur un profil payant, vous utiliserez une licence de votre forfait payant. Si vous dépassez ainsi le nombre de licences de votre forfait, une licence supplémentaire peut vous être facturée.
:::

## Foire aux questions

**Pourquoi l’option pour déplacer un tableau vers une autre équipe n’est-elle pas disponible dans le menu de mon tableau ?**

Seuls les propriétaires de tableau qui sont membres de plusieurs équipes peuvent déplacer des tableaux entre des équipes. Si vous n’êtes pas le propriétaire du tableau, vous pouvez [dupliquer le tableau](03-how-to-duplicate-a-board.md) (si cela est permis dans [les paramètres de contenu du tableau](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md)) et déplacer la copie du tableau.

L’option pour déplacer les tableaux peut également être restreinte par les admins d’entreprise sur le forfait Enterprise.

**Comment puis-je transférer la propriété de mon tableau à un autre utilisateur ?**

Découvrez comment [transférer la propriété d’un tableau à un autre collaborateur](05-how-to-transfer-board-ownership.md).

**Le lien du tableau est-il modifié lorsque je déplace le tableau vers une autre équipe ?**

Non, l’URL du tableau ne change pas.

**Puis-je déplacer un tableau modèle vers l’équipe d’un autre utilisateur ?**

Oui, vous pouvez soit demander à l’utilisateur de vous inviter dans son équipe puis déplacer le tableau, soit [partager le tableau](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) et leur permettre de [dupliquer votre tableau](03-how-to-duplicate-a-board.md) dans les [paramètres de contenu du tableau](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md).

**Puis-je déplacer des espaces entre les équipes ?**

Non, vous pouvez uniquement déplacer des tableaux.

**Puis-je déplacer plusieurs tableaux à la fois ?**

Non, ce n’est pas possible pour le moment.

**J’essaie de déplacer mon tableau et rien ne se produit ou un message d’erreur s’affiche. Que dois-je faire ?**

Veuillez essayer de déplacer le tableau dans un autre navigateur ou en mode incognito. Vous pouvez également essayer de basculer sur un autre réseau ou appareil.

Une autre option est de [dupliquer le tableau](03-how-to-duplicate-a-board.md) et de déplacer la copie. Si cela ne fonctionne pas, [signalez le problème au service d’assistance de Miro](../tools/troubleshooting/06-contacting-miro-support.md).
