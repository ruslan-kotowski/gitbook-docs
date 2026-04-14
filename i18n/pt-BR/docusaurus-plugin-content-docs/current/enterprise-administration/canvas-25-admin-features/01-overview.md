---
title: "Vis\xE3o geral"
article_id: 30969987585938
translation_id: 30969987585938
locale: pt-br
sidebar_position: 1
created_at: '2025-11-11T12:42:45Z'
updated_at: '2026-01-12T16:04:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

No Canvas 25, anunciamos o Espaço para inovação com IA com fluxos de trabalho visuais e agentes colaborativos impulsionados por IA no canvas. Além das funcionalidades para o usuário final, estamos introduzindo novas funcionalidades de admin para oferecer mais visibilidade, controles mais inteligentes e maneiras integradas de desbloquear as mais recentes ferramentas de IA da Miro para os seus times.

Use esta página para explorar as funcionalidades de admin de IA disponíveis para admins no plano Enterprise. Cada seção começa com uma breve visão geral, seguida por perguntas frequentes expansíveis que cobrem diferentes aspectos de cada funcionalidade.

- [Controles de admin da Miro AI:](01-overview.md) decida quais funcionalidades de IA estão disponíveis na sua organização e gerencie quem pode usá-las.
- Moderação de IA: defina níveis de filtro em toda a organização (Restrito, Padrão, Mínimo) para avaliar prompts que possam gerar resultados prejudiciais ou inadequados.
- Análise para Admins: use painéis no produto (Visão Geral e Miro AI) para acompanhar a adoção e entender a atividade da organização, alocação de licenças, uso de templates e uso da Miro AI em toda a sua organização.

:::note
Durante o beta do AI Workflows, os Termos de Serviço Personalizados de IA e os controles granulares de admin da Miro AI estavam disponíveis para os clientes do AI Workflows. Com a disponibilidade geral do AI Workflows, essas funcionalidades agora estão disponíveis apenas como parte do Enterprise Guard. Para mais informações, veja [Governaça avançada de IA com o Enterprise Guard](01-overview.md).
:::

## Controles de admin da Miro AI

Os controles de admin da Miro AI ajudam você a decidir quais funcionalidades de IA estão disponíveis na sua organização e a gerenciar quem pode usá-las. Para mais informações, veja a [documentação dos controles de admin da Miro AI](../managing-enterprise-teams-and-content/01-miro-ai-admin-controls.md).

**Propósito e escopo**

**Quais são os controles de admin da Miro AI?**

Os controles de admin da Miro AI permitem que os admins gerenciem o acesso às funcionalidades da Miro AI em toda a organização. Dependendo da sua configuração, você pode ativar o acesso para todos, restringir o acesso a times específicos ou desabilitar o acesso.

**Qual é a diferença entre uma funcionalidade de IA e uma funcionalidade de IA?**

Uma **funcionalidade** é uma categoria de capacidade de IA (por exemplo, criar conteúdo, trabalhar com imagens ou resumir atividade). Uma **funcionalidade** é uma ação específica dentro de uma capacidade (por exemplo, c*riar notas adesivas* ou r*emover fundo*).

Os controles de nível de funcionalidade (gerenciamento de funcionalidades individuais dentro de uma funcionalidade) estão disponíveis com o [Enterprise Guard](01-overview.md).

**Acesso e pré-requisitos**

**Onde posso gerenciar os controles de admin do Miro AI?**

No console de admin, vá para **Miro AI** > **Funcionalidades**. De lá, é possível ativar, restringir ou remover o acesso a cada funcionalidade de IA (e, se disponível, a funcionalidades individuais de IA).

**Quem pode configurar essas configurações?**

Os Admins da empresa podem gerenciar o acesso ao Miro AI no console de admin (a disponibilidade de funcionalidades de IA depende do seu plano e complementos habilitados).

**Opções de acesso e comportamento**

**O que significam as opções de acesso (Todos, Ninguém, Times específicos)?**

Use o menu suspenso ao lado de uma funcionalidade (ou funcionalidade específica, se disponível) para escolher como o acesso é concedido.

| Opção | O que faz | Quando usá-la |
| --- | --- | --- |
| **Todos** | Permite acesso para todos os usuários e times da sua organização (incluindo times criados posteriormente). Qualquer restrição em nível de time é sobreposta. | Implementação padrão em toda a organização. |
| **Ninguém** | Remove o acesso para todos. Você será solicitado a confirmar a remoção. | Bloqueio de uso em toda a organização. |
| **Times específicos** | Permite acesso apenas para os times que você selecionar. | Piloto com um subconjunto de times ou implementação faseada. |

**O que acontece se eu desativar uma funcionalidade?**

Quando uma funcionalidade é desativada, os usuários não podem mais acessar essa funcionalidade e seus recursos associados nos boards. Se todas as funcionalidades de Miro AI forem desativadas, **Crie com IA** aparecerá desabilitado no board.

**Essas configurações se aplicam a times criados posteriormente?**

Se você definir uma funcionalidade (ou recurso) para **Todos**, ela se aplicará à sua organização, incluindo times criados posteriormente. Se você escolher **Times específicos**, precisará atualizar a seleção à medida que novos times forem criados (se desejar incluí-los).

**Enterprise Guard e controle ao nível de funcionalidade**

**Como o Enterprise Guard altera o que posso controlar?**

Com [Enterprise Guard](01-overview.md), você pode gerenciar o acesso no **nível de funcionalidade** dentro de cada funcionalidade (não apenas no nível de categoria). Isso permite que você autorize algumas funcionalidades enquanto restringe outras dentro da mesma funcionalidade.

Exemplo: Você pode permitir c*riar imagens* e restringir r*emover fundo* (dentro da funcionalidade de Imagens).

**Visibilidade e disponibilidade**

**Por que não consigo ver as configurações para Fluxos, Assistente de IA ou Prototipagem?**

Algumas funcionalidades (como **Fluxos**, **Assistente de IA** e **Prototipagem**) são visíveis e gerenciáveis apenas se estiverem ativadas para a sua organização.

**Posso ver qual modelo de IA alimenta uma funcionalidade?**

Sim. No console de admin > **Miro AI** > **Funcionalidades**, os admins podem visualizar os modelos que alimentam cada funcionalidade de IA.

**Convidados ou visitantes podem usar a Miro AI se eu ativá-la?**

A Miro AI está disponível para **Membros**. Convidados e visitantes não podem usar a Miro AI.

**Solução de problemas e melhores práticas**

**Eu alterei as configurações de acesso, mas os usuários ainda veem o Miro AI. O que devo verificar?**

- **Confirme o escopo:** Certifique-se de que você atualizou a capacidade correta (ou a funcionalidade específica, se controles em nível de funcionalidade se aplicarem).
- **Verifique o direcionamento do time:** Se ajustado para *Times específicos*, confirme se o time do usuário está selecionado.
- **Dê tempo para propagação:** Em alguns casos, as mudanças podem levar um tempo curto para se aplicar em todas as sessões.
- **Atualize a sessão:** Solicite que o usuário atualize a guia do navegador, faça logout/login, ou reinicie o aplicativo para desktop (se aplicável).

## Moderação de Miro AI

Com a moderação da Miro AI, os Admins da empresa podem ajustar os níveis de filtragem de prompts que possam conter texto potencialmente nocivo ou impróprio. Você pode definir uma sensibilidade de moderação da Miro AI em toda a organização para filtrar conteúdos, incluindo ódio, conteúdo sexual, violência e automutilação. Isso ajuda a alinhar o uso da Miro AI com os requisitos, políticas e tolerância ao risco da sua organização. Para mais informações, veja a [documentação de moderação da Miro AI](../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**Propósito e escopo**

**O que é a Moderação da IA na Miro?**

A Moderação da IA permite que Admins da empresa definam um nível de filtragem para toda a organização (Restrito, Padrão ou Mínimo) que avalie prompts que possam gerar resultados prejudiciais ou inadequados (por exemplo, ódio, conteúdo sexual, violência, automutilação).

**Quem pode configurá-lo e em quais planos?**

Admins da empresa no plano Enterprise com o complemento AI Workflows podem configurar a definição nas configurações da organização.

**Funciona se minha organização conectar seu próprio LLM (por exemplo, uma integração direta com o provedor)?**

Se um LLM personalizado estiver conectado, o seletor de moderação pode ser desabilitado para essa integração, e qualquer nível escolhido anteriormente não se aplicará a ele.

**Acesso e pré-requisitos**

**Quem pode ativá-lo e do que eu preciso?**

Admins da empresa no plano Enterprise com o complemento Miro AI Workflows podem configurar a Moderação de IA nas configurações da organização.

**Como faço para ativá-lo?**

Acesse Configurações → Miro AI → Moderação, escolha Restrito/Padrão/Mínimo, e então clique em **Salvar alterações**. A aplicação é imediata em toda a organização.

**Níveis e comportamento**

**O que os níveis significam?**

- **Rígido:** Bloqueia conteúdo Padrão + de risco baixo a moderado (por exemplo, ódio sutil/codificado, conteúdo sexual sugestivo, violência não gráfica, menções não explícitas de autoagressão).
- **Padrão (recomendado):** Bloqueia conteúdo prejudicial de moderado a severo.
- **Mínimo:** Bloqueia apenas conteúdo severamente prejudicial.

**Quando as alterações entram em vigor?**

Imediatamente para toda a organização.

**As alterações são registradas?**

Sim. As atualizações são registradas na trilha de auditoria da sua organização.

**Configuração e ajustes**

**Onde definir ou atualizar o nível de moderação?**

Acesse Configurações → Miro AI → Moderação, escolha Restrito/Padrão/Mínimo, e então clique em **Salvar alterações**.

**Qual nível inicial você recomenda?**

O padrão atende à maioria das organizações; ajuste com base no feedback do piloto e na tolerância ao risco.

**Interações com outros controles**

**Como a moderação de IA se relaciona com as proteções e os controles de prompt?**

- **Proteções inteligentes:** Se um board estiver coberto pela proteção "Bloquear uso da Miro AI", a IA é desabilitada, independentemente do nível de moderação.
- **Bloqueio de prompt:** Funciona em conjunto com a moderação. O bloqueio de prompt impede a submissão de prompts sensíveis; a moderação filtra categorias prejudiciais.
- **Controles administrativos granulares:** Alternativas de funcionalidade governam quem pode acessar as funcionalidades de IA quando a IA está disponível.

**Solução de problemas e melhores práticas**

**Estamos tendo muitos falsos positivos.**

Considere mudar de Restrito → Padrão (ou de Padrão → Mínimo) e publique exemplos de uso aceitável. Se os problemas persistirem após ajustar as configurações, entre em contato com seu Gerente de Sucesso do Cliente na Miro para relatar isso, para que nossa equipe de produto possa revisar.

**Estamos vendo conteúdos nocivos passarem despercebidos.**

Mude para Padrão ou Restrito e forneça orientações internas. Revise após atualizações de políticas/regulamentações. Se os problemas continuarem após essas mudanças, entre em contato com seu Gerente de Sucesso do Cliente na Miro para relatar isso, para que nossa equipe de produto possa revisar.

## Análise para Admins

A Análise do Admin oferece aos Admins da empresa insights acionáveis e baseados em dados sobre a adoção, uso e gestão do Miro em escala. Inclui dois painéis: **Visão Geral** e **Miro AI**. Para mais informações, consulte [Visão geral da análise](../getting-started/admin-analytics/01-analytics-overview.md), [Painel de visão geral](../getting-started/admin-analytics/02-overview-dashboard.md) e [Painel Miro AI](../getting-started/admin-analytics/03-miro-ai-dashboard.md).

**Propósito e escopo**

**O que é a Análise de Admin?**

A Análise de Admin fornece métricas confiáveis e integradas no produto para ajudar você a entender como o Miro está sendo usado, gerenciar sua organização, impulsionar a adoção e dar suporte às necessidades de segurança e conformidade.

**Quais painéis estão incluídos?**

A Análise de Admin inclui dois painéis: **Visão Geral** (atividade da organização e adoção entre boards, usuários, times, licenças e templates) e **Miro AI** (adoção e uso do Miro AI em toda a organização).

**Painéis e navegação**

**Como alternar entre os painéis?**

Use as guias no topo da página de Análise para alternar entre **Visão Geral** e **Miro AI**.

**Como alterar o intervalo de tempo?**

Use o **seletor de intervalo de tempo** no canto superior direito da página de Análise para ajustar o intervalo de tempo exibido (**diariamente**, **semanalmente**, **mensalmente** ou **trimestralmente**).

**Quando os dados são atualizados?**

As métricas são atualizadas **diariamente**. Cada painel mostra um carimbo de **Última atualização**.

**Painel de visão geral**

**Quais métricas posso acompanhar no painel de visão geral?**

O painel de visão geral ajuda a acompanhar o nível de adoção e a entender a atividade da organização utilizando estes grupos de métricas:

- **Boards:** totais de boards, boards ativos e tendências históricas.
- **Usuários:** tendências de usuários ativos. Você também pode rastrear por função, como membros, Admins da empresa, convidados ou convidados do time.
- **Times:** contagem de times e níveis de atividade.
- **Licenças:** tipos de licenças alocadas e como a alocação muda ao longo do tempo.
- **Templates:** quais templates são mais usados na sua organização.

**Como devo interpretar gráficos históricos?**

- Em widgets que exibem dados históricos, os valores representam dados do **último dia de cada período**.
- O **período atual em curso** não é exibido nos gráficos históricos.
- Os dados históricos estão disponíveis por até **um ano** ou desde que os dados existam.

**Painel do Miro AI**

**O que posso acompanhar no painel do Miro AI?**

O painel do Miro AI ajuda a acompanhar a adoção e entender como a Miro AI é utilizada em sua organização usando essas métricas:

- **Times usando IA:** times que usam ativamente funcionalidades de IA, incluindo totais de times que usam versus os que não usam IA. Você pode filtrar o uso por caso de uso.
- **Pessoas usando IA:** totais de adoção para pessoas usando versus não usando IA, com histórico de uso mensal.
- **IA por caso de uso:** uso ao longo do tempo dividido por **criação de IA** e **automação de IA**.
- **Colaborações com Assistente de IA:** frequência com que os times interagem com os Assistentes de IA por meio de sessões de chat (prompts, perguntas de acompanhamento e respostas). A análise exibe o número de sessões iniciadas.
- **Fluxos de IA executados:** quantas vezes os usuários executaram um fluxo de IA com pelo menos dois passos ou nós consecutivos. A execução é contabilizada a partir do timestamp do primeiro evento associado ao fluxo.

**Como os casos de uso de IA são definidos?**

- **Criação com IA:** ações como criar a partir de prompts e criar a partir do contexto visual.
- **Automação com IA:** ações como iteração através de chat ou menu de contexto, edição de texto, agrupamento e remoção de fundo de imagem.

**O uso de Créditos de IA é o mesmo que as métricas de uso de IA?**

Não. **Os Créditos de IA não estão diretamente correlacionados** com as métricas de uso de IA exibidas neste painel.

**Considerações sobre dados**

**Por que vejo dados parciais?**

Se uma funcionalidade foi desabilitada durante parte de um período selecionado, você pode ver dados parciais no histórico de métricas (por exemplo, se uma funcionalidade foi ativada no meio do mês).

**Por que os gráficos não mostram dados para um período?**

Se nenhuma atividade foi registrada durante um determinado período (dia, semana ou mês), o gráfico não apresentará dados para esse intervalo de tempo.

**Dados antigos parecem faltar. O que devo fazer?**

Dados históricos estão disponíveis por até um ano ou desde quando os dados existem. Se dados antigos parecerem faltar, contate o Suporte da Miro para solicitar a verificação de backfill.

**Solução de problemas e melhores práticas**

**Nossos números parecem inferiores ao esperado. O que devo verificar?**

- Confirme o **período de tempo** e o tipo de período (diário, semanal, mensal, trimestral).
- Lembre-se de que **gráficos históricos mostram períodos concluídos**, e não o período atual em andamento.
- Se uma funcionalidade foi ativada no meio do período, espere **dados parciais** para esse intervalo de tempo.

**Como uso esses insights de forma eficaz?**

Use as métricas do Panorama para identificar times, templates ou tendências de licença subutilizados e, em seguida, execute uma habilitação direcionada. Use as métricas do Miro IA para identificar onde a adoção da IA está crescendo, apoiar os campeões e guiar a implementação responsável.

## Governança avançada de IA com Enterprise Guard

Enterprise Guard fornece funcionalidades adicionais de governança avançada de IA para admins Enterprise. Use esses controles para ajustar o acesso, proteger informações sensíveis e fortalecer o monitoramento e a conformidade para o uso de IA na Miro. Para mais informações, veja [capacidades de confiança de IA do Enterprise Guard e FAQs](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md).

- [Controles administrativos granulares da Miro AI](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): configure o acesso a nível de funcionalidade (Todos/Ninguém/Times específicos) dentro de cada categoria de funcionalidade.
- [Bloquear o uso da Miro AI com Proteções Inteligentes](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): use Proteções Inteligentes para bloquear todas as interações alimentadas por IA na Miro quando precisar proteger dados sensíveis ou confidenciais.
- [Bloqueio de prompts](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): bloqueie prompts contendo dados confidenciais ou código-fonte no momento do envio; mostre uma mensagem de política em vez de enviá-los para um LLM.
- [Enterprise Guard e Microsoft Purview DSPM para integração com IA](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): encaminhe prompts e respostas para o Purview para monitoramento centralizado, auditoria e governança.
