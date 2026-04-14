---
title: "Vis\xE3o geral da reten\xE7\xE3o legal"
article_id: 21922434361618
translation_id: 21922434361618
locale: pt-br
sidebar_position: 1
created_at: '2024-10-11T12:20:34Z'
updated_at: '2025-11-25T15:48:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
---

A funcionalidade de retenção legal foi criada para atender aos processos de conformidade e descoberta eletrônica, garantindo a preservação de boards que estão sujeitos à investigação ou que sejam relevantes para casos legais em andamento.

[Admins de eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) podem evitar a exclusão permanente de conteúdo, criando retenções legais baseadas em usuários específicos e suas atividades na Miro. Esta funcionalidade é essencial para garantir a preservação e a proteção das informações relevantes durante os procedimentos jurídicos.

Por exemplo, quando um usuário sujeito a uma retenção legal interage com um board, esse board é automaticamente colocado em retenção para evitar sua exclusão permanente.

Além disso, todas as versões do board também são preservadas, garantindo a retenção do conteúdo do board para fins legais.

![legalholdoverview.png](images/22388649794194_legalholdoverview.png)

:::note
Você deve ter a [função de admin de eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) para realizar tarefas de retenção legal. Para solicitar a função de admin de eDiscovery, fale com seu Admin da empresa.
:::

## Principais benefícios da retenção legal

- **Preservação de informações:** a retenção legal garante que todos os dados relevantes sejam preservados, evitando sua exclusão permanente. Isso é crucial para a conformidade e investigações legais, pois garante que os dados apresentados em casos legais permaneçam precisos e inalterados.
- **Conformidade com os requisitos jurídicos:** A retenção legal ajuda as organizações no cumprimento das obrigações legais e regulatórias, garantindo que as informações necessárias sejam preservadas e disponíveis quando necessário, ajudando a evitar penalidades ou desafios jurídicos.
- **Mitigação de riscos:** Ao proteger dados importantes, a retenção legal mitiga o risco de perda de dados que pode resultar em graves consequências jurídicas ou financeiras.
- **Auditoria e monitoramento:** toda vez que uma retenção legal é criada ou modificada, um log de auditoria é gerado, fornecendo total visibilidade e rastreabilidade. Todos os logs de auditoria de uma organização são preservados por tempo indeterminado enquanto pelo menos uma retenção legal está ativa. Isso garante o compromisso e a transparência no gerenciamento de retenções legais.

## Como a retenção legal funciona

- **Interações do Usuário ou Board:** Quando um usuário sob retenção legal abre, modifica ou interage com um board de qualquer forma (renomeando ou adicionando conteúdo), esse board é sinalizado e preservado. Por exemplo, se o nome do board for alterado ou o conteúdo for atualizado, esse board será automaticamente colocado em retenção legal. Além disso, a titularidade e a criação dos boards ficam sob retenção.

  Quando uma retenção legal é criada, ela se aplica aos boards que os custodiantes criaram, possuíam ou co-possuiam no momento da retenção. Além disso, todos os boards que os custodiantes acessem e modifiquem após a retenção também serão incluídos. As informações sobre o acesso ao histórico e atualizações do board não estão disponíveis nesta versão.
- **Ações do usuário final e exclusão do board:** Embora os usuários finais possam excluir os boards, esses boards são preservados se houver uma retenção legal em vigor. Eles ficam inacessíveis ao usuário final, mas são retidos para fins jurídicos e administrativos.
- **Controle administrativo:** admins de eDiscovery podem criar e excluir retenções legais na seção de eDiscovery nas configurações. As retenções legais podem ser aplicadas a todos os boards que um usuário criou, deteve, codeteve, editou ou acessou. Para gerenciar várias retenções legais, os admins podem primeiro criar um caso para agrupar essas retenções.
- **Exclusão do time:** Se um board sob retenção legal existir dentro de um time, esse time não pode ser excluído permanentemente até que a retenção seja liberada. Isso evita a perda indesejada de dados, garantindo que todo o conteúdo relevante seja preservado. Quando um time for excluído, mas contiver um board sob retenção legal, esse time será marcado como preservado na página de times excluídos e sua exclusão permanente ficará desabilitada até que a retenção legal seja removida.
- **Perspectiva de Admin e eDiscovery:** Embora os usuários finais não possam acessar nem recuperar um board excluído que esteja em retenção, os admins e os times de eDiscovery ainda podem interagir com ele. O board é preservado até o encerramento do caso legal, quando a retenção legal pode ser removida e o board pode ser excluído permanentemente.
- **Funcionalidade de exportação do board:** mesmo sob retenção legal, os boards podem ser exportados através da funcionalidade de exportação do board, o que facilita a coleta de dados relevantes para casos legais.
- **Como mover boards:** Os boards sob retenção legal não podem ser movidos para fora da organização. Caso um board esteja sob retenção legal, os times externos são automaticamente excluídos da lista de times para onde é possível mover o board.
