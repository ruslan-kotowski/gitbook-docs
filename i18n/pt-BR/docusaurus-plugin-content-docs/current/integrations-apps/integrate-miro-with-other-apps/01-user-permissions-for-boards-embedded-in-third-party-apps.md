---
title: Permissões de usuário para boards inseridos em aplicativos de terceiros
article_id: 4411883577618
translation_id: 4411883577618
locale: pt-br
sidebar_position: 1
created_at: '2021-12-08T10:13:42Z'
updated_at: '2025-11-25T16:07:55Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
availability:
  notes: 'Pessoas: Titulares e cotitulares do board Planos: Todos os planos Plataformas:
    Navegador, aplicativo para desktop'
---

A Miro oferece diversas integrações que permitem a você colaborar facilmente com boards em ambientes de terceiros, como [Microsoft Teams](../microsoft), [Confluence](../atlassian/01-miro-for-confluence.md), Notion e Google Meet. Você pode descobrir outros aplicativos compatíveis no [Marketplace da Miro](https://miro.com/marketplace/category/embed-miro/). Ao incorporar boards, você pode definir diferentes níveis de acesso de usuário e gerenciar essas permissões dentro da Miro.

## Entenda o acesso de incorporação

Ao compartilhar um board em um aplicativo externo, você pode fornecer acesso de visualização, comentários ou edição especificamente para os usuários dentro desse aplicativo para uma colaboração única, independentemente do acesso deles à Miro. Esses usuários não precisarão de um perfil da Miro para acessar o board dentro do aplicativo. Isso permite que você defina direitos de acesso específicos ao board para usuários do aplicativo que não estão registrados na Miro sem tornar o board publicamente disponível.

Para segurança máxima, desaconselhamos o uso deste método fora de uma colaboração única (como um workshop) e recomendamos que sua organização aloque o acesso à Miro de forma adequada para aqueles que dele necessitam.

![embed_Miro_in_Zoom.gif](../../../../../../docs/integrations-apps/integrate-miro-with-other-apps/images/21020254296722_embed%20Miro%20in%20Zoom.gif) *Como configurar direitos de acesso para incorporação de board*

O board fica acessível apenas no aplicativo onde foi inserido. O nível de acesso que você define para um board inserido no aplicativo não afeta as configurações de compartilhamento do board fora do aplicativo. Por exemplo, se um [board privado](../../using-miro/sharing-boards/15-make-a-miro-board-private.md) estiver incorporado em um canal do Microsoft Teams com o acesso "Qualquer pessoa pode visualizar", os usuários nesse canal do Microsoft Teams poderão visualizar o board sem iniciar sessão na Miro. Se os mesmos usuários tentarem acessar o board fora do canal do Microsoft Teams seguindo o link do board, eles não terão acesso.

No entanto, observe que as configurações de compartilhamento do board definidas na Miro têm precedência sobre o nível de acesso definido no aplicativo externo. Por exemplo, se um board for [compartilhado publicamente na Miro](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), ele estará disponível para qualquer pessoa no Microsoft Teams, mesmo que você tenha incorporado o board como Privado.

## Gerenciar e revogar acesso de incorporação

Você pode facilmente rastrear, gerenciar e revogar o acesso a boards incorporados em aplicativos externos compatíveis.

Para gerenciar e revogar o acesso a boards incorporados:

1. Clique no botão **Compartilhar** para abrir as configurações de compartilhamento de um board da Miro.
2. Selecione **Configurações de compartilhamento**.
3. Abra a guia **Inserir**.
4. Você verá os aplicativos externos onde o board foi inserido, incluindo o nome da integração, quando e por quem foi inserido, e as configurações de acesso ao board dentro do aplicativo.
5. Para revogar o acesso ao board em um aplicativo, clique em **Revogar acesso** ao lado do aplicativo. Observe que esta ação é irreversível.

ol

![remove_an_access_link.gif](../../../../../../docs/integrations-apps/integrate-miro-with-other-apps/images/21020265344914_remove%20an%20access%20link.gif)
*Como remover um link de acesso*

Quando o acesso ao board inserido é revogado, o acesso ao board fica restrito no aplicativo. Observe que o board ainda pode estar acessível no aplicativo se for compartilhado pelo lado da Miro. Por exemplo:

- Se alguém tiver permissão para **editar** o board no aplicativo e o mesmo board tiver sido [compartilhado publicamente](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) com acesso de **visualização** pelo lado da Miro, qualquer pessoa poderá **visualizar** o board no aplicativo.
- Se o board for privado e compartilhado apenas [com outros usuários por e-mail](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), o board incorporado exigirá **login** para ser acessado no aplicativo.

## Regras e limitações de incorporação

Observe as seguintes regras e limitações ao incorporar boards:

- Você não pode incorporar um board se ele estiver [inativo](../../using-miro/tools/troubleshooting/15-the-board-is-locked.md) ou se seu acesso ao board for somente de visualização.
- Os boards salvos em [times do plano Free](../../plans-billing/miro-plans/09-free-plan.md) não podem ser incorporados com acesso de comentário.
- Para usuários do [plano Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), suas configurações de acesso seguirão os controles de acesso definidos para toda a organização, o que pode implicar que algumas opções de compartilhamento sejam restritas. Saiba mais: [Como gerenciar a política de compartilhamento do plano Enterprise para integrações incorporadas](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
- Para alguns links antigos, você verá apenas o nível de acesso e a aplicação, mas não quem criou o board ou quando foi inserido.
- Se você deseja limitar a capacidade de inserção de boards da Miro em aplicativos externos para sua organização com plano Enterprise, consulte o artigo [Como gerenciar a política de compartilhamento do plano Enterprise para integrações inseridas](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
- O gerenciamento de links de acesso ao board inserido ainda não é compatível com dispositivos móveis e tablets.

Saiba mais sobre o [acesso a board inserido para usuários com licenças gratuitas limitadas](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).
