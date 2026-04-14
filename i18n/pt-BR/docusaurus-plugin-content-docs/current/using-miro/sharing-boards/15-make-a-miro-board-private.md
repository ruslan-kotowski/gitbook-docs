---
title: Tornar um board da Miro privado
article_id: 360021095159
translation_id: 360021095159
locale: pt-br
sidebar_position: 15
created_at: '2021-04-15T11:55:31Z'
updated_at: '2026-01-06T19:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: board-roles-and-permissions
availability:
  notes: 'Quem pode fazer isso: Titulares de board Quais planos: Starter, Business,
    Enterprise e Education Quais plataformas: Navegador, Desktop, Dispositivo móvel'
---

Se você está iniciando um projeto individual ou deseja trabalhar em um board antes de compartilhá-lo com seu time, pode criar um board privado da Miro ou tornar privado um board compartilhado existente.

## Compreendendo boards privados

Os boards privados são boards que não são compartilhados com ninguém e são acessíveis apenas pelo titular do board. Este recurso está disponível nos planos Starter, Education, Business e Enterprise.

No plano Free, todos os boards criados dentro de um time são visíveis para todos os membros do time. Você pode ver quem está no seu time em suas [configurações do time](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md) na guia **Usuários ativos**. Se você quiser um board privado em um plano Free, deve ser o único membro desse time.

## Gerenciar privacidade do board

Você pode criar um novo board com acesso privado desde o início ou alterar as configurações de um board existente para torná-lo privado.

### Criar um novo board privado

Para garantir que um novo board seja privado desde o momento de sua criação, siga estas etapas.

1. **Para admins: Definir configurações de compartilhamento padrão (opcional).** Se você é um Admin da empresa ou do time nos planos Starter, Business, Enterprise ou Education, pode configurar todos os novos boards para serem privados por padrão.
   1. Vá para **Configurações do time** > **Permissões** > **Configurações de compartilhamento**.
   2. Em **Configurações padrão para compartilhamento do board**, escolha **Somente o titular do board pode acessar**.
      ![Default sharing settings in Miro.](images/21016134764434_default sharing settings.jpg)
      *Configurações de compartilhamento padrão*
2. **Verifique a localização do board.** Antes de criar seu board, certifique-se de que está na seção **Boards neste time** do seu painel. Se você criar um board dentro de um [Espaço](../spaces/01-spaces.md) compartilhado, o board será automaticamente compartilhado com todos os membros desse Espaço.
   > ✏️ Se você tiver um espaço privado que não é compartilhado com ninguém, pode criar seu board com segurança lá.
3. **Confirme as configurações de privacidade.** Após criar o seu board, abra a caixa de diálogo **Compartilhar**. Aqui você pode verificar se o board está [compartilhado com seu time](03-sharing-boards-and-inviting-collaborators.md). Se for o caso, defina o nível de acesso do time para **No Access**.
   ![Animação mostrando como remover o acesso do time a um board na Miro.](../../../../../../docs/using-miro/sharing-boards/images/21016134729874_7-1-720p-10fps-s4-r20.gif)
   *Como remover o acesso do time a um board*

### Tornar um board compartilhadoprivado

Para tornar um board existente privado em um plano Starter, Business, Enterprise ou Education, você deve remover o acesso de todos os colaboradores. Abra a caixa de diálogo **Compartilhar** e pare de compartilhar o board em todos os níveis:

- Definir acesso do time para **Sem acesso**.
- (No Enterprise) Defina o acesso da empresa para **Sem acesso**.
- Desabilitar qualquer link público (definido para **Sem acesso**).
- Se o board estiver em um espaço, mova-o para fora ou descompartilhe o espaço.
- Remova todos os usuários individuais listados em **Configurações de compartilhamento** até que apenas você (o titular) permaneça.

:::note
Se você **não** for o titular do board, mas precisar torná-lo privado, deve [convidar seu próprio e-mail](03-sharing-boards-and-inviting-collaborators.md) para o board antes de remover o acesso do time, espaço ou empresa. Se você não fizer isso, perderá o acesso ao board assim que alterar as configurações de compartilhamento.
:::

![Animação mostrando como definir um board compartilhado da Miro como privado.](../../../../../../docs/using-miro/sharing-boards/images/21016121409426_7-2-720p-10fps-s4-r20.gif)
*Como definir um board compartilhado da Miro como privado*

Você pode sempre [check quem tem acesso ao seu board](05-who-has-access-to-my-board.md) na janela **Compartilhar**.

## Perguntas frequentes

Por que meus boards ficaram bloqueados após o downgrade para o plano Free?

No plano Free, não é possível ter boards privados. Compartilhe o board com seu time para desbloqueá-lo. Mais informações neste artigo: [O board está bloqueado](../tools/troubleshooting/15-the-board-is-locked.md).

Vi a opção de fazer upgrade para tornar meu board privado. Meu board é público por padrão?

No plano Free, ele é compartilhado com todo o time por padrão. Isso se refere apenas ao fato de seus boards serem "compartilhados com o time" dentro do seu time Free.

Meus boards públicos podem ser encontrados online?

A Miro se esforça para evitar que os boards públicos sejam indexados por mecanismos de busca como Google ou Bing. No entanto, qualquer pessoa com o link pode acessar esses boards e o link pode ser compartilhado além do seu público-alvo. Dependendo do seu plano da Miro, você pode aumentar a segurança [definindo uma senha](13-password-protection-for-public-boards.md) para o seu board público.

Sou membro de um time gratuito e de um time pago. Posso mover meus boards do time gratuito para o pago para torná-los privados?

Sim, você pode [mover seus boards da Miro](../managing-boards/04-how-to-move-a-board.md).

Meus boards públicos podem ser duplicados?

Sim, se isso for permitido nas [configurações de conteúdo do board](14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md).

Quando compartilho um board publicamente, devo pagar pelos usuários que acessarão o board por meio do link do board?

Não, os visitantes poderão acessar o board gratuitamente. Saiba como você pode [compartilhar seus boards publicamente](08-collaboration-with-visitors.md).
