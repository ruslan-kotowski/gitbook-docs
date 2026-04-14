---
title: "Aper\xE7u du blocage des prompts (b\xEAta)"
article_id: 29332642230546
translation_id: 29332642230546
locale: fr
sidebar_position: 4
created_at: '2025-09-09T07:58:00Z'
updated_at: '2026-01-12T11:23:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Le blocage des prompts permet aux admins de contenu sensible d'empêcher les utilisateurs d'envoyer des prompts d'IA contenant des informations sensibles, vous aidant à garder les données sensibles en dehors de Miro IA au sein de votre organisation. Miro analyse le texte qu'un utilisateur saisit dans le champ de prompt et tout contenu textuel qu'il ajoute depuis le tableau. Si ce contenu correspond aux étiquettes de sensibilité ou aux modèles de code source sélectionnés dans la configuration du blocage de prompt, Miro bloque l'envoi du prompt.

:::note
Seul le contenu textuel est pris en charge dans la version bêta.
:::

## Fonctionnement

- Vous choisissez quelles catégories de badges bloquer au niveau de l'organisation. Les modifications prennent effet immédiatement pour tous les membres de votre organisation.
- Lorsque des données sensibles sont détectées dans un prompt, Miro IA affiche un message de politique dans le point d'entrée de l'utilisateur, le prompt est bloqué et ne peut pas être envoyé à Miro IA.
- Le blocage de prompt et le balayage de tableau sont différents. Le balayage de tableau localise le contenu sensible sur les tableaux et peut classifier automatiquement le tableau. Le blocage de prompt examine ce que les utilisateurs tentent d'envoyer à Miro IA.

## Ce qui est bloqué

- Badges liés à la confidentialité : Sélectionnez parmi tous nos badges de confidentialité intégrés, tels que SPII, HIPAA, identifiants, numéros financiers. Pour plus d’informations sur nos badges de confidentialité intégrés, consultez la [Référence des badges de confidentialité et des types d'informations](../../canvas-25-admin-features/data-discovery/06-sensitivity-labels-and-infotypes-reference.md).
- Analyse du code. Lorsqu'elle est activée, Miro bloque les prompts qui incluent du code source reconnu. Voir [Analyse du code](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md) pour plus de détails.

## Résultats typiques pour les utilisateurs

Lorsque l'utilisateur entre un prompt contenant des informations sensibles selon votre configuration :

- Les utilisateurs voient un message indiquant que nous ne pouvons pas générer ce contenu car il peut violer la politique de votre organisation.
- Le prompt n'est pas envoyé à Miro IA. Les utilisateurs peuvent modifier le prompt et essayer à nouveau.

## Analyse du code

L'analyse du code bloque les prompts IA qui incluent du code source reconnaissable. Cela nécessite un minimum de 5 lignes de code pour déclencher le blocage.

Par exemple :

```
function connect() {

  const token = "example-token";

  fetch("https://api.example.com/health");

  return true;

}
```

## Langues prises en charge

- C
- C#
- C++
- Go
- HTML
- Java
- JavaScript
- JSON
- PHP
- PowerShell
- Python
- Rust
- Script shell
- SQL
- TypeScript
