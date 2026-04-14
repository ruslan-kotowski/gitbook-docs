---
title: "Adicionar uma reten\xE7\xE3o legal a um caso"
article_id: 22120471564946
translation_id: 22120471564946
locale: pt-br
sidebar_position: 7
created_at: '2024-10-21T23:29:24Z'
updated_at: '2025-11-25T16:22:33Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
---

Criar uma retenção legal é um processo crítico para os [admins de eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) quando é esperado um litígio ou uma investigação. As retenções legais garantem que os boards relevantes da Miro sejam preservados e protegidos contra alteração, exclusão ou remoção. Isso é essencial para manter a conformidade com os requisitos jurídicos e regulatórios, evitar a perda ou modificação de dados importantes, além de proteger as principais evidências durante todo o processo jurídico. Uma retenção legal permite que os admins restrinjam o acesso aos dados, garantindo que todos os boards relevantes da Miro possam ser revisados sempre que necessário.

A criação de uma retenção legal envolve identificar os usuários e boards relevantes da Miro associados a um caso, bem como aplicar a retenção para proteger contra modificações. Os admins podem gerenciar várias retenções de um único caso, garantindo que todos os dados necessários sejam agrupados e preservados de maneira organizada. Este processo ajuda a manter a integridade e a responsabilidade dos dados, garantindo que a empresa esteja em total conformidade e devidamente preparada para o processo legal.

Os boards da Miro sob retenção legal podem ser acessados e editados, mas todas as versões são preservadas. Caso seja excluído, o conteúdo continuará disponível sob retenção legal. O número de itens de conteúdo sob retenção pode aumentar de acordo com as ações futuras dos usuários. Quando um board é colocado em retenção legal, todas as suas versões são mantidas por tempo indefinido, até que a retenção legal seja removida.

Para criar uma retenção legal, siga as seguintes etapas:

:::note
Você precisa ter a função de [admin de eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) para executar esta tarefa. Para solicitar a função de admin de eDiscovery, fale com seu Admin da empresa.
:::

1. Vá para suas configurações do Miro.
2. No painel esquerdo, em **Enterprise Guard**, clique em **eDiscovery**.
3. Na página **eDiscovery**, clique na guia **Casos**.
4. Na página **Criar caso**, clique no caso ao qual deseja adicionar uma retenção legal.
5. Clique em **Adicionar retenção legal**.
6. Na página **Adicionar retenção legal**, insira ou selecione as informações apropriadas em cada campo. A tabela a seguir lista cada campo e sua descrição.

   |  |  |
   | --- | --- |
   | **Campo** | **Descrição** |
   | Nome da retenção legal  **(obrigatório)** | Nome da retenção legal.  Tamanho máximo: 60 caracteres. |
   | Critérios  **(obrigatório)** | Tipo de conteúdo incluído nesta retenção legal. Esta versão é compatível apenas com todo o conteúdo. |
   | **Usuários titulares, cotitulares, que acessaram, modificaram ou criaram conteúdo**  **(obrigatório)** | Adicione os usuários que deseja colocar em retenção legal. Clique no campo para pesquisar por nome ou e-mail. Você pode adicionar até 200 usuários de uma vez.    **Notas:**  - Quando um usuário sob retenção legal abre, modifica ou interage com um board de qualquer forma (renomeando ou adicionando conteúdo), esse board é sinalizado e preservado. Por exemplo, se o nome do board for alterado ou o conteúdo for atualizado, esse board será automaticamente colocado em retenção legal. Além disso, a titularidade e a criação dos boards ficam sob retenção.  - Quando uma retenção legal é criada, ela se aplica aos boards que os custodiantes criaram, possuíam ou co-possuíam no momento da retenção. Além disso, todos os boards que os custodiantes acessem e modifiquem após a retenção também serão incluídos. As informações sobre o acesso ao histórico e atualizações do board não estão disponíveis nesta versão. |
7. Clique em **Avançar**. A página **Revisar impacto** será exibida.
8. Revise o impacto da criação desta retenção legal, como o número de boards existentes que serão retidos e os usuários titulares, cotitulares, que acessaram, modificaram ou criaram os boards.

   **Notas:**
   - Os boards sob retenção ainda podem ser acessados e editados, mas todas as versões serão preservadas. Caso seja excluído, o conteúdo continuará disponível em retenção. O número de itens de conteúdo sob retenção pode aumentar de acordo com as ações futuras dos usuários.

   - Quando um usuário sob retenção legal abre, modifica ou interage com um board de qualquer forma (renomeando ou adicionando conteúdo), esse board é sinalizado e preservado. Por exemplo, se o nome do board for alterado ou o conteúdo for atualizado, esse board será automaticamente colocado em retenção legal. Além disso, a titularidade e a criação dos boards ficam sob retenção.

   - Quando uma retenção legal é criada, ela se aplica aos boards que os custodiantes criaram, possuíam ou eram cotitulares no momento da retenção. Além disso, todos os boards que os custodiantes acessem e modifiquem após a retenção também serão incluídos. As informações sobre o acesso ao histórico e atualizações do board não estão disponíveis nesta versão.
9. Após revisar o impacto da retenção legal que você está criando, clique em **Adicionar retenção legal**.
   A página do caso aparece exibindo a retenção legal que ela contém e as informações sobre cada retenção legal, como o nome da retenção legal, o tipo de conteúdo afetado pela retenção, o número de usuários nessa retenção legal, a data em que a retenção foi criada, o status da retenção legal e o número de boards que estão sob retenção legal.
