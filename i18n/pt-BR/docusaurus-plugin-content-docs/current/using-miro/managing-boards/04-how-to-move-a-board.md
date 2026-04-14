---
title: Como mover um board
article_id: 360017730093
translation_id: 13643368194450
locale: pt-br
sidebar_position: 4
created_at: '2023-09-11T07:53:48Z'
updated_at: '2026-03-27T16:09:52Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
availability:
  roles: board_owner
  notes: 'Relevant for: All plans'
backstage_link:
  entity_kind: capability
  entity_id: move-board-to-space
---

> **Quem pode fazer:** titulares de boards
> **Relevante para:** Todos os planos

Todo usuário da Miro pode ser membro de vários times. Seu perfil da Miro é seu endereço de e-mail. Você pode mover um board da Miro de um time para outro ou transferir seu board da Miro para outro perfil.

:::note
Nos planos Enterprise, cotitulares de boards e admins de conteúdo podem mover boards usando a [API REST da Miro](https://developers.miro.com/reference/update-board), que difere intencionalmente da experiência na interface da Miro, onde apenas titulares podem mover seus boards.
:::

:::note
Os Admins da empresa no plano Enterprise podem [restringir a opção de mover boards para e de um time](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md) para todos os usuários não-admins e titulares de board.
:::

## Cenários comuns

Aqui estão vários cenários comuns que envolvem mover boards, juntamente com a seção deste artigo que explica como fazer isso:

- Você tem **dois perfis da Miro** (endereços de e-mail associados à Miro) e deseja mover os boards de um perfil para outro.
  *Siga as etapas em* [*desta seção*](04-how-to-move-a-board.md)*, usando a guia **Plano Free**.*
- Você fez **upgrade de um plano Free para um plano pago** e deseja mover os boards para o plano pago.
  *Siga as etapas em* [*desta seção*](04-how-to-move-a-board.md)*, usando a guia **Plano Free**.*
- Você quer **mover boards entre dois times pagos**.
  *Siga os passos nesta* [*seção*](04-how-to-move-a-board.md)*, usando a guia **Paid, Education plans**.*

## Como mover boards entre times

:::warning
Quando você move um board para outro time, seu [histórico de versões](12-board-history-versions.md) será perdido. Se deseja manter o histórico de versões, recomendamos [copiar o conteúdo do board](../working-on-the-board/09-copy-as-text-or-as-an-image.md) em vez disso.
:::

Para mover um board entre os times, é necessário:

- ser titular do board
- ser membro de ambos os times

Existem duas maneiras de mover um board para um time diferente: através do painel ou diretamente dentro do board.

### Como mover um board diretamente do board

1. Abra seu board e clique no ícone de três pontinhos (**...**) que fica logo à direita do nome do seu board (canto superior esquerdo)
2. Navegue para **Board > Mover para > Outro time![moving-board-three-dots.png](../../../../../../docs/using-miro/managing-boards/images/21537437708306_moving-board-three-dots.png)**

### Como mover um board usando o painel

1. Vá para o seu painel para ver todos os boards de um time.
2. Passe o mouse sobre o cartão do board que você deseja mover.
3. Clique nos três pontos e então clique em **Mover para time**.
   Uma caixa de diálogo se abrirá.
4. Selecione a organização para onde você deseja mover o board.
5. Selecione um time nessa organização.
6. Clique em **Mover**.

### Como mover um board para um Espaço diferente

1. Abra seu board e clique no ícone de três pontinhos (**...**) que fica logo à direita do nome do seu board (canto superior esquerdo)
2. Navegue para **Board > Mover para > Outro Espaço.** Você também pode optar por notificar os membros do time de que o board foi movido para outro Espaço.![moving-boards-spaces.png](../../../../../../docs/using-miro/managing-boards/images/21537453797394_moving-boards-spaces.png)*Movendo um board para outro Espaço*

### Acesso negado ao usuário

Se quaisquer colaboradores do board não fizerem parte do time para onde o board está se movendo, você verá uma mensagem de acesso negado.

Há duas maneiras de ver quais e-mails de usuários perderão o acesso ao board após movê-lo. Se o número de usuários for menor do que 10, você pode ver a lista de e-mails clicando em **Visualizar e-mails dos usuários** na **mensagem de acesso negado.** Se o número for maior do que 10, haverá um link para baixar a lista de e-mails.

Para garantir que todos os colaboradores mantenham acesso ao board, você pode [convidar membros para o novo time](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) antes de mover o board.

Você também pode escolher **Mover mesmo assim** e adicionar colaboradores ao board novamente depois que ele for movido.

![warning when moving a board.png](../../../../../../docs/using-miro/managing-boards/images/16759524012690_warning%20when%20moving%20a%20board.png)
*Mensagem de acesso negado ao mover um board de um time para outro*

**Se você mover um board para um time gratuito**, ele será compartilhado com todos os membros do time.

![private boards are not available in free teams.png](../../../../../../docs/using-miro/managing-boards/images/16759539790738_private%20boards%20are%20not%20available%20in%20free%20teams.png)
*Os boards privados estão indisponíveis em times gratuitos*

## Como mover boards entre perfis

Seu perfil na Miro é o endereço de e-mail com o qual você se cadastrou. Se acaso se cadastrou com dois e-mails diferentes, isso significa que você tem dois perfis. Você pode transferir um board de um perfil para outro.

### Como mover boards entre perfis

Planos pagos, Education Plano Free

Se o board estiver localizado em um time pago ou do Education e você quiser movê-lo para outro time pago ou do Education, basta salvar o backup do board e carregá-lo para esse time.

1. Abra seu painel.
2. Passe o mouse sobre o cartão do board que você deseja mover.
3. Clique nos três pontos.
4. Clique em **Download do backup do board**.
5. O arquivo .rtb será salvo no seu dispositivo.

   ![board-backup.png](../../../../../../docs/using-miro/managing-boards/images/23122136352530_board-backup.png)
6. Faça login no seu segundo perfil da Miro.
7. Alterne para o time onde você deseja mover o board.
8. Clique em **+ Criar novo** > **Importar** > **Importar backup**.
9. O seletor de arquivos será aberto.
10. Escolha o arquivo de backup .rtb que você salvou anteriormente e clique em **Abrir**. O board estará então disponível no seu painel.

    ![board-import-backup.png](../../../../../../docs/using-miro/managing-boards/images/23122136353682_board-import-backup.png)

Siga estas etapas se seu board estiver localizado em um time gratuito ou se precisar mover um board para um time gratuito.

1. Faça login na Miro com o perfil #1.
2. Compartilhe o board com o perfil #2. Clique em **Compartilhar**.
   ![free-sharing-board.png](../../../../../../docs/using-miro/managing-boards/images/23122136354066_free-sharing-board.png)
3. Digite o e-mail do perfil #2 > clique em **Enviar convites**.

   ![free-sharing-board-dialog.png](../../../../../../docs/using-miro/managing-boards/images/23122136354706_free-sharing-board-dialog.png)
4. Transfira a titularidade do board do perfil #1 para o perfil #2. Clique no botão **Compartilhar** > **Configurações de compartilhamento** > escolha o perfil #2 > selecione **Titular** no menu suspenso.
5. Faça login na Miro com o perfil #2, onde você verá o board.
6. Mova o board para outro time.

:::warning
Se seu segundo perfil estiver no plano Free e convidar seu perfil gratuito para um perfil pago, você usará uma licença desse seu plano pago. Se exceder o número de licenças do seu plano, você poderá receber a cobrança por uma licença extra.
:::

## Perguntas frequentes

**Por que não vejo a opção de mover para um time no menu do meu board?**

Somente titulares de boards que são membros de vários times podem mover os boards entre eles. Se você não é o titular do board, pode [duplicar o board](03-how-to-duplicate-a-board.md) (se isso for permitido nas [configurações de conteúdo do board](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md)) e mover a cópia do board.

A opção de mover boards também pode ser restrita por Admins da empresa no plano Enterprise.

**Como posso passar a titularidade do meu board para outro usuário?**

Saiba como [transferir a titularidade do board para outro colaborador](05-how-to-transfer-board-ownership.md).

**O link do board altera quando eu movo o board para outro time?**

Não, o URL do board não altera.

**Posso mover um board de template para o time de outro usuário?**

Sim, você pode pedir ao usuário para convidá-lo para o time dele e depois mover o board, ou [compartilhar o board](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) e permitir que ele [duplique o seu board](03-how-to-duplicate-a-board.md) nas [configurações de conteúdo do board](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md).

**Posso mover Espaços entre times?**

Não, você só pode mover boards separados.

**Posso mover vários boards em massa?**

Não, esta opção não está disponível no momento.

**Tento mover meu board e nada acontece ou aparece uma mensagem de erro. O que devo fazer?**

Tente mover o board em outro navegador ou no modo de navegação anônima. Você também pode tentar usar outra rede ou dispositivo.

Outra opção é [duplicar o board](03-how-to-duplicate-a-board.md) e mover a cópia do board. Se isso não ajudar, [reporte o problema ao Suporte Miro](../tools/troubleshooting/06-contacting-miro-support.md).
