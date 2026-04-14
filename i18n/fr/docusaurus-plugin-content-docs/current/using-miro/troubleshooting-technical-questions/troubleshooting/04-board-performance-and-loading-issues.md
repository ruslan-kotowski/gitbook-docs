---
title: "Probl\xE8mes de performance et de chargement de tableau"
article_id: 360013588560
translation_id: 360013588560
locale: fr
sidebar_position: 4
created_at: '2020-05-06T08:17:24Z'
updated_at: '2025-04-01T16:57:11Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Découvrez des conseils pour améliorer les performances d'un tableau pendant les sessions collaboratives et sur les tableaux de grande taille, et pour résoudre les problèmes de lenteur et les pannes.

## Améliorer les performances d'un tableau

Un tableau peut ralentir pendant les **sessions collaboratives** avec un grand nombre d’utilisateurs, ainsi que dans le cas d’un **tableau de grande taille** contenant beaucoup de contenu.

Conseils pour les sessions collaboratives Conseils pour les tableaux de grande taille

Le nombre croissant d'utilisateurs sur un tableau et leur activité intensive peuvent impacter les performances du tableau.  Les utilisateurs dotés d’appareils plus anciens et moins puissants sont plus susceptibles de subir une baisse des performances./span>

**Si vous participez à une session collaborative, assurez-vous :**

- fermez ou réduisez tous les onglets et fenêtres superflus, si vous travaillez dans un navigateur de bureau [de bureau](../technical-guidelines/02-supported-browsers-browser-restrictions.md)
- masquer les curseurs des collaborateurs et fermer toutes les barres latérales
- d'éviter de sélectionner et de modifier plusieurs objets du tableau en même temps
- De minimiser la navigation dans le tableau
- D’utiliser le mode haute performance plutôt que le mode économie d’énergie si vous accédez à Miro depuis un ordinateur portable

**Si vous planifiez une session collaborative sur Miro :**

- Invitez les utilisateurs qui n’ont pas besoin d’éditer le tableau comme lecteurs.  Familiarisez-vous avec la configuration des [droits d’accès au tableau](../../sharing-boards/01-board-access-rights.md)
- Veillez à ce que le contenu du tableau soit bien structuré. Consultez les **Conseils pour les tableaux de grande taille** dans le deuxième onglet ci-dessus.

Le nombre maximum d’objets que vous pouvez ajouter sur un tableau est de 100 000.  Cependant, les performances peuvent être impactées à partir de 1 000 objets. Pour une meilleure expérience, nous vous recommandons de ne pas dépasser 5 000 objets.
Pour déterminer le nombre d’objets sur votre tableau :

- Sélectionnez tous les objets du tableau (ctrl-A sur Windows, cmd-A sur Mac, ou faites glisser une boîte de sélection autour de tous vos objets).
- Le menu contextuel s’affiche et indique le nombre total d’objets.
- Cliquez sur **Filter** (Filtre) pour voir le nombre d’objets par type.

![nombre d'objets.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/25736281544466_number-of-objects.gif)
*Mesurer le nombre d’objets sur un tableau*

Outre le nombre d’objets, les objets plus lourds ou plus complexes (notamment les fichiers et les tableaux chargés) peuvent également ralentir votre tableau.

Pour accélérer un grand tableau, gardez-le en ordre :

- Supprimez le contenu inutile, en particulier les fichiers et documents lourds (par exemple, les PDF vectoriels avec de nombreux détails ou les images haute résolution).
- Convertissez les fichiers PDF lourds et les images haute résolution en fichiers PNG/JPG et téléchargez-les de nouveau sur le tableau.
- Réduisez la taille du contenu de votre tableau s’il semble trop grand lorsque vous réalisez un zoom à 100 % :
  - Accédez à la carte dans le coin inférieur droit et définissez le zoom sur 100 %.
  - Si, à ce niveau de zoom, votre contenu semble trop grand, sélectionnez-le en utilisant **Ctrl + A** (pour Windows) ou **Cmd + A** (pour Mac) et réduisez-le.
  - envisagez également de réduire l’échelle des images de grande taille
    **![redimensionner les tableaux.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/25736308553874_resize-board-objects.gif)**
    *Réduction d’échelle du contenu*
- [résoudre les commentaires](../../facilitation-tools/asynchronous-tools/01-comments.md)
- Convertissez les éléments réalisés avec [le stylo](../../essential-tools/10-pen.md) en images :
  - faites une capture d'écran d'un dessin
  - Téléchargez-la sur le tableau.
  - supprimez le dessin
- si cela est possible, divisez le tableau en plusieurs tableaux :
  - Copiez une partie du contenu du tableau en la sélectionnant et en appuyant sur **Ctrl + C** (Windows) ou **Cmd + C** (Mac).
  - [Créez un nouveau tableau](../../../getting-started/start-here/your-first-board/01-create-a-miro-board.md) et collez-y le contenu.
  - Supprimez le contenu copié du tableau d’origine.

## Résoudre les problèmes de mauvaises performances ou de chargement sans fin

Votre appareil, votre connexion Internet, votre navigateur et d'autres facteurs peuvent influencer les performances d'un tableau et la vitesse de chargement.  Si vous rencontrez de mauvaises performances, ou si votre tableau ou tableau de bord ne se charge pas sur un navigateur, une application de bureau, une tablette ou un appareil mobile, essayez les étapes de dépannage proposées.

:::warning
Avant d’explorer les solutions ci-dessous, consultez la [Miro Status Page](https://status.miro.com/) (page de statut de Miro) pour prendre connaissance des informations disponibles concernant la dégradation des performances.
:::

Navigateur Application de bureau Tablette, mobile

1. 1. Ouvrez Miro en mode incognito/span> [(privé)](https://support.google.com/chrome/answer/95464) **et/ou dans un** navigateur différentSi Miro fonctionne en mode incognito ou dans un navigateur différent, supprimez le cache et les cookies de votre navigateur.

**Effacer les données de site Miro dans Chrome**

1. Rendez-vous sur https://miro.com/ et ouvrez les /span>[Developer tools (Outils de développement)](https://miro.com/) de Chrome (**Commande + Option + J****sur Mac***,* Ctrl + Maj + J **sur Windows***)*. Choisissez l’onglet **Application (Appli) > Storage (Stockage)**. Cliquez sur **Clear site data.**​ Cela devrait supprimer toutes les données Miro enregistrées dans votre navigateur Chrome, et vous pouvez démarrer une nouvelle session. Veuillez noter que vous serez déconnecté de votre profil Miro.![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)*L'option pour effacer les données du site dans Chrome*

Vous devrez peut-être également mettre à jour le navigateur vers la dernière version ou désactiver certaines extensions. Veuillez consulter la liste des [navigateurs pris en charge](../technical-guidelines/02-supported-browsers-browser-restrictions.md).

2. Vérifiez votre **connexion Internet**. Si la bande passante de votre réseau n’atteint pas le minimum demandé de 8 Mb/s, passez sur un autre réseau, de préférence plus rapide.

3. Assurez-vous que votre appareil répond aux [**exigences système**](../technical-guidelines/01-system-requirements.md) :

- CPU - 3 GHz (2 cœurs/4 threads)
- Mémoire RAM - 8 Go

4. Si vous accédez à Miro depuis un ordinateur portable, assurez-vous d’être **en mode** haute performance/span> en non en mode économie d’énergie.

5. 5. Si vous rencontrez un problème avec des tableaux spécifiques, essayez [de les dupliquer](../../managing-boards/03-how-to-duplicate-a-board.md)/span> **afin de déterminer si le problème persiste dans le tableau copié.** Pour les utilisateurs qui ne peuvent pas charger Miro et y accéder :

6. 6. Vérifiez que votre connexion prend en charge WebSockets. /span> Pour en savoir plus sur WebSockets et les étapes de dépannage, consultez Ajouter Miro aux applications autorisées.

7. Vérifiez si votre navigateur prend en charge **WebAssembly**. Miro s'appuie sur WebAssembly pour rendre le contenu du tableau. Si votre navigateur, vos extensions ou vos paramètres de sécurité bloquent WebAssembly, il se peut que les tableaux ne se chargent pas. Pour vérifier si votre navigateur prend en charge WebAssembly, essayez d'ouvrir [cette page de test.](https://wasm.joway.io/) Si ce n'est pas le cas, consultez votre équipe informatique ou vérifiez les paramètres de votre navigateur pour vous assurer que WebAssembly est **autorisé**.

8. Vérifiez auprès de votre service informatique si votre entreprise utilise des pare-feux ou un proxy susceptibles de bloquer Miro. Suivez les instructions pour autoriser Miro ou fournir un contournement dans Ajouter Miro aux applications autorisées.

Si le problème persiste, [contactez le service d’assistance Miro](../../tools/troubleshooting/06-contacting-miro-support.md) et envoyez-nous [les journaux de la console du navigateur](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

1. Vérifiez si vous rencontrez des performances ralenties ou un chargement sans fin en utilisant une [**version Web**](https://miro.com/app/dashboard/). Si vous ne pouvez pas accéder à Miro depuis la version Web, essayez le guide de dépannage pour navigateur.
2. Si vous ne rencontrez aucun problème dans votre navigateur, **réinitialisez les données de l’application**.

   **Réinitialiser les données de l’application sur Windows**

   Appuyez sur Alt, cliquez sur **Help** (Aide) dans le coin supérieur droit, puis choisissez **Reset application data** (Réinitialiser les données de l'application) :

   ![reset_app_data_on_Windows.jpg](https://help.miro.com/hc/article_attachments/12305900586898)
   *Réinitialisation des données d’application sur l’application de bureau pour Windows*

   Si vous ne trouvez pas le menu, vous utilisez probablement l’application téléchargée depuis le MS Store. Dans ce cas, pour réinitialiser les données de l’application, ouvrez **les paramètres** Windows > **Applications**> Applications et fonctionnalités > recherchez Miro dans la liste > Options avancées > Réinitialiser.

   **Réinitialiser les données de l'application sous macOS**

   Lorsque vous êtes dans l'application Miro, cliquez sur **Help** (Aide) dans le menu supérieur et choisissez **Reset application data** (Réinitialiser les données de l'application) :

   ![reset_app_data_on_Mac.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695741458_reset%20app%20data%20on%20Mac.jpg)
   *Réinitialisation des données de l’application sur Mac*
3. Si le problème persiste, essayez de supprimer l’application et [**de la réinstaller**](https://miro.com/apps/).

Si vous rencontrez toujours des problèmes, [contactez le service d’assistance Miro](../../tools/troubleshooting/06-contacting-miro-support.md) et envoyez-nous [les journaux de la console de l’application](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

1. Vérifiez votre **connexion Internet**.  Si la bande passante de votre réseau n’atteint pas le minimum demandé de 8 Mb/s, passez sur un autre réseau, de préférence plus rapide.
2. Assurez-vous que votre appareil répond aux **exigences techniques** :

- Pour l’application Miro pour tablette :- 6 Go de RAM- iOS 12.0 ou version ultérieure, Android 6.0 ou version ultérieure, Windows 10 version 1607 ou ultérieure- Résolution d’écran de 768×1024 pixels ou plus
- Pour l’application Mobile de Miro :- iOS 12.0 ou une version ultérieure- Android 6.0 ou une version ultérieure

Supprimez l’application et **réinstallez-la** sur votre appareil.

**Pour les utilisateurs d’iPad :**veuillez noter que la dégradation des performances d'un tableau sur iPad peut être causée par les limitations en matière de RAM des iPad. Essayez ce qui suit :

1. Fermez toutes les applications d'arrière-plan inutiles avant d'utiliser Miro. Cela devrait améliorer les performances.
2. Travaillez sur des tableaux de plus petite taille. Cela devrait alléger la charge de l’application sur le système.
3. Passez vers un autre appareil (ordinateur portable ou de bureau) disposant de plus de RAM et utilisez la version pour navigateurs de Miro.

## Résoudre les problèmes courants

Synchronisation...  Merci de patienter Connexion rétablie/span>

La notification **Synching...**  Please wait (Synchronisation... Merci de patienter) signifie généralement qu’une charge lourde est en cours de traitement et que le processus manque de puissance pour la traiter dans le délai prévu. Le message peut donc apparaître si vous travaillez sur un tableau extrêmement lourd lors du déplacement en masse de nombreux objets, par exemple, ou en cas de perte de paquets. Notez que même si vos tableaux semblent relativement simples, pour Miro les objets lourds sont les images haute résolution, les fichiers PDF ou les dessins au stylo (ce sont des graphiques vectoriels difficiles à afficher) ou les tableaux. Ces éléments peuvent causer la dégradation des performances, ce qui déclenche le message.

Essayez de diviser le tableau en tableaux plus petits, en copiant et en collant votre contenu sur un nouveau tableau, et vérifiez si le problème persiste.  Si le problème persiste :

- Vérifiez que votre appareil répond aux exigences système minimales et que votre navigateur est à jour (version la plus récente).
- Si vous avez de nombreux onglets ouverts dans le navigateur, essayez de les fermer ou de les mettre en pause avant de travailler dans Miro, pour que votre navigateur puisse diriger toute sa puissance de traitement vers Miro sans la diviser entre de nombreux onglets.
- Testez Miro en mode Incognito (privé) (pour exclure la possibilité que des extensions de navigateur interférent) et dans un autre navigateur. Fermez tous les onglets du navigateur et les applications s’exécutant en arrière-plan si nécessaire.
- Videz le cache et les cookies de votre navigateur, redémarrez votre navigateur et forcez l’actualisation de la page en cliquant sur F5 (ou Ctrl/Cmd + R) plusieurs fois.
- Si vous rencontrez des problèmes avec des tableaux spécifiques, essayez de les dupliquer et vérifiez si le problème persiste sur les nouveaux tableaux. Vous pouvez également essayer d’ouvrir un tableau avec moins d’éléments ou un tableau plus petit pour voir si vous rencontrez le même problème.
- Si vous utilisez un VPN, vérifiez si le problème persiste lorsque vous le désactivez.
- Essayez de dupliquer le tableau et vérifiez si l’erreur persiste sur le nouveau tableau.

Généralement, la notification **Reconnecting...**, **Connection restored** (Reconnexion..., Connexion rétablie) s’affiche dans les cas suivants :

- Lorsqu’il y a des problèmes de connectivité de votre côté.  Assurez-vous que votre connexion réseau répond aux exigences minimales. Essayez de passer à un réseau plus rapide si possible.
- Lorsque vous travaillez sur plusieurs tableaux lourds ouverts dans le même navigateur.  Si cela semble être votre cas, fermez tous les autres onglets et les applications en cours d’exécution de votre navigateur et actualisez la page du navigateur.

Vérifiez également votre connexion WebSocket (en particulier si vous rencontrez des problèmes sur tous les tableaux, même les plus petits).  Contactez votre équipe informatique et demandez-lui d’activer les connexions WebSocket sur les ports 80 et 443 (SSL), et [vérifiez également si autre chose peut être la cause des problèmes](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)/span>.

## Foire aux questions

*Les performances du tableau dépendent-elles du plan que j’utilise (gratuit/payant) ?*

Non, les performances d'un tableau ne sont pas affectées par votre plan.

*Les paramètres de partage de mon tableau ont-ils une incidence sur les performances ?*

Les tableaux de partage ne devraient pas avoir d'incidence sur les performances du tableau, mais le nombre d'utilisateurs sur votre tableau peut les influencer. Vous pouvez utiliser les conseils ci-dessus pour les sessions collaboratives.
