---
title: "Editar uma reten\xE7\xE3o legal"
article_id: 27968005251090
translation_id: 27968005251090
locale: pt-br
sidebar_position: 8
created_at: '2025-07-09T17:31:49Z'
updated_at: '2025-11-25T15:52:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
---

Editar uma retenção legal permite que os admins de eDiscovery ajustem e aprimorem os esforços contínuos de preservação legal à medida que os requisitos do caso evoluem. Seja pela identificação de novos responsáveis, pelo surgimento de boards da Miro adicionais que se tornam relevantes ou pela exclusão de boards ou usuários existentes do escopo, editar uma retenção legal assegura que os dados corretos permaneçam preservados e defensáveis ao longo do processo legal.

Os Admins podem atualizar o nome ou a descrição da retenção legal e adicionar ou remover usuários e boards conforme necessário. Essa flexibilidade dá suporte a fluxos de trabalho jurídicos dinâmicos e garante que a preservação permaneça precisa, atualizada e alinhada com o escopo da questão jurídica—mantendo a conformidade enquanto evita a retenção desnecessária de dados.

Quando uma retenção legal é editada:

- Os boards recém-adicionados à retenção começarão a ter suas versões preservadas a partir desse ponto.
- Boards ou usuários removidos da retenção deixarão de ser preservados, e suas versões não serão mais mantidas como parte dessa retenção legal.
- Os boards que permanecem sob retenção continuarão a ter todas as versões preservadas, incluindo quaisquer exclusões que ocorram após a aplicação da retenção.

Essa abordagem garante que as organizações possam responder às demandas legais com precisão e responsabilidade à medida que um caso evolui.

Para editar uma retenção legal, siga as seguintes etapas:

:::note
Você deve ter a [função de Admin de eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) para realizar esta tarefa. Para solicitar a função de admin de eDiscovery, fale com seu Admin da empresa.
:::

1. Vá para as configurações da Miro.
2. No painel esquerdo, em **Enterprise Guard**, clique em **eDiscovery**.
3. Na página **eDiscovery**, clique na guia **Casos**.
4. Clique no caso em que deseja editar uma retenção legal.
   A lista de retenções legais dentro do caso aparece.
5. Clique nas reticências (três pontos) na linha da retenção legal que deseja editar e clique em **Editar retenção legal**.
6. Na página **Editar retenção legal**, insira ou selecione as informações adequadas para cada campo. A tabela a seguir lista cada campo e sua descrição.

   |  |  |
   | --- | --- |
   | **Campo** | **Descrição** |
   | Nome da retenção legal  **(obrigatório)** | Nome da retenção legal.  Comprimento máximo: 60 caracteres. |
   | Critérios  **(obrigatório)** | Tipo de conteúdo incluído nesta retenção legal. Esta versão é compatível apenas com todo o conteúdo. |
   | **Usuários titulares, cotitulares, que acessaram, modificaram ou criaram conteúdo**  **(obrigatório)** | Adicione os usuários que deseja colocar em retenção legal. Clique no campo para pesquisar por nome ou e-mail. Você pode ter até 200 usuários por retenção legal, incluindo usuários adicionados em atualizações de retenção legal.  **Notas:**  - Quando um usuário sob retenção legal abre, modifica ou interage com um board de qualquer forma (renomeando ou adicionando conteúdo), esse board é sinalizado e preservado. Por exemplo, se o nome do board for alterado ou o conteúdo for atualizado, ele será automaticamente colocado em retenção legal. Além disso, a titularidade e a criação dos boards ficam sob retenção.  - Quando uma retenção legal é editada, ela se aplica aos boards que os custodiantes criaram, possuíam ou co-possuíam no momento da retenção. Além disso, todos os boards que os custodiantes acessem e modifiquem após a retenção também serão incluídos. As informações sobre o acesso ao histórico e atualizações do board não estão disponíveis nesta versão.  - Os boards recém-adicionados à retenção terão suas versões preservadas a partir do momento em que você salvar as atualizações de retenção legal na etapa 9.  - Boards ou usuários removidos da retenção deixarão de ser preservados, e suas versões não serão mais mantidas como parte dessa retenção legal.  - Boards que permanecem sob retenção continuarão a ter todas as versões retidas, incluindo quaisquer exclusões que ocorram após a aplicação da retenção. |
7. Clique em **Próximo**. A página **Revisar impacto** é exibida.
8. Revise o impacto da criação desta retenção legal, como:
   - O número de boards que permanecem sob retenção, serão liberados da retenção e adicionados à retenção.
   - Os usuários titulares, cotitulares, que acessaram, modificaram ou criaram os boards.
   Os critérios para a retenção.
   - A lista de boards que permanecem sob retenção.

   **Notas:**
   - Os boards sob retenção ainda podem ser acessados e editados, mas todas as versões serão preservadas. Caso seja excluído, o conteúdo continuará disponível em retenção. O número de itens de conteúdo sob retenção pode aumentar de acordo com as ações futuras dos usuários.

   - Quando um usuário sob retenção legal abre, modifica ou interage com um board de qualquer forma (renomeando ou adicionando conteúdo), esse board é sinalizado e preservado. Por exemplo, se o nome do board for alterado ou o conteúdo for atualizado, esse board será automaticamente colocado em retenção legal. Além disso, a titularidade e a criação dos boards ficam sob retenção.

   - Quando uma retenção legal é criada, ela se aplica aos boards que os custodiantes criaram, eram titulares ou cotitulares no momento da retenção. Além disso, todos os boards que os custodiantes acessem e modifiquem após a retenção também serão incluídos. As informações sobre o acesso ao histórico e atualizações do board não estão disponíveis nesta versão.
9. Após revisar o impacto da retenção legal que você está criando, clique em **Salvar retenção legal**.
   A página do caso aparece exibindo a retenção legal atualizada, como o nome da retenção legal, o tipo de conteúdo afetado pela retenção legal, o número de usuários nesta retenção legal, a data em que a retenção legal foi criada, o status da retenção legal e a quantidade de boards mantidos em retenção legal.
