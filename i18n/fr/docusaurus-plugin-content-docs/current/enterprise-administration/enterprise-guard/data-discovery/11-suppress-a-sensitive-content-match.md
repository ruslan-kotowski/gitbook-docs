---
title: Supprimer une correspondance de contenu sensible
article_id: 17144258002962
translation_id: 17144258002962
locale: fr
sidebar_position: 10
created_at: '2024-02-20T00:16:59Z'
updated_at: '2025-11-25T15:41:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

Au cours du processus de découverte de données, il est possible que le système génère des correspondances qui, bien que correctes sur le plan technique, peuvent ne pas être pertinentes ou considérées comme des données sensibles selon les différentes politiques de sécurité et les besoins spécifiques d’une organisation. Supprimer une correspondance qui ne présente pas de risque de sécurité ou de confidentialité est crucial pour adapter le processus de découverte des données aux exigences de sécurité et de confidentialité spécifiques d’une organisation.

Il peut également arriver que le système signale à tort des données de vos tableaux comme susceptibles d’être sensibles (faux-positif). Divers facteurs entrent en jeu pour expliquer ces résultats, notamment la proximité de termes associés ou la mise en forme des données sensibles. Vous pouvez également supprimer les faux-positifs.

Lorsque vous supprimez une correspondance, les mises à jour ont lieu en temps réel. La classification du tableau et les garde-fous appliqués sont également mis à jour selon la configuration de la classification automatique et des garde-fous intelligents.

:::note
Pour supprimer une correspondance de contenu sensible, vous devez avoir [le rôle d’admin de contenu sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Contactez votre admin d’entreprise pour lui demander de vous attribuer le rôle d’admin de contenu sensible.
:::

Pour supprimer une correspondance de contenu sensible, procédez comme suit :

1. Si vous êtes sur la page de l’**explorateur de contenu**, passez à l’étape 2.
   Si vous n’êtes pas sur la page de l’**explorateur de contenu** :
   a. Accédez aux [Paramètres de Miro.](https://help.miro.com/hc/articles/https://miro.com/app/settings)
   b. Dans le volet de gauche, sous **Sécurité et conformité**, cliquez sur **Explorateur de contenu**.
2. Sur la page de **l’explorateur de contenu/de la découverte des données**, cliquez sur le tableau que vous souhaitez examiner.
   Un panneau coulissant apparaît à droite de l’écran.
   ![Figure 1 : volet coulissant](images/21017529201810_slide_out_panel.png)*Figure 1 : panneau coulissant*
3. Cliquez sur les points de suspension à côté de la correspondance de données sensibles que vous souhaitez supprimer, puis sélectionnez **Masquer la correspondance**. Notez que les mises à jour se produisent en temps réel. La classification du tableau et les garde-fous appliqués sont également mis à jour selon la configuration de la classification automatique et des garde-fous intelligents.

    Lorsque vous supprimez une correspondance, les mises à jour ont lieu en temps réel. La classification du tableau et les garde-fous appliqués sont également mis à jour selon la configuration de la classification automatique et des garde-fous intelligents.

   Répétez cette étape pour chaque correspondance de données sensibles que vous souhaitez supprimer.
4. Cliquez sur le tableau suivant avec lequel vous souhaitez travailler dans la liste de résultats de l’explorateur de contenu et effectuez les actions nécessaires, ou fermez le panneau coulissant en cliquant sur le bouton **Fermer** en haut à droite.
