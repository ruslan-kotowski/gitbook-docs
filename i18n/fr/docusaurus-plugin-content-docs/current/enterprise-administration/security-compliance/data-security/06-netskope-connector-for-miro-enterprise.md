---
title: Connecteur Netskope pour Miro Enterprise
article_id: 4415711060498
translation_id: 4415711060498
locale: fr
sidebar_position: 6
created_at: '2022-01-19T06:23:42Z'
updated_at: '2025-02-26T11:27:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Le connecteur personnalisé Miro pour Netskope permet d’obtenir de la visibilité sur les événements liés aux fuites de données et permet de gérer le trafic suivant dans Miro :

- [Téléchargement des sauvegardes de tableau](../../../using-miro/import-and-export/export/05-how-to-save-board-backup.md)

Ce guide vous explique comment configurer Netskope pas-à-pas pour les plans Enterprise Miro et décrit l’expérience utilisateur.

> **Disponible pour** : [Plan Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md)

### Créer une nouvelle application Miro dans Netskope

Dans votre instance Netskope, allez dans **Settings (Paramètres) > Security Cloud Platform (Plateforme cloud de sécurité) > App Definition (Définition d’application)** et cliquez sur **NEW CLOUD APP** (Nouvelle application de cloud) :

new_cloud_app.jpg
![Création d’une application cloud dans Netskope](blob:https://miro.atlassian.net/8cb061a4-e184-4bd6-bb95-774cd34fc8e7#media-blob-url=true&id=78b7a8cb-792a-41da-bf16-b26ca4480059&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.08.43.png&size=181298&height=513&width=1028&alt=)

Pour créer une nouvelle application dans Netskope, vous devrez importer le fichier JSON suivant **miro-activities-for-netskope.json** :

```
Version : 0.0.0.1.

"domain_name" : "miro.com",
"uri_path" : "/api/v1/ tableaux/.+/",
"http_method" : OBTENIR
"uri_param" : [{"key" : "archive", "value" : "true" }],
"resp_code" : 200.
"pattern" : "",
"nom_de_l'activité" : télécharger


"domain_name" : "miro.com",
"uri_path" : "/api/v1/ tableaux/.+/resources/.+/files/original",
"http_method" : OBTENIR
"uri_param" : [],
"resp_code" : 307.
"pattern" : "",
"nom_de_l'activité" : télécharger
```

Entrez le nom de l’application, sélectionnez l’option **Custom Connector** (Connecteur personnalisé) et cliquez sur **IMPORT FROM FILE (Importer à partir du fichier) > Add To Activity List (Ajouter à la liste d’activités)** pour charger le fichier **miro-activities-for-netskope.json** téléchargé à l’étape précédente**.**

uploading_the_file.jpg
Chargement du fichier

Une fois le fichier **miro-activities-for-netskope.json** importé, les activités enregistrées seront affichées. Vous pouvez désormais poursuivre en cliquant sur **SAVE** (Enregistrer) pour créer l’application Miro.

save_the_app.jpg
![Enregistrement de l’application](blob:https://miro.atlassian.net/b9da4e19-b3b1-4c25-aed3-762f458fd639#media-blob-url=true&id=f7549007-0265-42e1-b946-a3e167124f12&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.26.58.png&size=209044&height=693&width=1028&alt=)

Une fois l’application créée, vous devez la sélectionner et cliquer sur **APPLY CHANGES** (Appliquer les modifications).

apply_changes.jpg
/strong>L’option permettant d’appliquer les modifications à l’application Miro

![](blob:https://miro.atlassian.net/82b8ac6e-1952-44e7-a62f-cefb7dbee6ab#media-blob-url=true&id=975f42e8-de5d-4bbb-ae07-c243cce9bb2f&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.32.06.png&size=257154&height=575&width=1780&alt=)

### Créer une nouvelle Policy (Politique) pour votre application Miro dans Netskope

Une fois l’application créée, vous pouvez passer à la création d’une politique. Pour ce faire, rendez-vous dans la rubrique **Policy (Politique) > R****eal-time Protection (Protection en temps réel)** et cliquez sur **NEW POLICY (Nouvelle politique) > Cloud App Access (Accès à l’application cloud).**

create_a_policy.jpg
![Création d’une politique pour votre application Miro](blob:https://miro.atlassian.net/d2ae8479-8f5c-4417-8b09-2b57ee344d90#media-blob-url=true&id=e9c82ee5-cdea-4b33-8491-9613a848be81&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.39.02.png&size=107320&height=321&width=635&alt=)

Dans **Destination,** vous devez partager l’application Miro que vous avez créée à l’étape précédente, configurer un **Policy Name (Nom de politique)** et cliquer sur **SAVE (Enregistrer)**.

save_the_policy.jpg
/strong>Enregistrement de la politique

![](blob:https://miro.atlassian.net/abf26593-27ad-40f4-b3e5-731a9e58d062#media-blob-url=true&id=0edd2e23-2762-4173-8f3f-9a7bb74bf217&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.45.14.png&size=200430&height=722&width=1575&alt=)altVous pouvez ensuite sélectionner l’emplacement où vous souhaitez placer la politique et cliquer sur altSAVE (Enregistrer).

move_policy.jpg
Sélection de l’endroit où vous préférez placer la politique

Enfin, vous pouvez appliquer les modifications en cliquant sur le bouton **APPLY CHANGES** (Appliquer les modifications).

applying_changes.jpg
Application des modifications

![](blob:https://miro.atlassian.net/41cdf802-aa1c-4f9a-bd22-950ea6ad755e#media-blob-url=true&id=7f85d987-6550-4271-90da-c9273a0cbc9a&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2019.29.17.png&size=157218&height=490&width=1576&alt=)

### Visualisation des événements

Une fois tous les éléments définis, vous pouvez visualiser le trafic en naviguant sur **Skope IT**, en filtrant l’application Miro personnalisée et en cliquant sur **See Events** (Voir les événements) comme suit.

see_events.jpg
L’option permettant de voir les événements de trafic

### Expérience utilisateur

Le client Netskope doit être installé sur l’ordinateur des utilisateurs pour lesquels les activités de téléchargement devraient être bloquées.  Lorsque les utilisateurs tentent d’effectuer un téléchargement de sauvegarde, Netskope bloque l’action et affiche un message dans une fenêtre contextuelle native du système d’exploitation.

alert.jpg
Un message affiché aux utilisateurs qui ne sont pas autorisés à télécharger une sauvegarde d’un tableau Miro
