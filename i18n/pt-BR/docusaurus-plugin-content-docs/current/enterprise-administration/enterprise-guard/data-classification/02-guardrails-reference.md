---
title: "Refer\xEAncia de prote\xE7\xF5es"
article_id: 28839068735890
translation_id: 28839068735890
locale: pt-br
sidebar_position: 1
created_at: '2025-08-18T09:35:15Z'
updated_at: '2025-11-25T15:53:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

## Proteções de segurança de conteúdo

A tabela a seguir lista as proteções de segurança de conteúdo suportadas na versão atual.

|  |  |  |
| --- | --- | --- |
| **Proteção** | **Descrição** | **Usuários afetados** |
| **Bloquear a replicação de conteúdo** | - As opções para gerenciar a replicação de conteúdo tanto na interface de usuário da Miro quanto nas APIs da Miro não estão disponíveis. Por exemplo, a opção para atualizar quem pode copiar o conteúdo do board não está disponível na interface de usuário e a opção para atualizar o acesso à cópia via a API de atualização do board não está disponível.  - As opções para replicação de conteúdo não estão disponíveis na interface de usuário da Miro. Isso inclui:     - Duplicar um board para outros     times de usuários     - Baixar arquivos no board     - Baixar imagens no board     - Baixar PDFs no board     - Copiar conteúdo ou objetos de      o board para outro board     - Exportar boards como uma imagem     - Exportar boards como PDF     - Salvar boards como um      template     - A replicação de conteúdo via APIs está      não disponível. A API retorna um      erro 403 como resposta. | O titular e os cotitulares do board não têm restrições. O titular e os cotitulares do board podem executar ações de replicação de conteúdo, pois isso é necessário para que o titular atualize o board e crie versões sanitizadas dos boards para colaboração futura.  Todos os outros estão restritos. |
| **Bloquear uso da Miro AI** | - Todas as funcionalidades da Miro AI estão desabilitadas, impedindo o acesso a funcionalidades impulsionadas por IA como geração de texto, reconhecimento de imagens e sugestões inteligentes.  - Os usuários não poderão interagir ou ativar quaisquer ferramentas impulsionadas por IA dentro da Miro.  - O conteúdo existente gerado pela Miro AI permanece inalterado, e os usuários podem modificar ou expandir esse conteúdo. No entanto, os usuários não podem mais usar a Miro AI para editar ou atualizar o conteúdo. | Todos estão restritos, incluindo o titular e os cotitulares do board. |

## Compartilhamento de proteções

A tabela a seguir lista as proteções de compartilhamento suportadas na versão atual.

|  |  |  |
| --- | --- | --- |
| **Proteção** | **Descrição** | **Usuários afetados** |
| **Bloquear o compartilhamento público** | - A opção de compartilhar com *Qualquer pessoa com o link* não está disponível na interface do usuário da Miro.  - O compartilhamento público via API não está disponível. A API retorna um erro 403 como resposta.  - O bloqueio do compartilhamento público não se aplica a boards incorporados usando o link de acesso do Live Embed, pois esses boards não são considerados como compartilhados via link público. Para mais informações, consulte [Como permitir ou restringir a incorporação de boards da Miro em aplicativos compatíveis.](../../managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md) | Todos estão restritos, incluindo o titular do board. |
| **Bloquear o compartilhamento com os times** | - A opção de compartilhar com *Qualquer pessoa do time* não está disponível na UI da Miro.  - Compartilhar com os times via API não está disponível. A API retorna um erro 403 como resposta. | Todos estão restritos, incluindo o titular do board. |
| **Bloquear o compartilhamento com a organização** | - O">Opção de compartilhar com *Qualquer pessoa da organização* não está disponível na UI da Miro.  - Compartilhar com a organização via API não está disponível. A API retorna um erro 403 como resposta. | Todos estão restritos, incluindo o titular do board. |
| **Bloquear o compartilhamento fora de domínios permitidos** | - O compartilhamento de boards via convite direto por e-mail é limitado a usuários cujos endereços de e-mail pertencem aos domínios permitidos nesta lista. Esta proteção não afeta o acesso concedido por meio de times, organizações ou links públicos, pois essas situações são controladas por proteções separadas.  - Você pode adicionar até 20 domínios permitidos nesta lista.  - Esta proteção é projetada para funcionar com a configuração de [**Segurança > Compartilhamento > Domínios permitidos**](../data-security/07-sharing-policy-on-enterprise-plan.md), que pode ser configurada tanto nos níveis de organização quanto de time. Isso significa que, se você tiver a configuração de **Domínios Permitidos** ativada, deve assegurar que o domínio no qual deseja permitir o compartilhamento de boards esteja listado tanto na configuração de Proteções Inteligentes quanto na configuração de [**Segurança > Compartilhamento > Domínios permitidos**](../data-security/07-sharing-policy-on-enterprise-plan.md).   **Notas:**  - Se o board já foi compartilhado com endereços de e-mail que não estão nesta lista, os usuários que já têm acesso ao board continuarão a ter acesso.  - Usuários existentes que já têm acesso a um board, mas não estão na lista de domínios permitidos são indicados na interface Gerenciar acesso ao board. Você pode remover o acesso desses usuários manualmente. - Você pode visualizar facilmente informações sobre restrições de domínio aplicadas via a página de Classificação.   **Exemplo 1:** **Segurança > Compartilhamento > Domínios permitidos:** miro.com, gmail.com  **Domínios permitidos do guardrail:** miro.com  ***Resultado:*** O compartilhamento de boards via convite por e-mail direto é limitado a e-mails que terminam em miro.com. Embora gmail.com seja permitido na configuração Segurança > Compartilhamento > Domínios permitidos, não é permitido pelo guardrail.  **Exemplo 2:** **Segurança > Compartilhamento > Domínios permitidos:** miro.com, gmail.com  **Domínios permitidos do guardrail:** example.org, example.com  ***Resultado:*** O compartilhamento de boards via convite direto por e-mail não é permitido para nenhum domínio, pois não há sobreposição entre as duas listas. | O compartilhamento de boards via convite direto por e-mail é limitado a usuários cujos endereços de e-mail pertencem aos domínios permitidos nesta lista. Esta proteção não afeta o acesso concedido por meio de times, organização ou links públicos, pois estes são controlados por proteções separadas.  Se o board já foi compartilhado com endereços de e-mail que não estão nesta lista, as pessoas que já têm acesso ao board continuarão a ter acesso.   Este guardrail é projetado para funcionar com a configuração [**Segurança > Compartilhamento > Domínios permitidos**](../data-security/07-sharing-policy-on-enterprise-plan.md), que pode ser configurada tanto nos níveis de organização quanto de time. Veja a coluna de descrição para uma descrição detalhada e exemplos. |
