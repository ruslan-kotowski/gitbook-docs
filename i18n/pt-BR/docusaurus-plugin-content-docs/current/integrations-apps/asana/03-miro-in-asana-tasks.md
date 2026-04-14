---
title: Miro em tarefas Asana
article_id: 4420591454866
translation_id: 4420591454866
locale: pt-br
sidebar_position: 3
created_at: '2022-02-15T06:32:16Z'
updated_at: '2025-02-26T11:44:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: asana-cards
---

Principais funcionalidades:

- Adicione um board da Miro a qualquer tarefa Asana, criando um novo board ou adicionando seu board existente
- Facilite a anexação de uma board existente: quando o usuário começar a digitar o nome de uma board , ele verá uma lista de suas boards da Miro existentes
- Compartilhe automaticamente o board da Miro com os "colaboradores" na tarefa, enviando convites por e-mail e notificações de dentro do Asana

### Como instalar e autorizar o aplicativo da Miro no Asana

Autorize e instale o aplicativo da Miro do [Asana Marketplace](https://app.asana.com/-/install_platform_ui_app?app_id=1201153108289813).

![Miro_app_para_Asana.jpg](../../../../../../docs/integrations-apps/asana/images/21017653436434_Miro%20app%20for%20Asana.jpg)
*Clique em **Começar** depois de seguir o link*

Em seguida, selecione **Conectar ao Miro** e permita que o Miro acesse sua conta Asana.

![conceder_permissão.jpg](../../../../../../docs/integrations-apps/asana/images/21017653438354_grant%20permission.jpg)
*Permitir que o Miro acesse sua conta Asana*

Escolha um time para instalar o aplicativo e clique em **Instalar e autorizar**. O aplicativo será instalado para todos os membros da time, mas cada usuário da time precisará autorizar para anexar seus próprios boards da Miro às tarefas.

![instalar_aplicativo_Miro_para_Asana.jpg](../../../../../../docs/integrations-apps/asana/images/21017683076114_install%20Miro%20app%20for%20Asana.jpg)
*Selecionando um time*

Na próxima etapa, selecione os projetos Asana que você gostaria de conectar ao Miro.

Depois de instalar e autorizar o aplicativo, você poderá anexar boards desta time. Se você precisar anexar seus boards de **outras times** também, siga [este link](https://app.asana.com/-/install_platform_ui_app?app_id=1201153108289813) e instale o aplicativo para as times.

### Como anexar um board da Miro existente a uma tarefa Asana

:::warning
Você só pode anexar seus próprios boards armazenados na(s) time(s) onde o aplicativo foi instalado.
:::

1. Selecione a tarefa na qual você gostaria de anexar uma board da Miro.
2. Na seção de detalhes da tarefa, selecione o menu suspenso **Anexar board Miro** .
   ![anexar_um_quadro_Miro_à_tarefa_Asana.jpg](../../../../../../docs/integrations-apps/asana/images/21017683077266_attach%20a%20Miro%20board%20to%20Asana%20task.jpg)
   *Anexando um board da Miro a uma tarefa Asana*
3. Selecione **Anexar board existente**.
4. Encontre a board da Miro específica para importar diretamente do Miro pesquisando o nome da board . Você também pode colar o URL do board diretamente no formulário e selecionar **Adicionar**. Você pode anexar apenas suas próprias boards .
5. Se na janela Compartilhamento do board , a opção **Qualquer pessoa com o link pode ver/ comentar/editar** estiver ativada, o board será automaticamente compartilhado com todos os colaboradores atuais e futuros do Asana para esta tarefa.

:::warning
O recurso de compartilhamento automático será desativado se uma tarefa ficar inativa por mais de 30 dias. Os usuários ainda poderão [compartilhar manualmente o board no Miro](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).
:::

Seus colegas colaboradores receberão uma notificação por e-mail informando que você os convidou para o board da Miro.

:::warning
Observe que, se você remover um colaborador da tarefa do Asana, o acesso dele ao board anexado não será afetado. Então, se você quiser remover o usuário do board, você precisa [alterar o acesso dele nas configurações de compartilhamento do board no lado do Miro](../../using-miro/sharing-boards/01-board-access-rights.md).
:::

### Como criar um novo board da Miro em uma tarefa Asana

1. Selecione a tarefa na qual você gostaria de anexar uma board da Miro.
2. Na seção de detalhes da tarefa, selecione o menu suspenso **Adicionar board da Miro** .
3. Selecione **Criar novo board.
   ![anexar_um_novo_quadro_a_uma_tarefa_Asana.jpg](../../../../../../docs/integrations-apps/asana/images/21017683078162_attach%20a%20new%20board%20to%20an%20Asana%20task.jpg)***Criando um novo board da Miro de dentro do Asana*
4. Digite o nome do board desejado e convide colaboradores do Asana selecionando uma das opções de caixa de seleção. Você pode escolher convidar todos os colaboradores atuais da tarefa ou convidar automaticamente todos os futuros colaboradores da tarefa, o que inclui todos os colaboradores do Asana que interagem com a tarefa (por meio de postagens na seção de comentar ou sendo adicionados pelo criador da tarefa como colaborador).
5. Selecione **Criar board**.
   ![criando_um_quadro.jpg](../../../../../../docs/integrations-apps/asana/images/21017653442450_creating%20a%20board.jpg)
   *Criando um novo board da Miro de dentro do Asana*

Seus colegas colaboradores receberão uma notificação por e-mail informando que você os convidou para o board da Miro.
