---
title: "Afficher les r\xE9sultats de la recherche de donn\xE9es"
article_id: 15794382139154
translation_id: 15794382139154
locale: fr
sidebar_position: 16
created_at: '2023-12-15T15:47:29Z'
updated_at: '2025-11-25T15:40:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

Le cycle de découverte de données s'exécute au moins une fois par heure et analyse toutes les mises à jour des tableaux à la recherche d'informations relatives à la protection de la vie privée. Cela inclut les tableaux qui ont déjà été analysés lors du cycle précédent de recherche de données.

:::note
Pour visualiser les résultats de la recherche de données, vous devez avoir le [rôle d'administrateur de contenu sensible.](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) Pour demander le rôle d’admin du contenu sensible, contactez l’admin de votre entreprise.
:::

*![privacy_related_dd.png](images/24937489374226_privacy_related_dd.png)
Figure 1 : Résultats de la recherche de données*

Bien que nous travaillions en permanence avec notre partenaire technologique et nos clients pour améliorer le système de détection des contenus sensibles, nous ne pouvons pas garantir qu'il trouvera et signalera 100 % des données sensibles sur vos tableaux. Notre système de détection des contenus sensibles utilise des modèles et d'autres critères pour déterminer la probabilité d'une correspondance. Il peut arriver que le système signale par erreur des données sur vos tableaux comme étant probablement sensibles (faux positif) ou qu'il ne signale pas des données comme étant sensibles (faux négatif). Différents facteurs contribuent à ces occurrences, notamment la proximité de termes apparentés ou le formatage de données sensibles.

Pour plus d'informations sur la manière dont vous pouvez supprimer les résultats faussement positifs, reportez-vous à la section [Supprimer une correspondance avec un contenu sensible.](11-suppress-a-sensitive-content-match.md)

## Affichez les informations relatives à la dernière recherche de données effectuée

La section **Résultats de** la recherche de données affiche la date à laquelle la dernière recherche de données a été effectuée, représentée par le format de date Mois Jour, Année, et par le format de temps Heure:Minute AM/PM, avec une spécification de fuseau horaire (GMT+offset). Par exemple, 14 décembre 2023, 22:15 PM GMT+1 (Figure 1).

## Afficher les résultats de la recherche de données

La section **Résultats de la** recherche de données affiche des informations telles que le nom du règlement, une brève description, l'étiquette associée et le nombre de tableaux contenant un contenu potentiellement sensible susceptible d'entrer dans le champ d'application du règlement (figure 1).

Pour explorer les tableaux contenant des données très sensibles, cliquez sur le lien "Nombre de tableaux". L'explorateur de contenu s'affiche avec la liste des tableaux. Pour plus d'informations, reportez-vous à la section [Tableaux de révision contenant des données hautement sensibles](16-review-boards-with-privacy-related-information.md).
