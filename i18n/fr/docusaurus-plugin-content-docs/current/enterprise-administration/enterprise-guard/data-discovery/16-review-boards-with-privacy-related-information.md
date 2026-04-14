---
title: "Examiner les tableaux avec des informations relatives \xE0 la vie priv\xE9\
  e"
article_id: 15431051181458
translation_id: 15431051181458
locale: fr
sidebar_position: 15
created_at: '2023-11-29T16:31:14Z'
updated_at: '2025-11-25T15:39:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

Le tableau de bord Data Discovery permet aux [administrateurs de contenu sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) d'examiner les occurrences de données liées à la confidentialité détectées par la découverte de données et de valider les résultats.

:::note
Pour examiner les tableaux contenant des données liées à la confidentialité, vous devez avoir le [rôle d’admin de contenu sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Pour demander le rôle d’admin du contenu sensible, contactez l’admin de votre entreprise.
:::

Pour revoir un tableau avec des données liées à la confidentialité, procédez comme suit :

1. Accédez à vos [paramètres Miro](https://miro.com/app/settings).
2. Dans le volet de gauche, sous **Enterprise Guard**, cliquez sur **Découverte des données**.
3. Sur la page **Vue d'ensemble de la découverte des données** **Vue d'ensemble**, faites défiler jusqu'à la section sous les métriques, puis cliquez sur le nombre de tableaux pour la catégorie de tableaux que vous souhaitez examiner.
   Une nouvelle page apparaît avec la liste des tableaux et leurs informations.
4. Cliquez sur le tableau que vous souhaitez examiner.
   Un panneau coulissant apparaît à droite de l'écran.
5. Le panneau coulissant vous permet d'effectuer les actions suivantes :
   - **Afficher ou masquer** **les informations relatives à la vie privée** **:** Par défaut. les informations relatives à la vie privée sont masquées. Si vous souhaitez voir des informations liées à la vie privée, cliquez sur le bouton bascule **Afficher les informations sensibles** pour l'activer.
   Lorsque des informations relatives à la vie privée sont visibles, vous pouvez masquer les informations relatives à la vie privée en cliquant sur le bouton bascule **Afficher les informations sensibles** pour le désactiver.

   - **Filtrer** **les informations relatives à la vie privée** **en fonction de la catégorie de données :** Pour afficher les informations relatives à la vie privée qui appartiennent à une étiquette spécifique, cliquez sur l'onglet **Informations relatives à la vie privée**, puis cliquez sur l'étiquette de sensibilité appropriée sous l'onglet.

   **- Supprimer les correspondances faussement positives:** Dans le processus de découverte de données liées à la confidentialité, vous pourriez rencontrer des situations où le système génère des correspondances qui, bien que techniquement exactes, peuvent ne pas être pertinentes ou considérées comme des données sensibles en fonction des différentes politiques de sécurité et des besoins spécifiques d'une organisation. Supprimer une correspondance qui ne présente pas de risque pour la sécurité ou la confidentialité devient crucial pour adapter le processus de découverte des données aux exigences spécifiques d'une organisation en matière de sécurité et de confidentialité des données.

   Il peut aussi arriver que le système identifie à tort des données sur vos tableaux comme probablement sensibles (un faux positif). Divers facteurs contribuent à ces occurrences, notamment la proximité de termes connexes ou le formatage de données liées à la confidentialité. Vous pouvez également supprimer les correspondances faussement positives.

   Lorsque vous supprimez une correspondance, les mises à jour se produisent en temps réel. La classification du tableau et les garde-fous appliqués sont également mis à jour selon la configuration de classification automatique et des garde-fous intelligents.

   Pour supprimer une fausse alerte, cliquez sur l'ellipse à côté de la correspondance de données liée à la confidentialité que vous souhaitez supprimer, puis sélectionnez **Masquer la correspondance**. Notez que les mises à jour se font en temps réel. La classification du tableau et les garde-fous appliqués sont également mis à jour selon la configuration de la classification automatique et des garde-fous intelligents.
6. Cliquez sur le tableau suivant avec lequel vous souhaitez travailler dans la liste des résultats de l'Explorateur de contenu et effectuez les actions nécessaires, ou fermez le panneau coulissant en cliquant sur le bouton **Fermer** en haut à droite du panneau.
