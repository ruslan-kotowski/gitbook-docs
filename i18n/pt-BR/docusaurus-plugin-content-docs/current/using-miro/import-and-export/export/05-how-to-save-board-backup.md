---
title: Salvando um backup de board
article_id: 360017572774
translation_id: 360017572774
locale: pt-br
sidebar_position: 5
created_at: '2019-02-11T10:14:51Z'
updated_at: '2025-12-02T10:14:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: export-pdf-canvas
availability:
  notes: 'Quem pode fazer isso: Titulares dos boards, co-titulares dos boards, Admins
    da empresa com [permissões de admin de conteúdo](../../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md)
    no [Enterprise Plan](../../../plans-billing/miro-plans/04-enterprise-plan.md)
    Quais planos: Starter, Business, Enterprise, Education Quais plataformas: Navegador,
    Desktop'
---

Crie cópias arquivadas dos seus boards ao salvar backups do board. Os backups permitem que você garanta a segurança do seu conteúdo e compartilhe cópias dos seus boards com outros usuários da Miro.

## Salvar um backup do board

Para criar um backup:

1. Abra o board e clique no ícone de **três pontos verticais** (![icon-main.svg](../../../../../../../docs/using-miro/import-and-export/export/images/27743904151698_icon-main.svg)).
2. Selecione o submenu **Board**.
3. Depois, selecione o submenu **Exportar**.
4. Escolha a opção **Baixar backup do board** e siga as instruções na tela.

![backup-entry-point.png](../../../../../../../docs/using-miro/import-and-export/export/images/21537453245330_backup-entry-point.png)
*Baixando backup do board*

Você também pode salvar um backup a partir do seu painel. Abra o menu do board clicando no ícone de **três pontos** (**...**) e selecione **Baixar backup do board** nas opções.

O arquivo **.rtb* será salvo no seu dispositivo.

:::warning
Observe que **somente titulares de boards** e cotitulares podem baixar os backups de boards localizados em **times pagos**. Se esta opção estiver desativada no menu Exportar, verifique se esta funcionalidade está [disponível no seu plano](../../../plans-billing/miro-plans/02-plans-and-features-available.md) e se você é o [titular do board](../../sharing-boards/01-board-access-rights.md) ou [cotitular do board](../../sharing-boards/06-co-owners-of-boards-and-spaces.md).
:::

## Como restaurar um board a partir de um backup

A opção de carregar um backup do board está disponível para qualquer usuário em times pagos. Você pode enviar uma cópia arquivada do seu board para outro usuário da Miro, para que ele possa recriar a cópia do board em seu time pago.

Para restaurar um board a partir de um backup:

1. No [painel](https://miro.com/app/dashboard/), clique em **Criar Novo**.
2. Selecione **Importar**.
3. Em seguida, selecione **Importar backup**.
   Uma caixa de diálogo aparecerá.
4. Escolha o seu arquivo de backup **.rtb*.
5. Depois de confirmar sua escolha, um novo board com o mesmo conteúdo será criado no time. O título do board incluirá **Restaurado**.

Após restaurar o board, você também tem a capacidade de mover o board para um espaço diferente dentro do seu time.

![backup-import.png](../../../../../../../docs/using-miro/import-and-export/export/images/21537453249938_backup-import.png)
*Restauração de um board a partir do backup*

## Solução de problemas

Observe que os downloads e os uploads de backup de boards são limitados. Para downloads, há um limite de **1GB**. Se o seu board for maior que isso, será necessário dividir o board em menores ou utilizar as [versões do board](../../managing-boards/12-board-history-versions.md) em vez dos backups baixados do board.

Quanto aos uploads, a interface da Miro pode carregar backups de boards com um máximo de **1GB**. Para carregar arquivos de backup maiores, entre em contato com a equipe de Suporte da Miro:

1. Faça login no Miro e envie sua solicitação [pelo formulário de suporte](../../tools/troubleshooting/06-contacting-miro-support.md).
2. Anexe seu arquivo de backup à sua solicitação ou carregue-o em qualquer armazenamento em nuvem e envie-nos o link (certifique-se de permitir que qualquer pessoa com o link possa baixar o arquivo).
3. Se o seu arquivo de backup for inferior a 1GB e ainda assim você tiver problemas para carregá-lo, verifique as etapas de solução de problemas [nesta página](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

Se você receber o erro: **Não é possível encontrar a cópia do recurso existente para o recurso otimizado 0** ao tentar carregar um backup, isso significa que o backup do board contém um recurso que precisa ser excluído. Você pode [enviar o arquivo .*rtb* para o Suporte da Miro](../../tools/troubleshooting/06-contacting-miro-support.md) para que possamos deletar os dados do recurso e garantir o sucesso no upload do backup.

:::note
Se tiver problemas ao salvar um backup, tente as etapas de solução de problemas deste [artigo](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).
:::

## Perguntas frequentes

**Não tenho a opção de baixar o backup do board. Por quê?**

Observe que apenas titulares de boards/co-titulares em times pagos ou Admins da empresa com [permissões de admin de conteúdo](../../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md) no [plano Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md) podem salvar backups de boards.

**O que fazer se meu board foi excluído?**

Confira este guia: [Como restaurar um board excluído](../../managing-boards/08-how-to-restore-a-deleted-board.md).

**Posso fazer backups de vários boards ao mesmo tempo?**

No momento, isso não é possível. Você precisará fazer backup de cada board individualmente.
