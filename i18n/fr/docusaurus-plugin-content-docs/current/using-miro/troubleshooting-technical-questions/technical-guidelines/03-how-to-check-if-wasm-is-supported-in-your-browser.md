---
title: Comment vérifier si WASM est pris en charge par votre navigateur
article_id: 33769132852498
translation_id: 33769132852498
locale: fr
sidebar_position: 3
created_at: '2026-03-04T12:47:24Z'
updated_at: '2026-03-16T13:02:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Qui peut le faire: Tous les utilisateurs Quels forfaits: Free, Starter,
    Business, Enterprise, Éducation Quelles plateformes: Navigateur'
---

WebAssembly (WASM) peut être désactivé pour des raisons incluant la conformité avec les politiques de sécurité définies par votre organisation, ou l'absence de support dans les environnements plus anciens, par exemple.

> **ASTUCE :** Le [tableau comparatif de WebAssembly](https://webassembly.org/features/?categories=browsers) montre quelles fonctionnalités WASM sont prises en charge dans votre navigateur.

Vous pouvez vérifier si votre navigateur prend en charge WASM.

Suivez les étapes suivantes :

1. Ouvrez les outils de développement.
   - Dans votre navigateur :
     - (MacOS) Chrome, Edge, Firefox : `⌘ + ⌥ + I`
     - (Linux, Windows) Chrome, Edge, Firefox : `Ctrl + Maj + I`, ou `F12`
     - (MacOS) Safari : Allez dans **Réglages** > **Avancé**. Activer **Afficher le menu Développement dans la barre de menus** | **Afficher les fonctionnalités pour les développeurs web**. Ouvrir **Développement** > **Afficher la console JavaScript**.
   - Dans l'application de bureau Miro :
     - En haut à gauche, cliquez sur **Aide** > **Ouvrir les outils de développement**.
2. Dans les DevTools, cliquez sur l'onglet **Console**.
3. Dans la ligne d'entrée de la console, tapez ou collez `typeof WebAssembly`.
4. Sur votre clavier, appuyez sur **ENTRER**.
5. Interprétez le résultat :
   - Si la console renvoie `undefined`, alors WebAssembly n'est pas supporté ou est désactivé.
   - Si la console retourne `object`, alors WebAssembly est pris en charge.![](../../../../../../../docs/using-miro/troubleshooting-technical-questions/technical-guidelines/images/33770259460626_image.png)
     *La console DevTools affiche* `object` *lorsque WASM est disponible dans votre navigateur.*

     > **REMARQUE :** Si la console retourne `object` et que vous ne parvenez toujours pas à accéder à Miro, vous pouvez consulter d'autres [problèmes possibles et dépannage](../troubleshooting), ou contacter le [service d’assistance de Miro](../../tools/troubleshooting/06-contacting-miro-support.md).
