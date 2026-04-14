---
title: Déplacer des données entre régions – Migration automatique
article_id: 24866660560402
translation_id: 24866660560402
locale: fr
sidebar_position: 5
created_at: '2025-02-24T08:47:08Z'
updated_at: '2025-10-29T14:40:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Qui peut le faire: Administrateurs de l''entreprise Quels forfaits: Enterprise
    Quelles plateformes: Navigateur, Bureau'
---

:::note
La migration automatique est un service payant avec des services professionnels. Pour obtenir un devis, contactez votre interlocuteur Miro dédié.
:::

Cet article explique la migration automatique des données. Pour en savoir plus sur d'autres options de déplacement de données entre régions, voir [Déplacer des données entre régions](../../canvas-25-admin-features/data-residency/03-move-data-between-regions.md).

## Données incluses dans une migration automatique entre régions

La liste suivante montre les données incluses dans une migration automatique entre régions :

- Tableaux, contenu des tableaux, et paramètres de partage des tableaux
- Hiérarchie du contenu, y compris les équipes, les espaces, et les sections d'espaces
- Paramètres de l'organisation, des équipes, et des tableaux
- Utilisateurs, profils d'utilisateur, et paramètres d'utilisateur, y compris les invités
- Journaux d'audit, classification des données, et paramètres de sécurité du contenu

## Préparer une migration de données entre régions

Pour vous préparer à une migration de données entre régions, suivez ces étapes :

1. Pour garantir que vous puissiez gérer tous les utilisateurs de votre domaine, vérifiez tous les domaines que vous possédez avec la vérification DNS.
2. Activez la politique de **Contrôle de domaine pour bloquer les abonnements propres**, ce qui garantit que les utilisateurs ne créent pas accidentellement des abonnements Miro Free dans votre ancienne région.
3. Consolidez les équipes et/ou organisations en une seule organisation avec un seul abonnement.
4. Vérifiez quelles intégrations votre organisation utilise et dont elle a besoin dans la nouvelle région, puis planifiez un planning pour reconfigurer chaque intégration dans votre nouvelle région.

## Comment fonctionne une migration de données interrégionale et combien de temps elle dure

Une migration interrégionale comprend les cinq étapes suivantes :

- **Préparation**
  En général 4-8 semaines. L’admin d’entreprise, soutenu par Miro, prépare son organisation pour la migration, planifie le temps d’arrêt de la migration et communique avec les utilisateurs finaux.
- **Migration**
  Temps d’arrêt habituellement inférieur à 8 heures. L'organisation et ses données sont migrées vers la nouvelle région.

  > ✏️ L'équipe Miro coordonne avec vous pour choisir la date de migration. Si la migration échoue pour une quelconque raison, l'accès à votre région source est rétabli, et Miro coordonne avec vous une nouvelle date de migration pour réessayer.
- **Vérification et configuration**
  Typiquement 2-3 semaines. L'admin doit reconfigurer certaines intégrations, comme le SSO, dans la nouvelle région. L'admin et les utilisateurs vérifient que leurs tableaux et leurs données ont bien été transférés dans la nouvelle région comme prévu.
- **Formation**
  Typiquement 2-3 semaines. Les utilisateurs sont formés sur l'accès à leur nouvelle organisation Miro.
- **Conformité**
  Dans les 120 jours suivant la date de migration – Miro vérifie que les données de l'organisation ont été supprimées de la région source.

## Que faire après une migration automatisée de données interrégionales

Après une migration de données interrégionales, assurez-vous de faire ce qui suit :

- Reconfigurez immédiatement l'SSO, si applicable, pour les nouveaux sous-domaines régionaux. Par exemple, au.miro.com.

  > ✏️ Vos utilisateurs ne peuvent pas se connecter à la nouvelle région tant que l'SSO n'est pas reconfiguré du côté de l'IdP.
- Reconfigurez SCIM pour les nouveaux sous-domaines régionaux. Par exemple, au.miro.com.
- Vérifiez que **Bloquer les abonnements personnels** dans les paramètres de contrôle de domaine est activé.
- Validez vos autres paramètres de contrôle de domaine.
- Réinstallez et configurez les applications et intégrations pertinentes.

## FAQ sur les migrations automatisées de données interrégionales

**Qu’est-ce qu’une migration de données interrégionale ?**

Les migrations de données interrégionales automatisent le déplacement des données client d’une région géographique à une autre. Le résultat final d’une migration interrégionale est que vos données client Miro couvertes par le processus seront stockées et traitées dans la nouvelle région.

**Comment cela fonctionne-t-il et combien de temps cela prend-il ?**

Voir Comment fonctionne une migration de données interrégionale et combien de temps elle dure.

**Qui est éligible, et qui ne l'est pas ?**

Pour automatiser une migration interrégionale, vous devez être un client Enterprise. Cependant, un client Enterprise utilisant Enterprise Guard et la gestion des clés de chiffrement n'est pas éligible. Pour plus d'informations, contactez votre interlocuteur Miro.

**Quelles données sont incluses dans une migration automatisée interrégionale ?**

Pour savoir quelles données sont incluses dans une migration automatisée interrégionale, consultez Données incluses dans une migration automatisée interrégionale.

**Quelles données ne sont pas incluses dans une migration de données automatisée entre régions ?**

Une migration automatisée entre régions n'inclut pas les données suivantes :

- Applications et intégrations, y compris l'authentification unique (SSO) et SCIM, qui doivent être reconfigurées pour la nouvelle région
- Enregistrements
- Les notifications dans l'application sont effacées

**Y a-t-il un coût supplémentaire ?**

Oui. Une migration automatisée entre régions est un service payant offert par Miro Services. Pour plus de détails, veuillez contacter votre interlocuteur Miro.

**Comment Miro garantit-il la suppression des données de mon organisation de la région source ?**

Pour supprimer vos données de la région source après une migration inter-régions, Miro suit le protocole suivant :

- Les données restent dans la région source pendant 30 jours pour garantir qu'une sauvegarde fiable est disponible en cas de problème avec la migration.
- Après 30 jours, Miro commence à supprimer vos données de la région source.
- Au bout d'un maximum de 120 jours après la date de migration initiale, Miro a supprimé toutes les données de la région source.

**Que voient les utilisateurs lors d’une migration interrégionale ?**

Pour en savoir plus sur l'expérience utilisateur pendant une migration, consultez [Expérience utilisateur lors du transfert de données entre régions](../../canvas-25-admin-features/data-residency/04-user-experience-while-moving-data-between-regions.md).

**Que se passe-t-il si la migration échoue ?**

Si la migration échoue pour une raison quelconque, Miro rétablit l'accès à votre région d'origine et coordonne une nouvelle date pour retenter la migration.
