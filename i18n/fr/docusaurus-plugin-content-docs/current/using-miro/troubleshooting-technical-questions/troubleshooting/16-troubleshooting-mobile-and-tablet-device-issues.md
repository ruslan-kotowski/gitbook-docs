---
title: "R\xE9solution des probl\xE8mes li\xE9s aux appareils mobiles et aux tablettes"
article_id: 360021113559
translation_id: 360021113559
locale: fr
sidebar_position: 16
created_at: '2021-04-16T08:25:42Z'
updated_at: '2025-11-25T16:04:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Si vous rencontrez des problèmes lorsque vous travaillez sur Miro depuis votre téléphone mobile ou votre tablette, tentez tout d’abord de *réinstaller l’application et d’actualiser votre appareil*.  Si le problème persiste, découvrez les raisons possibles ci-dessous.

| **Problèmes rencontrés sur un téléphone mobile** | | |
| --- | --- | --- |
| **Problème** | **Raison possible** | **Solution** |
| L’application mobile sur iOS plante et ne fonctionne pas correctement | La version iOS est trop ancienne | Veuillez mettre à jour votre version iOS ou utiliser un autre appareil. Notre application mobile pour iOS est prise en charge par les versions 12 et ultérieures |
| Je peux me connecter avec succès à l’application de bureau, mais sur mobile, l’application se bloque sur le logo Miro | Les données d’authentification sont corrompues (mauvais cache) | Accédez à **App settings (Paramètres de l’application) > Storage (Stockage) > Clear storage (Effacer le stockage)** ou réinstallez l’application Miro sur votre appareil |
| Je reçois l’erreur « Something went wrong » (Une erreur est survenue) lors de l’authentification par SSO sur l’application mobile | 1. 1. La connexion réseau est sécurisée et quelque chose bloque les requêtes  2. 2. Chrome est ajouté à la liste WIAsupportedUserAgents de l’ADFS et ne redirige pas l’utilisateur correctement/span>  3. 3. Il est possible que cet appareil spécifique ne puisse pas accéder à l’environnement SSO de l’entreprise | 1. 1. Essayez de vous connecter à partir d’un réseau différent et de l’autoriser  2. 2. Contactez votre admin système et demandez-lui de supprimer Chrome de la liste  3. Vérifiez auprès de votre service informatique s’il existe des restrictions quant aux appareils autorisés à utiliser l’authentification unique. |
| Je ne parviens pas à trouver les fichiers importés à partir des tableaux dans le système de fichiers de mon téléphone mobile | Lorsque vous téléchargez un fichier depuis un tableau sur mobile, il est « masqué » pendant un certain temps | Veuillez attendre jusqu’à ce que le fichier apparaisse dans le dossier des téléchargements |
| Lorsque je me connecte sur Miro sur mobile, je vois le message « No accounts available » (Aucun compte disponible) et je ne peux pas accéder à mon profil | Vous profil a été supprimé de vos équipes ou vous les avez [quittées](../../managing-your-profile/06-how-to-leave-a-team.md). | Veuillez vous connecter à Miro sur le bureau ou la tablette et créer une nouvelle équipe ou demandez à un autre utilisateur de vous inviter à une équipe Miro |
| Je ne peux pas modifier les tableaux Miro depuis un navigateur sur mobile | Il s’agit d’une limitation connue pour le moment | Veuillez passer sur l’[application mobile](../../../getting-started/apps-for-devices/08-mobile-app.md), l’application pour tablette ou l’application de bureau |
| Je ne peux pas exporter mon tableau depuis l’application mobile | Il s’agit d’une limitation connue pour le moment | Veuillez passer sur un autre appareil.  Apprenez-en plus sur l’exportation sur Miro sur [cette page](../../import-and-export/export/03-how-to-export-your-board.md). |

| **Problèmes rencontrés sur une tablette** | | |
| --- | --- | --- |
| **Problème** | **Raison possible** | **Solution** |
| La barre d’outils disparaît et l’application Miro présente un comportement bizarre sur iPad | Notre application utilise WebView pour faire le rendu des éléments visuels et l’une des règles liées à la gestion de la mémoire fait que le processus de rendu n’est pas autorisé à utiliser plus de 25 % de la mémoire RAM de l’appareil. Après cette marque, l’application devient limitée et cesse de se charger correctement sans donner de messages d’erreur ou de plantage | - Fermez toutes les applications inutiles fonctionnant en arrière-plan avant d’utiliser Miro. - Travaillez sur des tableaux de *plus petite* taille - Enfin, tentez d’ouvrir Miro sur *un autre appareil* (bureau) ayant une meilleure mémoire RAM |
| Je peux me connecter avec succès à l’application de bureau, mais sur la tablette, l’application se bloque sur le logo Miro | Les données d’authentification sont corrompues | Accédez à **App settings (Paramètres de l’application) > Storage (Stockage) > Clear storage (Effacer le stockage)** ou réinstallez l’application Miro sur votre appareil. |
| Le message d’erreur « Sorry, you cannot copy so many objects at once » (Désolé, vous ne pouvez pas copier autant d’objets en une seule fois) apparaît lorsque vous collez des objets sur iPad | Vous avez dépassé la quantité de données pouvant être mises en mémoire tampon sur l’iPad | Veuillez copier et coller moins de widgets en même temps |
| Je ne peux pas modifier [les documents Google Docs chargés sur mon tableau](../../../integrations-apps/google/05-google-drive.md) depuis ma tablette | Il s’agit d’une limitation connue pour le moment | Pour la contourner, vous pouvez ouvrir le document via l’application Google Docs en cliquant sur **l’icône** Source |
| J’utilise un Apple Pencil sur iPad.  Lorsque je tape deux fois sur l’écran pour passer de l’outil stylo à l’outil gomme et vice-versa, rien ne se passe | La fonctionnalité permettant de passer des outils plume à gomme et vice-versa en tapant deux fois l’écran est une fonctionnalité native prise en charge par la 2e génération des stylets Apple Pencil et non pas une fonctionnalité développée par Miro.  Elle est prise en charge dans l’application pour tablette uniquement | Veuillez vous assurer que votre Apple Pencil prend en charge cette fonctionnalité et passez sur [l’application pour tablette](../../../getting-started/apps-for-devices/11-tablet-app.md) |
| Les 2 choses suivantes ne fonctionnent pas sur iPad :   - Le zoom lorsque vous utilisez la molette de la souris - La navigation du tableau en balayant avec deux doigts sur le pavé tactile | Il s’agit d’une limitation connue liée aux restrictions de l’OS sur iPad | Malheureusement, aucune solution ne permet de résoudre ces problèmes pour le moment. |
