---
title: 'Histórico do board: versões'
article_id: 360021668819
translation_id: 360021668819
locale: pt-br
sidebar_position: 12
created_at: '2021-05-17T11:56:55Z'
updated_at: '2026-01-06T19:02:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: activity-list
availability:
  notes: 'Quem pode fazer isso: Titulares do board, cotitulares, editores do board
    que são membros do time onde o board está localizado se tiverem permissão para
    copiar o conteúdo do board Quais planos: Starter,
    Business, Enterprise, Education Quais plataformas: Navegador, aplicativo para
    desktop, aplicativo para tablet'
---

Todas as versões dos seus boards da Miro são salvas automaticamente no histórico do seu board. Você pode revisar e restaurar as alterações a qualquer momento.

### Principais funcionalidades

- O backup dos boards é feito a cada hora, se houver alguma alteração, bem como no final de cada sessão colaborativa.
- As versões salvas do histórico do board são armazenadas por *90 dias*
- O board original *não* é alterado. A versão restaurada é criada como um board *separado* e seu título é datado por padrão.

:::warning
Ocasionalmente, problemas de rede imprevistos podem impedir que o backup de um board seja feito. Certifique-se de ter uma conexão de internet estável para fazer backups regularmente.
:::

### Restaurar uma versão anterior de um board

Para restaurar uma versão anterior:

1. Na barra do board, selecione os **três pontos** verticais.
   O **menu principal** é aberto.
2. Selecione **Board** > **Histórico**.
   O painel **Histórico** é aberto. A guia **Atividade** é aberta por padrão.
3. Selecione **Versões**.
4. Selecione uma versão.
   O modal **Restaurar como um board separado** é aberto.
5. (Opcional) Siga as instruções na tela.
6. Selecione **Restaurar**.

### Limitar ou desabilitar a restauração de versões anteriores do board

- A funcionalidade está disponível para [titulares](../sharing-boards/01-board-access-rights.md), cotitulares e pode ser habilitada para [editores](../sharing-boards/01-board-access-rights.md) que são membros do time onde o board está localizado
- A funcionalidade depende das [configurações de conteúdo do board](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md): a opção está disponível para membros do time apenas se o titular do board permitir que os membros do time copiem o conteúdo do board. Isso pode ser configurado no botão do board **Compartilhar** > **Configurações de compartilhamento** > **Permissões**
- [Permissões de admin de conteúdo](../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md) no [plano Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md) — quando habilitadas — permitem que os Admins da empresa acessem as **versões** do board mesmo quando desabilitadas pelas configurações de conteúdo ao [redefinir a titularidade do board para si mesmos](../sharing-boards/01-board-access-rights.md)

Se você não tiver permissão para usar a opção, verá a mensagem correspondente na guia **Versões**. Entre em contato com o titular do board para ter a funcionalidade habilitada.

## Perguntas frequentes

**Recentemente, eu [atualizei meu time](../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md). Posso restaurar uma versão do board que foi criada quando meu time estava no plano Free?**

Sim, após a sua atualização, você pode restaurar versões criadas enquanto estava no plano Free.

**Não tenho versões no histórico do board. Por quê?**

Observe que a funcionalidade não é suportada em [times gratuitos](../../plans-billing/miro-plans/09-free-plan.md). Além disso, certifique-se de que sua função no board permite que você restaure versões (você deve ser o [titular do board](../sharing-boards/01-board-access-rights.md), [cotitular](../sharing-boards/06-co-owners-of-boards-and-spaces.md) ou [editor](../sharing-boards/01-board-access-rights.md) e ser membro do time onde o board está localizado). Além disso, o titular/cotitular do board deve permitir que os membros do time copiem o conteúdo do board.
Se você excluiu um objeto, também pode restaurá-lo — confira [este guia](../working-on-the-board/18-restoring-board-content.md).
