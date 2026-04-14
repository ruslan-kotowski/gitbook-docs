---
title: Cotitulares de boards e Espaços
article_id: 360021580759
translation_id: 360021580759
locale: pt-br
sidebar_position: 6
created_at: '2021-05-12T07:36:28Z'
updated_at: '2026-01-06T19:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: board-roles-and-permissions
availability:
  notes: 'Quem pode fazer isso: Titulares de boards, cotitulares de boards, titulares
    de Espaços, cotitulares de Espaços, admins do time, Admins da empresa Quais planos:
    Business e Enterprise Quais plataformas: Navegador, desktop, dispositivo móvel'
---

A função de cotitular melhora a colaboração permitindo que os titulares de boards deleguem responsabilidades na preparação e facilitação do trabalho em um board, seja para sessões ao vivo ou assíncronas.

Um cotitular garante um fluxo de trabalho suave, mesmo se o titular principal do board estiver indisponível, pois cotitulares podem executar quase todas as ações de nível de titular, desde gerenciar configurações do board até controlar a visibilidade do conteúdo. Um cotitular ajuda a distribuir a carga de trabalho e fornece um backup confiável para o gerenciamento do board.

Para saber quais permissões um cotitular tem para um board ou Espaço, consulte a referência de cotitulares.

## Habilitar a função de cotitular para a organização

Como Admin da empresa, siga estas etapas:

1. No seu painel da Miro, clique no seu avatar no canto superior direito e clique em **Console de admin**.
2. Vá para **Segurança** > **Compartilhamento** > **Funções e permissões**.
3. Habilite a opção **Permitir a função cotitular**.

Admins podem agora habilitar a função de cotitular para seus times.

## Ativar a função de cotitular para um time

Como Admin da empresa ou admin do time, siga estas etapas:

1. No seu painel da Miro, clique no seu avatar no canto superior direito e clique em **Console de admin** | **Configurações**.
2. Vá para **Times** > **\{team name\}** > **Configurações**.
3. Em **Configurações de colaboração**, ative a opção **Ativar função de cotitular em boards e Espaços**.

## Adicionar cotitulares a boards

Como titular de um board, ou um cotitular existente, siga estas etapas:

1. No seu painel da Miro, faça um dos seguintes procedimentos:
   1. Para um board, clique nos três pontos (**...**) e clique em **Compartilhar**.
   2. Abra um board e clique em **Compartilhar** no canto superior direito.
2. Insira o endereço de e-mail dos usuários que você deseja adicionar como cotitulares.
3. Para seus direitos de acesso, clique em **É cotitular**.
4. (Opcional) Adicione uma mensagem personalizada.
5. Clique em **Enviar convites**.

:::note
Você pode atribuir a função de cotitular apenas aos membros do time. Para adicionar um cotitular de fora do time, primeiro convide-o para se juntar ao time.
:::

## Adicionar cotitulares aos Espaços

Como titular de um Espaço, ou cotitular existente, siga estas etapas:

1. No seu painel da Miro, faça um dos seguintes procedimentos:
   1. Para um Espaço na barra lateral, clique nos três pontos (**...**) e clique em **Compartilhar**.
   2. Abra um Espaço, depois clique na etiqueta no topo que mostra o número de membros.
2. Clique em **Gerenciar acesso**.
3. Para um membro do Espaço, atualize seus direitos de acesso para **cotitular.**

:::note
Você pode atribuir a função de cotitular apenas aos membros do Espaço. Para adicionar um cotitular de fora do Espaço, primeiro convide-o para participar do Espaço.
:::

> Um cotitular de Espaço tem permissões de editor para todo o conteúdo dentro desse Espaço.

## Referência de cotitulares

### Permissões de cotitular do board

Além de todas as permissões de Editor, um cotitular do board tem as seguintes permissões:

- **Gerenciar configurações de conteúdo do board e configurações de ferramentas de colaboração**
  Controle quem pode copiar o conteúdo do board e gerenciar ferramentas como o cronômetro, votação, videoconferência, compartilhamento de tela e gerenciamento de atenção
- **Oculte e revele quadros**
  Controle a visibilidade do conteúdo do quadro durante apresentações ou workshops.
- **Adicionar bloqueio protegido**
  Evitar o movimento ou a exclusão acidental de conteúdo durante a colaboração.
- **Adicionar senha ao board**
  Proteja os boards públicos exigindo uma senha para acesso.
- **Baixar um backup do board**
  Crie cópias arquivadas dos boards. Cotitulares também podem restaurar boards a partir de backups.
- **Adicionar cotitulares**
  Conceder status de cotitular a outros usuários.
- **Alterar os detalhes do board**
  Alterar a capa e renomear o board
- **Compartilhe o board**
  Modifique os direitos de acesso do time e de outros usuários no board
- **Configurar permissões avançadas de compartilhamento do board**
  Especifique se o board pode ser compartilhado fora do time ou da organização

:::note
Nos planos Enterprise, cotitulares de boards e admins de conteúdo podem mover boards usando a [API REST da Miro](https://developers.miro.com/reference/update-board), que difere intencionalmente da experiência da Miro UI, onde apenas titulares podem mover seus boards.
:::

Um cotitular do board não pode realizar as seguintes operações:

- Excluir o board
- Mova o board para outro time.
- Alterar o titular do board

### Permissões de cotitular do espaço

Além de todas as permissões de Editor, um cotitular de Espaço tem as seguintes permissões:

- Renomear o Espaço
- Compartilhe o Espaço
- Modifique os direitos de acesso do time e de outros usuários no Espaço
- Adicionar cotitulares ao Espaço

Um cotitular do Espaço não pode realizar as seguintes operações:

- Excluir o Espaço
- Alterar o titular do Espaço

## Perguntas frequentes

**Não tenho a opção de atribuir um cotitular. Por quê?**

O recurso de cotitular está disponível nos planos Business e Enterprise. O Admin da empresa deve ativar este recurso nas configurações do time ou da empresa. Somente os membros existentes do time podem ser promovidos para cotitulares. Certifique-se de que o usuário foi convidado para o board por e-mail antes de tentar atribuir a função de cotitular.

**Sou admin com permissões de admin de conteúdo habilitadas. Por que não consigo adicionar cotitulares do board?**

Admins com permissões de admin de conteúdo (CAP) precisam primeiro se adicionar como titulares no board específico. Assim que se tornam titulares de um board, eles podem então atribuir cotitulares.

**Devo pagar adicionalmente pelos cotitulares convidados para meus boards?**

Somente os membros existentes do time podem ser designados como cotitulares. Se o usuário que você deseja tornar cotitular ainda não faz parte do seu time, primeiro será necessário convidá-lo para o time, o que pode envolver a compra de uma licença adicional, dependendo do seu plano e contagem atual de usuários. Depois de se tornarem membros do time, você pode atribuir a eles a função de cotitular.
