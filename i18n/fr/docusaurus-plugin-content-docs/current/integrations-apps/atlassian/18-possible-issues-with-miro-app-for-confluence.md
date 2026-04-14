---
title: "\xC9ventuels probl\xE8mes de l\u2019application Miro pour Confluence"
article_id: 360021388500
translation_id: 8637993452562
locale: fr
sidebar_position: 21
created_at: '2022-11-18T11:41:35Z'
updated_at: '2025-02-26T11:23:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
---

Utilisez les conseils de dépannage ci-dessous si vous avez rencontré un problème lors de l’utilisation du [plugin Confluence](https://help.miro.com/hc/articles/360020712594).

|  |  |  |
| --- | --- | --- |
| **Message/problème** | **Causes éventuelles** | **Étapes pour résoudre le problème** |
| Vous avez un sélecteur Miro noir/blanc lorsque vous essayez de vous connecter à Miro ou d’intégrer des tableaux Miro dans des pages de Confluence. | Paramètres incorrects de navigateur | Allez dans les paramètres de votre navigateur et vérifiez que :   - La case à cocher **Prevent cross-site tracking** (Prévenir le suivi intersite) est désactivée. - La case à cocher **Block all cookies** (Bloquer tous les cookies) est désactivée :   mceclip0.png   - **Les fenêtres contextuelles** sur les sites de Miro & Atlassian sont autorisées :   mceclip1.png |
| Vous avez uniquement une autorisation de lecture sur le tableau et ne pouvez pas le partager ou l’intégrer.  **mceclip0.png** | Vous n’êtes pas éditeur/propriétaire du tableau. | Veuillez vous assurer que:   - Vous êtes éditeur ou propriétaire du tableau. - Vous disposez des autorisations nécessaires pour accéder à Miro dans votre navigateur avec les informations d’identification correctes. - Vous intégrez un tableau dans Confluence dans le même navigateur. |
| Après avoir intégré un tableau Miro, vous voyez apparaître le message suivant : "Miro demande l'accès à vos fichiers de cookies" | Votre navigateur ne permet pas de sauvegarder des cookies tiers | Pour activer l’intégretion, vous devez activer les cookies dans votre navigateur. Cela se produit principalement sur Mozilla et Safari. |
| Le tableau intégré affiche le message d’erreur « Your session has expired » (Votre session a expiré). |
| Lorsque vous essayez d'intégrer un tableau, vous obtenez le message suivant : "Vous n'êtes membre d'aucune équipe. Please log in to the full version of the product and create your team or let someone invite you to the existing one. » (Vous n’êtes membre d’aucune équipe. Veuillez vous connecter à la version complète du produit et créer votre équipe ou laissez quelqu’un vous inviter dans une équipe déjà existante.)  mceclip0.png | Vous n’êtes membre d’aucune équipe sous le profil Miro autorisé dans le navigateur. | Allez sur [Miro](https://miro.com/app/dashboard/) et créez une équipe. Si vous savez que vous êtes membre de certaines équipes dans Miro, veuillez ouvrir Miro sur un autre onglet du navigateur et assurez-vous que vous êtes autorisé avec le **bon e-mail** |
