---
title: "Comment d\xE9sactiver les pop-ups de l\u2019application de bureau Miro dans\
  \ votre navigateur ?"
article_id: 360019244239
translation_id: 360019244239
locale: fr
sidebar_position: 5
created_at: '2021-01-29T12:48:31Z'
updated_at: '2026-03-06T13:37:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Si vous l’application [de bureau Miro](../../../getting-started/apps-for-devices/05-desktop-app.md) installée sur votre appareil, lors de l’ouverture Miro dans un navigateur, vous pouvez voir la pop-up qui suggère d’ouvrir le tableau dans l’application.

browser_pop-up.jpg
La fenêtre contextuelle du navigateur qui vous conduit sur l’application de bureau Miro

Si vous souhaitez désactiver la pop-up, veuillez suivre les instructions ci-dessous.

- Pour les utilisateurs de Mac
- Pour les utilisateurs de Windows
- Navigateur Safari

### Pour les utilisateurs de Mac

**Étape 1.** Supprimez (désinstallez) l'application bureau de votre ordinateur.

**Étape 2.** Annulez le paramètre "Toujours ouvrir l'URL dans l'application Miro" dans votre navigateur. Voici comment procéder dans Chrome et Firefox.

*Pour Chrome :*

1. Fermez toutes les fenêtres de Chrome et Miro avant de commencer (utilisez **C****md + Q** pour quitter le navigateur).
2. Ouvrez Finder sur votre Mac > appuyez sur les touches **Commande + Maj + G** > entrez le chemin suivant dans la zone de recherche : **~/Library/Application Support/Google/Chrome**. Ouvrez le dossier de votre profil Chrome, allez dans Preferences (Préférences).

   Il peut y avoir plusieurs dossiers avec le fichier, veuillez suivre les suggestions suivantes :

   - ouvrez et recherchez **Préférences** dans le dossier **par défaut**, si vous n’avez qu’un seul profil dans Google Chrome
   - Ouvrez et recherchez **Préférences** dans le dossier **Profile X**, si vous avez plusieurs profils dans Google Chrome, où **X** est un chiffre de la liste des profils.
   - ouvrir et rechercher **Préférences** dans chaque dossier (**par Défaut, Profil invité, Profil X**), s’ils existent
3. Ouvrez les **Préférences** dans un éditeur de texte.
4. Recherchez **`https://miro.com":\{"miroapp":true\}`**.
5. Supprimez **`https://miro.com":\{"miroapp":true\}`**.
6. Sauvegardez les modifications.
7. Redémarrez votre navigateur Chrome.

Si vous utilisez plusieurs profils Google, vous devrez modifier les Préférences dans chaque catalogue. Pour cela, à l’étape 2 vous devrez ouvrir **~/Library/Application Support/Google/Chrome** et modifier les **Préférences** dans les dossiers **de Profil 1**, Profil 2, etc.

*Pour Firefox :*

1. Ouvrez les paramètres du navigateur.
2. Dans la section **Générale**, faites défiler vers le bas jusqu’à **Applications.**
3. Trouvez **miroapp** et modifiez l’option **Use Miro** (default) (Utiliser Miro (par défaut)) en sélectionnant **Always ask** (Toujours demander) en sélectionnant l’option dans le menu déroulant.

### Pour les utilisateurs de Windows

**Étape 1.** Supprimez (désinstallez) l'application bureau de votre ordinateur.

**Étape 2 : Utilisez le script disponible via [ce lien](https://desktop.miro.com/platforms/Miro_DeleteAppSchema.reg) pour effacer la valeur du registre Windows*. Une fois cette opération effectuée, la notification ne devrait plus apparaître dans votre navigateur. Si la pop-up est toujours là, suivez l’étape 3.***

**Étape 3.** Annulez le paramètre "Toujours ouvrir l'URL dans l'application Miro" dans votre navigateur. Voici comment procéder dans Chrome et Firefox.

*Pour Chrome :*

1. Fermez toutes les fenêtres Chrome et Miro avant de commencer.
2. *N*aviguez vers **PC** > **Users (Utilisateurs) > \{current_user\} (utilisateur actuel) > AppData > Local > Google > Chrome > UserData > Default > Preferences.**
3. Ouvrez les **Préférences** dans un éditeur de texte.
4. Recherchez **`https://miro.com":\{"miroapp":true\}`**.
5. Supprimez **`https://miro.com":\{"miroapp":true\}`**.
6. Sauvegardez les modifications.
7. Redémarrez votre navigateur Chrome.

Si vous utilisez plusieurs profils Google, vous devrez modifier les Préférences dans chaque catalogue. Pour cela, allez sur **PC** > **Users (Utilisateurs) > \{utilisateur actuel\} > AppData > Local > Google > Chrome > UserData** et modifiez **Preferences** (Préférences) dans les dossiers **Profile 1, Profile 2** (Profil 1, Profil 2), etc.

*Pour Firefox :*

1. Ouvrez les paramètres du navigateur.
2. Dans la section **Générale**, faites défiler vers le bas jusqu’à **Applications.**
3. Trouvez **miroapp** et modifiez l’option **Use Miro** (default) (Utiliser Miro (par défaut)) en sélectionnant **Always ask** (Toujours demander) en sélectionnant l’option dans le menu déroulant.

### Navigateur Safari

Si vous avez besoin de désactiver la fenêtre contextuelle dans Safari, veuillez supprimer l’application de bureau Miro de votre appareil.
