---
title: Chiffres visuels dans les tables (bêta)
article_id: 31356870414610
translation_id: 31356870414610
locale: fr
sidebar_position: 18
created_at: '2025-11-25T19:40:55Z'
updated_at: '2026-03-13T12:26:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: tables
availability:
  notes: 'Qui peut le faire: Éditeurs de tableaux Quels forfaits: Business, Enterprise
    Quelles plateformes: Navigateur, Desktop, Mobile'
---

Visual Numbers permet aux utilisateurs de transformer des chiffres en barres de progression visuelles. Les utilisateurs peuvent définir des règles de mise en forme conditionnelle avec des couleurs personnalisées et définir des plages min/max pour une meilleure visualisation des données. Visual Numbers permet également une mise en forme en pourcentage ou en devise.

## Formater les nombres visuellement

La mise en forme numérique visuelle transforme des données numériques en barres de progression, facilitant ainsi l'identification des tendances et le suivi des progrès en un clin d'œil. Vous pouvez afficher les nombres sous forme de pourcentages ou de devises, définir des plages personnalisées et appliquer des règles de mise en forme conditionnelle.

Appliquez une mise en forme visuelle à un champ numérique :

1. Passez le curseur sur le nom du champ numérique ou de formule pour afficher l'icône des **trois points** (**...**).
2. Cliquez sur l'icône des **trois points** (**...**) et sélectionnez **Modifier le champ**.
3. Dans la section **Affichage** du dialogue, cliquez sur **Barre**.
   Les chiffres s'afficheront sous forme de barres de progression.
4. Choisissez votre format :
   1. Pourcentage (%): Idéal pour les taux de réalisation et le suivi de la progression.
   2. Devise : Sélectionnez parmi les principales devises ($, €, £, ¥, et plus).
5. Définissez la plage de **Min** et **Max** pour vos barres de progression. Pour les pourcentages, utilisez typiquement 0-100. Pour les devises, définissez des valeurs min/max appropriées pour vos données.
6. Choisissez une couleur de barre à partir du sélecteur de couleurs.
7. Activer ou désactiver les étiquettes numériques :
   1. Activé : Affiche la valeur numérique à côté de la barre de progression.
   2. Désactivé : Affiche uniquement la barre de progression pour une vue plus épurée.
8. Cliquez sur **Enregistrer**.

## Appliquer un formatage conditionnel

La mise en forme conditionnelle colore automatiquement vos barres de progression en fonction des règles que vous définissez, vous aidant à identifier rapidement les valeurs qui nécessitent une attention.

1. Ouvrez les **Paramètres de champ** pour un champ numérique ou une formule.
2. Activez les **Couleurs conditionnelles**.
3. Cliquez sur **Ajouter une règle**.
4. Définissez votre règle :
   1. Sélectionnez une condition (égal à, différent de, supérieur à, inférieur à, supérieur ou égal à, inférieur ou égal à, est vide, n'est pas vide).
   2. Entrez la valeur à comparer (si applicable).
   3. Choisissez une couleur pour les valeurs qui respectent cette règle.
5. Ajoutez plusieurs règles selon vos besoins. Glissez-déposez les règles pour définir leur priorité. Les règles en haut prennent le dessus.
6. Cliquez sur **Enregistrer**.

La mise en forme conditionnelle apparaît à la fois dans la vue table et dans le panneau latéral lors de la consultation des enregistrements individuels.

Le formatage visuel des nombres est actuellement disponible uniquement dans la vue table et le panneau latéral.

Les vues Chronologie, Kanban et Cartes afficheront le formatage numérique standard.
