---
title: Configuration requise
article_id: 360017731553
translation_id: 360017731553
locale: fr
sidebar_position: 1
created_at: '2019-02-11T10:14:54Z'
updated_at: '2026-03-06T14:57:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Cet article décrit les exigences système pour utiliser Miro, y compris l'appareil, le GPU et WebAssembly.

Pour travailler dans Miro, assurez-vous que votre appareil répond aux exigences système minimales ou recommandées suivantes.

Cependant, veuillez garder à l'esprit que les paramètres mentionnés ci-dessous ne sont pas définitifs car les performances de Miro peuvent être liées à plusieurs autres facteurs tels que :

- Tâches en arrière-plan
- Nombre d’onglets dans le navigateur et fréquence de basculement entre eux
- Résolution du moniteur sur lequel vous ouvrez Miro
- Stabilité de la connexion Wi-Fi
- Nombre d’utilisateurs sur le tableau
- Système de refroidissement de l’appareil

Si vous rencontrez des problèmes de performance ou d'accès, veuillez consulter [les guides de dépannage](../troubleshooting) et les [astuces pour optimiser les performances du tableau](../../tools/troubleshooting/04-board-performance-and-loading-issues.md).

|  |  |  |
| --- | --- | --- |
|  | **Minimum** | **Recommandé** |
| **CPU** | 3 GHz (2 cœurs/4 threads) | 2,8 GHz (4 cœurs/8 threads) |
| **Mémoire RAM** | 8 Go | 16 Go (DDR4) |
| **Bande passante réseau** | 8 Mb/s | 32 Mb/s |

** Veuillez noter que l’exécution de Miro sur du matériel haut de gamme bien au-dessus des spécifications recommandées peut ne pas vous donner l’amélioration des performances attendue, car Miro est une application Web qui fonctionne à l’aide d’un moteur Web de navigateur. Le moteur Web n’est pas capable d’utiliser tout le potentiel de l’appareil comme un logiciel installé localement sur votre ordinateur et conçu pour un système d’exploitation et une architecture de processeur particuliers.*

Les exigences minimales du système pour une utilisation confortable de Miro sur [tablettes](../../../getting-started/apps-for-devices/11-tablet-app.md) sont de 6 Go de RAM.

Miro peut être utilisé sur différents types d’appareils. Vous pouvez ouvrir Miro dans un navigateur, télécharger l’[application de bureau](../../../getting-started/apps-for-devices/05-desktop-app.md), l’[application pour tablette](../../../getting-started/apps-for-devices/11-tablet-app.md), l’[application mobile](../../../getting-started/apps-for-devices/08-mobile-app.md), ou [utiliser Miro sur un écran interactif](../../../getting-started/apps-for-devices/07-interactive-displays.md).

**Mode hors ligne**

Étant donné que Miro s’appuie sur la vision d’une solution cloud transparente pour la collaboration *en ligne*, le mode *hors ligne* de l’outil n’est actuellement pas envisagé. Cependant, nous fournissons plusieurs options d'exportation. [En savoir plus](../../import-and-export/export/03-how-to-export-your-board.md).

## Exigences GPU et WebAssembly

Miro utilise l'accélération matérielle GPU et WebAssembly (WASM) pour un rendu fluide et pour prendre en charge certaines fonctionnalités avancées.

### Utilisation de Miro sans GPU

Pour des performances optimales, Miro nécessite l'accélération matérielle GPU.

Si l'accélération matérielle GPU n'est pas disponible, par exemple sur certaines machines virtuelles, ou lorsque l'accélération matérielle est désactivée, alors Miro passe automatiquement à un rendu basé sur le CPU.

:::tip
Pour profiter de l'expérience Miro optimale, laissez l'accélération matérielle activée lorsque cela est possible.
:::

Sans accélération matérielle GPU, vous pourriez rencontrer les changements de performance suivants :

- Certaines fonctionnalités dépendantes du GPU peuvent être indisponibles ou affichées comme des espaces réservés
- Un panoramique et un zoom plus lents, surtout pour les grands tableaux ou ceux contenant beaucoup de médias
- Les fonctionnalités principales du tableau peuvent ne pas se comporter comme prévu
- Une utilisation plus élevée du CPU

### Utiliser Miro sans WebAssembly (WASM)

Certaines fonctionnalités de Miro reposent sur des modules WebAssembly (WASM).

La plupart des navigateurs modernes activent WASM par défaut. Si WASM n'est pas disponible, par exemple bloqué pour respecter les politiques d'entreprise, désactivé dans le navigateur, ou non pris en charge dans des environnements plus anciens, Miro bascule automatiquement vers des chemins de rendu basés sur JavaScript lorsque cela est possible.

**Pour plus d'informations :** Consultez [Comment vérifier si WASM est pris en charge dans votre navigateur](https://help.miro.com/hc/articles/33769132852498).

:::tip
Pour une expérience optimale avec Miro, gardez WebAssembly activé. Dans un environnement géré, si vous suspectez que WASM est bloqué, vérifiez auprès de votre équipe IT.
:::

Sans WASM, vous pourriez constater les changements de performance suivants :

- Les fonctionnalités nécessitant WASM peuvent ne pas s'initialiser et sont masquées ou affichées sous forme de substituts
- Les tableaux qui dépendent des fonctionnalités basées sur WASM peuvent ne pas se charger complètement ou pas du tout
