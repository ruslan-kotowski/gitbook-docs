---
title: Airtable
article_id: 360012807619
translation_id: 360012807619
locale: pt-br
sidebar_position: 1
created_at: '2020-03-24T12:09:00Z'
updated_at: '2025-08-05T07:33:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Pessoas: Todos os usuários da Miro, usuários em planos pagos do Airtable
    Planos da Miro: Todos os planos Plataformas: Navegador'
---

Traga o poder da visualização em lousas para o seu trabalho ao usar o Airtable! Você pode exportar dados da Miro para o Airtable e incorporar boards da Miro em bases do Airtable para visualizá-los, comentá-los e editá-los diretamente dentro do Airtable.

## Exportar dados de boards da Miro para o Airtable

A integração Airtable Sync permite que você exporte dados (por exemplo, notas adesivas, cartões) de seus boards da Miro e os organize no Airtable. Para saber mais sobre como configurar e usar essa funcionalidade, visite a [documentação oficial do Airtable](https://support.airtable.com/docs/airtable-sync-integration-miro).

## Incorporar boards da Miro em bases do Airtable

### Instale o aplicativo da Miro no Airtable

:::warning
O aplicativo da Miro para Airtable **não** está disponível no navegador **Safari**.
:::

Os editores de base no Airtable podem instalar o aplicativo da Miro. Para fazer isso:

1. Abra sua base do Airtable e clique em **Extensões** no canto superior direito.

   ![Airtable extensions button in the top right corner.](../../../../../../docs/integrations-apps/more-integrations/images/21017651877394_Airtable%20extensions.jpg)
   *Botão de extensões no canto superior direito de uma base do Airtable.*
2. Clique em **Adicionar uma extensão**.

   ![Add an extension option in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017647938834_add%20an%20extension.jpg)
   *A opção de adicionar uma nova extensão.*
3. Procure por "Miro" no Marketplace do Airtable e clique em **Adicionar**.

   ![Miro app in Airtable Marketplace.](../../../../../../docs/integrations-apps/more-integrations/images/21017647933714_Miro%20in%20Airtable.jpg)
   *Aplicativo da Miro no Marketplace do Airtable.*

### Adicionar boards existentes da Miro a bases do Airtable

Depois que o aplicativo da Miro for adicionado à sua base do Airtable, clique em **Adicionar um board** na seção do aplicativo da Miro que aparece no painel de extensões.

![Add a Miro board button in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651876498_add%20a%20Miro%20board.jpg)
*Adicionando um board da Miro via o aplicativo da Miro no Airtable.*

Um seletor de boards da Miro aparecerá. Se você ainda não estiver conectado à Miro no seu navegador, será solicitado que faça login ou crie uma conta Miro.

Após selecionar um board, defina as permissões de compartilhamento de como ele aparecerá no Airtable, usando o menu suspenso. Você tem três opções:

- **Qualquer pessoa pode visualizar:** Qualquer pessoa no Airtable pode [visualizar](../../using-miro/sharing-boards/01-board-access-rights.md) o conteúdo do board incorporado.
- **Qualquer pessoa pode comentar:** Qualquer pessoa no Airtable pode [deixar comentários](../../using-miro/sharing-boards/01-board-access-rights.md) no board incorporado. (Nota: Esta opção não está disponível para boards armazenados na Miro [nos planos Free](../../plans-billing/miro-plans/09-free-plan.md).)
- **Privado:** O board seguirá suas configurações de compartilhamento existentes conforme configuradas na Miro.

  > ✏️ Para usuários do plano [Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md) da Miro, suas configurações de acesso seguirão os controles de acesso da organização, o que pode significar que algumas opções de compartilhamento estão restritas. Saiba mais: [Como gerenciar a política de compartilhamento do plano Enterprise para integrações incorporadas](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).

![Sharing settings options when adding a Miro board to Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651879826_board%20access%20in%20Airtable.jpg)
*Configurações de compartilhamento ao adicionar um board da Miro ao Airtable.*

O board da Miro incorporado aparecerá então em sua base do Airtable, onde você poderá visualizá-lo, comentá-lo ou editá-lo com base nas permissões configuradas.

![Embedded Miro board within an Airtable base.](../../../../../../docs/integrations-apps/more-integrations/images/21017651872402_Miro%20board%20in%20Airtable.jpg)
*Um board da Miro incorporado no Airtable.*

Para substituir um board inserido por outro, clique no ícone de engrenagem (**Configurações**) do aplicativo da Miro no Airtable, selecione **Escolher um board** e escolha outro board no seletor da Miro.

![Replacing an embedded Miro board in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017647932690_replacing%20a%20board.jpg)
*Substituindo um board da Miro inserido no Airtable.*

### Criar novos boards da Miro a partir do Airtable

Para criar um novo board da Miro diretamente do Airtable:

1. Na seção do aplicativo da Miro dentro do Airtable, clique em **Adicionar board** (ou **Escolher um board** se um já estiver inserido e você estiver substituindo-o).
2. No seletor da Miro, selecione a opção para criar um **Novo board**.

![Creating a new Miro board from the picker within Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651880466_add%20a%20new%20board%20to%20Airtable.jpg)
*Criando um novo board da Miro a partir do seletor no Airtable.*

O novo board será criado na sua conta da Miro e incorporado em sua base do Airtable.

### Remover boards da Miro do Airtable

Para remover um board da Miro inserido da sua base do Airtable, você precisa remover ou reconfigurar a extensão do aplicativo da Miro dentro dessa base. Clique no menu suspenso no aplicativo da Miro no painel de extensões e escolha remover ou gerenciar a extensão.

![Deleting the Miro app from Airtable extensions panel.](../../../../../../docs/integrations-apps/more-integrations/images/21017647933074_deleting%20the%20app.jpg)
*Removendo o aplicativo da Miro do painel de extensões do Airtable.*
