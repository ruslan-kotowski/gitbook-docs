---
title: Como permitir ou restringir a cópia e exportação de boards e conteúdo
article_id: 360018350399
translation_id: 360018350399
locale: pt-br
sidebar_position: 14
created_at: '2020-12-14T06:10:03Z'
updated_at: '2026-01-22T14:23:08Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: export-pdf-canvas
availability:
  notes: 'Quem pode fazer: Membros do time, admins do time (Configuração), admins
    da empresa (Configuração) Quais planos: Starter, Business, Enterprise, Education
    Quais plataformas: Navegador, Desktop, Mobile'
---

Admins da empresa e Admins do time podem especificar se membros do time e não membros do time podem copiar o conteúdo dos boards e definir a configuração padrão de cópia para novos boards.

Titulares e cotitulares do board podem especificar as configurações de cópia para outros membros do time em um determinado board. Se os admins permitirem que não membros do time copiem boards, incluindo visitantes e convidados, então os titulares e cotitulares podem permitir que não membros do time copiem.

Se os admins não permitirem que não membros do time copiem conteúdos, então a opção de permitir cópia de boards por não membros do time é removida.

:::note
No plano Free, copiar boards é ativado por padrão e não pode ser modificado.
:::

## Como definir permissões de cópia de boards para um time

Para um determinado time, um Admin da empresa ou admin do time pode especificar se não-membros do time podem copiar e exportar boards e conteúdo, e definir as permissões padrão de cópia para boards recém-criados.

Siga estes passos:

1. Vá para o **Admin Console**.
2. Clique em **Teams**.
3. Clique na linha de **\{Team name\}**.
   Painel de **\{Team name\}** será aberto.
4. Clique para abrir a guia **Settings**.
5. Role até **Segurança de Conteúdo**.
6. Para **Copiar Conteúdo**, especifique se somente membros do time ou qualquer pessoa na organização pode copiar o conteúdo do board.
7. Especifique a **Configuração padrão para copiar conteúdo**. Os titulares dos boards podem modificar essa configuração para boards individuais.
   As suas configurações são salvas automaticamente.

:::note
Se copiar conteúdo do board não for permitido para não membros do time, a opção **Qualquer pessoa com acesso ao board** é removida das configurações do board. Por exemplo, visitantes e convidados estão proibidos de copiar o conteúdo.
:::

:::note
Não é possível copiar imagens entre boards privados conectados a times diferentes. Fale com o Admin da empresa da sua conta na Miro sobre como obter permissão para acessar o outro board para copiar imagens.
:::

## Como definir permissões de cópia para um board

Para um determinado board, o titular ou cotitular pode especificar quem pode copiá-lo.

Siga estes passos:

1. Em um board que você possui, co-possuí ou criou, clique no canto superior direito em **Compartilhar**.
   O modal de compartilhamento será aberto.
2. No canto inferior direito, clique em **Configurações de compartilhamento**.
3. Em **Quem pode copiar conteúdo do board**, especifique uma das opções.

   > ✏️ Se o Admin da empresa ou o admin do time desabilitar a opção **Qualquer pessoa com acesso ao board**, então a opção ficará indisponível.
4. Clique em **Concluído**.
   Suas alterações serão salvas automaticamente e aplicadas a todos que têm acesso ao board.

## Opções de cópia do board por tipo de usuário

Assumindo que **Qualquer pessoa com acesso ao board** pode copiar conteúdo, a tabela a seguir mostra permissões por tipo de usuário.

|  | Salvar board como template | Copiar conteúdo do board | Exportar | Duplicar | Baixar arquivos do board |
| --- | --- | --- | --- | --- | --- |
| Membros do time | ✔ | ✔ | ✔ | ✔ | ✔ |
| Convidados | ✘ | ✔ | ✔ | ✔ | ✔ |
| Visitantes com conta da Miro | ✘ | ✔ | ✔ | ✔ | ✔ |
| Visitantes sem conta da Miro | ✘ | (Com acesso de edição) ✔ | ✘ | ✘ | ✔ |

:::note
(Enterprise) Se [mover boards entre times não for permitido](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md), então a opção de duplicar um board estará indisponível.
:::

:::note
Observe que algumas opções não estão disponíveis para determinadas categorias de usuários mesmo se a pessoa titular do board permitir que qualquer pessoa com o link copie o conteúdo do board.
:::

## Perguntas frequentes

*Por que não posso copiar e colar conteúdo em um board da Miro?*

O titular ou cotitular do board pode não permitir cópias para sua função. Você pode ver sua função na barra de colaboração, no canto superior direito de um board da Miro. Entre em contato com o titular ou cotitular do board para solicitar permissões de cópia para sua função.

Você também pode querer garantir que tenha iniciado sessão na Miro. Se sua função tiver permissões de cópia e você estiver conectado, inicie sessão e abra o board em outro navegador e tente copiar.

*Por que a opção **Qualquer pessoa com acesso ao board** não está disponível para mim?*

Seu(s) Admin(s) da empresa ou admin(s) do time desabilitou essa opção. Se você é Admin da empresa ou admin do time, veja Como definir permissões de cópia de boards para um time.

*Como posso permitir que visitantes baixem arquivos enquanto restrinjo sua capacidade de copiar ou duplicar o board?*

Crie um board separado com os arquivos e, em seguida, ative a opção de copiar o conteúdo do board para qualquer pessoa com o link do board. Compartilhe o link do board com os visitantes.

Alternativamente, você pode inserir o novo board com os arquivos, e copiar habilitado para qualquer pessoa com o link, no board original. Para mais informações sobre incorporação, [Incorporar um board da Miro](../import-and-export/export/02-embed-a-miro-board.md).

*Por que não consigo encontrar **Permissões** no menu de **Compartilhamento** do board?*

(Pago) Somente o titular e o cotitular do board podem especificar permissões de conteúdo. (Free) As permissões de conteúdo não podem ser modificadas de seu padrão, que permite a cópia para todos os usuários.

*Posso especificar quem pode carregar conteúdo para o meu board?*

Qualquer pessoa com direitos de **pode editar** pode carregar conteúdo para o seu board.
