---
title: "Funcionalidades de Confian\xE7a de IA e Perguntas Frequentes"
article_id: 30943405198994
translation_id: 30943405198994
locale: pt-br
sidebar_position: 0
created_at: '2025-11-10T14:17:30Z'
updated_at: '2026-03-11T21:32:10Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ai-granular-admin-settings
---

No Canvas 25, anunciamos o Espaço para inovação com IA com fluxos de trabalho visuais e agentes colaborativos impulsionados por IA no canvas. Além das funcionalidades para o usuário final, estamos introduzindo novas funcionalidades de admin para oferecer mais visibilidade, controles mais inteligentes e maneiras integradas de desbloquear as mais recentes ferramentas de IA da Miro para os seus times.

Use esta página para explorar as funcionalidades de Confiança em IA disponíveis com o complemento Enterprise Guard. Cada seção começa com uma breve visão geral, seguida por perguntas frequentes expansíveis que cobrem diferentes aspectos de cada funcionalidade.

- Controles administrativos granulares da Miro AI: configure o acesso a nível de funcionalidade (Todos/Ninguém/Times específicos) dentro de cada categoria de funcionalidade.
- [Bloquear o uso da Miro AI com Proteções Inteligentes](#h_block_ai_with_guardrails): use as Proteções Inteligentes para bloquear todas as interações alimentadas por IA na Miro quando precisar proteger dados sensíveis ou classificados.
- [Painel de Visão Geral de Análise do Admin](#h_admin_analytics_overview): rastreie boards, usuários, times, licenças e templates com tendências históricas e atualização diária.
- Moderação de IA (também disponível no nível Enterprise): defina níveis de filtro em toda a organização (Restrito, Padrão, Mínimo) para avaliar prompts que possam gerar resultados prejudiciais ou inadequados.
- Bloqueio de prompt: bloqueie prompts que contenham dados confidenciais ou código-fonte no momento da submissão; mostre uma mensagem de política em vez de enviar para um LLM.
- Enterprise Guard e Microsoft Purview DSPM para integração de IA: encaminhe prompts e respostas para o Purview para monitoramento centralizado, auditoria e governança.

## Controles granulares de admin da Miro AI para o complemento Enterprise Guard

Os controles de admin da Miro AI permitem que os Admins da empresa no plano Enterprise decidam quais funcionalidades de IA estão disponíveis em sua organização e gerenciem quem pode usá-las. Os admins também podem visualizar os modelos que impulsionam cada funcionalidade de IA. Com o complemento Enterprise Guard, os controles da Miro AI se estendem ao nível de funcionalidade dentro de cada categoria de funcionalidades, o que ajuda a priorizá-las com base nas necessidades organizacionais e nos requisitos de segurança. Além da categoria completa de funcionalidades da Miro AI, os admins podem também habilitar, restringir ou remover funcionalidades específicas da Miro AI. Por exemplo, dentro da categoria Imagens, você pode ativar Criar imagens com IA e desabilitar Remover fundo. Use esses controles para implementar a IA com segurança e atender aos requisitos de segurança enquanto promove a adoção das funcionalidades de IA. Para mais informações, consulte a [documentação dos controles de admin granulares da Miro AI](../../enterprise-guard/ai-trust/02-miro-ai-granular-admin-controls.md).

**Propósito e escopo**

**O que é controle granular para Miro AI?**

Com o complemento Enterprise Guard, os Admins da empresa podem ativar, restringir ou remover o acesso a funcionalidades individuais de IA dentro de cada categoria de funcionalidades. Isso permite escolher exatamente quais funcionalidades os times podem usar.

**Por que usar controles granulares?**

Para equilibrar adoção com segurança. Por exemplo, dentro de Imagens, você pode permitir Criar imagens enquanto desativa Remover fundo.

**Acesso e pré-requisitos**

**Quem pode configurar controles granulares e em quais planos?**

Admins da empresa em planos Enterprise com o complemento Enterprise Guard, no navegador.

**Onde posso gerenciar o acesso no nível de funcionalidades?**

Console do Admin → Miro AI → Funcionalidades. Expanda uma funcionalidade para ver e definir o acesso para suas funcionalidades individuais.

**Controles e comportamento**

**Controles granulares: qual é a diferença entre controle por nível de funcionalidades e por nível de funcionalidade, e o que acontece quando os ativamos ou desativamos?**

- **Nível de funcionalidades:** Todos, Ninguém ou Times específicos se aplica a toda a categoria. Se você desativar uma funcionalidade, os usuários perdem o acesso a essa funcionalidade e a todas as suas funcionalidades em todos os boards. Se desativar todas as funcionalidades, Crie com IA aparecerá desabilitado no board.
- **Nível de funcionalidade:** Com o Enterprise Guard, você pode definir Todos, Ninguém ou Times específicos para cada funcionalidade individual. Desativar uma funcionalidade remove o acesso apenas a essa funcionalidade; outras funcionalidades na mesma funcionalidade permanecem disponíveis se ativadas.

**Quais opções de acesso existem no nível da funcionalidade?**

Para cada funcionalidade, escolha Todos, Ninguém ou Times específicos. Todos ativa a funcionalidade em toda a organização e substitui restrições no nível de time. Ninguém remove o acesso para todos os usuários. Times específicos direciona apenas para os times selecionados.

**O que acontece quando eu desativo uma funcionalidade individual?**

Os usuários não podem acessar essa funcionalidade em nenhum board, mas outras funcionalidades na mesma capacidade permanecem disponíveis, se ativadas.

**Referência e exemplos**

**Quais funcionalidades posso controlar individualmente?**

Consulte a referência no produto para a lista atual. Exemplos na criação de conteúdo incluem Criar notas adesivas, Agrupar notas adesivas, Criar e editar Documentos, Tabelas, Diagramas e operações de Texto, como reescrever, encurtar, ajustar tom e traduzir. Imagens incluem Criar imagens, Remover fundo e Adicionar legendas. Resumo de atividades inclui Fique por dentro e Resumo de conversas. Fluxos, Assistentes de IA e Protótipos aparecem se ativados para sua organização.

**Posso ver quais modelos alimentam funcionalidades específicas?**

Sim. Admins podem visualizar os modelos associados a cada funcionalidade de IA na área de referência para dar suporte à revisão e governança.

## Bloquear o uso da Miro IA com Proteções Inteligentes

Use as Proteções Inteligentes para bloquear todas as interações movidas por IA na Miro quando você precisar proteger dados sensíveis ou classificados. Quando essa proteção é aplicada, todas as ferramentas da Miro AI são desabilitadas nos boards afetados, enquanto a colaboração sem IA permanece disponível. Para o contexto e configuração, consulte a visão geral das Proteções Inteligentes e Defina proteções.

**Propósito e escopo**

**O que significa "Bloquear uso do Miro AI"?**

Ele desabilita todas as funcionalidades do Miro AI (por exemplo, geração de texto, geração/reconhecimento de imagem, sugestões inteligentes) onde quer que esse guardrail seja aplicado, impedindo qualquer interação com conteúdo sensível ou classificado por meio de IA.

**O que permanece disponível para os usuários?**

Os usuários podem continuar a colaboração regular, sem IA. Conteúdos já gerados pela IA permanecem nos boards e podem ser visualizados, movidos ou editados manualmente — mas os usuários não podem usar o Miro AI para modificar ou regenerar esse conteúdo.

**Acesso e pré-requisitos**

**Quem pode configurar esta proteção e onde?**

Admins de Conteúdo Sensível configuram proteções em *Enterprise Guard* em Classificação de Dados → Proteções. (Admins da empresa atribuem a função de Admin de Conteúdo Sensível.)

**O que eu preciso antes de atribuir esta proteção?**

Defina os seus níveis de classificação e (opcionalmente) a classificação automática para que a proteção possa ser aplicada pela classificação (por exemplo, INTERNA, CONFIDENCIAL).

**Comportamento e impacto**

**Quem é afetado quando a proteção é aplicada?**

Todos — incluindo titulares e cotitulares de boards — não poderão acessar ou invocar a Miro AI nos boards afetados.

**Remove o conteúdo de IA existente?**

Não. Ele impede interações futuras com a IA; o conteúdo de IA existente permanece disponível para visualização e edição manual.

**Quando as alterações entram em vigor?**

Após publicar suas atualizações de proteção, a aplicação é imediata nos boards afetados.

**Configuração e ajustes**

**Como ativar "Bloquear uso do Miro AI" para uma classificação?**

1. Vá para *Enterprise Guard* → Classificação de Dados → **Guardrails**.
2. Clique no ícone **Editar** para um nível de classificação (por exemplo, CONFIDENCIAL).
3. Selecione a caixa de seleção **Bloquear uso do Miro AI** e **Concluído**.
4. Clique em **Avançar** e revise o impacto, depois **Publicar** para aplicar.

**Devo usar o modo Padrão ou Estrito?**

No modo Padrão, as proteções não substituirão as configurações de compartilhamento existentes. No modo Estrito, as proteções substituem o compartilhamento ativo e aplicam os controles mais rigorosos. Escolha com base nas suas necessidades de gestão de mudanças.

**Experiência do usuário**

**O que os usuários verão nos boards onde a IA está bloqueada?**

Os pontos de entrada da Miro IA aparecerão desabilitados ou indisponíveis, e os usuários não poderão invocar ferramentas de IA do canvas ou dos menus nesses boards.

**Os usuários podem solicitar exceções em um único board?**

Não. A proteção é aplicada pela política de classificação. Altere a classificação do board (ou a política para esse nível) para modificar a aplicação.

**Interações com outros controles**

**Como isso se relaciona com controles administrativos granulares da Miro AI?**

Os controles granulares definem quem pode usar funcionalidades específicas de IA. O guardrail é uma camada de política: quando ativo, ele bloqueia a IA independentemente das configurações de funcionalidade.

**Como isso difere do bloqueio de prompt ou da Moderação de IA?**

- **Bloqueio de prompt** impede a submissão de prompts sensíveis; a IA permanece disponível para prompts não sensíveis.
- **Moderação de IA** filtra conteúdos nocivos ou inapropriados.
- **Bloquear o uso da Miro AI** desabilita completamente a IA nos boards afetados.

**Solução de problemas**

**IA ainda aparece em alguns boards. O que devo verificar?**

- Confirme que a classificação do board é uma onde as proteções estão ativadas e que você clicou em **Publicar** após editar as proteções.
- Se estiver usando classificação automática, verifique se a classificação do board foi atualizada com base no conteúdo atual.
- Nos modos Estrito vs Padrão, garanta que suas expectativas correspondam ao modo de implementação que você selecionou.

**Precisamos reativar a IA para um subconjunto de trabalho.**

Ajuste as proteções para a classificação relevante ou reclassifique os boards que devem permitir IA, em seguida, publique a atualização.

## Visão geral do painel de Análise do Admin

**Escopo e métricas**

**O que o painel de Visão Geral abrange?**

Boards, Usuários, Times, Licenças e Templates, com tendências históricas quando aplicável.

**Como é definido "Ativo neste período" para Boards, Usuários e Times?**

- **Boards:** Boards únicos abertos desde o início do período selecionado. Inclui boards posteriormente movidos para a lixeira.
- **Usuários:** Usuários únicos que abriram um board pelo menos uma vez desde o início do período. Inclui usuários que agora estão desativados.
- **Times:** Times únicos com pelo menos um membro que abriu um board desde o início do período. Pode incluir times posteriormente movidos para a lixeira.

**Os totais excluem itens na lixeira?**

Sim. Os totais de boards e times excluem itens que estão atualmente na lixeira. Contagens históricas de "ativos" podem incluir itens que foram posteriormente movidos para a lixeira.

**O que o gráfico de Licenças mostra?**

Totais de alocação e histórico para licenças Full, Free e licença gratuita limitada, refletindo quantas licenças estão atualmente em uso.

**O que os Templates mostram hoje?**

Os templates mais populares usados dentro de um board. Outras fontes podem ser adicionadas em lançamentos futuros.

**Comportamento de tempo e histórico**

**Como os valores históricos são exibidos nos gráficos de Resumo?**

Os widgets históricos mostram os valores no último dia de cada período. Até um ano de histórico está disponível ou o máximo que os dados existirem.

**Atualização de dados e controles**

**Com que frequência os dados do Panorama são atualizados e onde posso vê-los?**

Pelo menos uma vez a cada 24 horas. Um carimbo de "Última atualização" está disponível no painel.

**Como altero o intervalo de tempo?**

Use o seletor de intervalo de tempo no canto superior direito da página de Análise.

## Moderação de Miro AI

Com a moderação da Miro AI, os Admins da empresa podem ajustar os níveis de filtragem de prompts que possam conter texto potencialmente nocivo ou impróprio. Você pode definir uma sensibilidade de moderação da Miro AI em toda a organização para filtrar conteúdos, incluindo ódio, conteúdo sexual, violência e automutilação. Isso ajuda a alinhar o uso da Miro AI com os requisitos, políticas e tolerância ao risco da sua organização. Para mais informações, consulte a [documentação de moderação da Miro AI](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**Propósito e escopo**

**O que é a Moderação da IA na Miro?**

A Moderação da IA permite que os Admins da empresa definam um nível de filtragem para toda a organização (Restrito, Padrão ou Mínimo) que avalie prompts que possam gerar resultados prejudiciais ou inadequados (por exemplo, ódio, conteúdo sexual, violência, automutilação).

**Quem pode configurá-lo e em quais planos?**

Admins da empresa no Enterprise com Enterprise Guard podem configurar a definição nas Configurações da organização.

**Funciona se minha organização conectar seu próprio LLM (por exemplo, uma integração direta com o provedor)?**

Se um LLM personalizado estiver conectado, o seletor de moderação pode ser desabilitado para essa integração, e qualquer nível escolhido anteriormente não se aplicará a ele.

**Acesso e pré-requisitos**

**Quem pode ativá-lo e do que eu preciso?**

Admins da empresa no Enterprise com o complemento Enterprise Guard podem configurar a Moderação de IA nas configurações da organização.

**Como faço para ativá-lo?**

Acesse Configurações → Miro AI → Moderação, escolha Restrito/Padrão/Mínimo, e então clique em **Salvar alterações**. A aplicação é imediata em toda a organização.

**Níveis e comportamento**

**O que os níveis significam?**

- **Estrito:** Bloqueia conteúdo Padrão + de risco baixo a moderado (por exemplo, ódio sutil/codificado, conteúdo sexual sugestivo, violência não gráfica, menções não explícitas de autoagressão).
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

**Como a moderação de IA se relaciona com as proteções e controles de prompt?**

- **Proteções inteligentes:** Se um board estiver coberto pela proteção “Bloquear uso da Miro AI”, a IA é desabilitada, independentemente do nível de moderação.
- **Bloqueio de prompt:** Funciona em conjunto com a moderação. O bloqueio de prompt impede a submissão de prompts sensíveis; a moderação filtra categorias prejudiciais.
- **Controles administrativos granulares:** As alternativas de funcionalidade governam quem pode acessar as funcionalidades de IA quando a IA está disponível.

**Solução de problemas e melhores práticas**

**Estamos tendo muitos falsos positivos.**

Considere mudar de Restrito → Padrão (ou de Padrão → Mínimo) e publique exemplos de uso aceitável. Se os problemas persistirem após ajustar as configurações, entre em contato com seu Gerente de Sucesso do Cliente na Miro para relatar isso, para que nossa equipe de produto possa revisar.

**Estamos vendo conteúdos nocivos passarem despercebidos.**

Mude para Padrão ou Restrito e forneça orientações internas. Revise após atualizações de políticas/regulamentações. Se os problemas continuarem após essas mudanças, entre em contato com seu Gerente de Sucesso do Cliente na Miro para relatar isso, para que nossa equipe de produto possa revisar.

## Bloqueio de prompt

O bloqueio de prompt permite que admins de conteúdo confidencial impeçam usuários de enviar prompts de IA que incluam informações sensíveis, ajudando a manter dados confidenciais fora da Miro AI em toda a sua organização. Miro escaneia o texto que um usuário insere no campo de prompt e qualquer conteúdo baseado em texto que eles adicionem ao board. Se esse conteúdo corresponder às etiquetas de sensibilidade ou padrões de código-fonte selecionados na configuração de bloqueio de prompt, Miro bloqueia o envio do prompt. Para mais informações, consulte a [documentação sobre bloqueio de prompt](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md).

**Propósito e escopo**

**O que é o Bloqueio de prompt?**

O Bloqueio de prompt impede que usuários submetam prompts de IA que incluam informações sensíveis. A Miro verifica o texto que um usuário digita no campo de prompt e qualquer conteúdo baseado em texto que eles adicionem no board; se corresponder a etiquetas de sensibilidade ou padrões de código-fonte selecionados, a submissão é bloqueada e uma mensagem de política é exibida. No momento, suportamos apenas conteúdo baseado em texto.

**Como o Bloqueio de prompt é diferente da verificação do board?**

A verificação do board encontra conteúdo sensível nos boards e pode classificar automaticamente os boards; o Bloqueio de prompt verifica o que os usuários tentam enviar para a Miro AI no momento do envio.

**Quais etiquetas de sensibilidade são suportadas?**

Use as categorias em nível organizacional listadas na referência de etiquetas de sensibilidade e infotipos.

**O que é Varredura de código?**

Varredura de código bloqueia prompts que contêm código fonte reconhecível; por design, requer um bloco mínimo de código (por exemplo, 5+ linhas) para acionar. Ative ou desative na configuração de Bloqueio de Prompt.

**Conteúdo não textual (por exemplo, imagens) é analisado?**

Não. Neste momento, o Bloqueio de Prompt suporta apenas conteúdo baseado em texto.

**Acesso e pré-requisitos**

**Quem pode ativá-lo e do que eu preciso?**

Admins de Conteúdo sensível no Enterprise com o complemento Enterprise Guard podem ativá-lo em Configurações → Enterprise Guard → Descoberta de dados → Configuração.

**Como faço para ativá-lo?**

Abra o Bloqueio de prompt → Ativar, escolha Selecionar tudo ou categorias de etiquetas específicas, opcionalmente habilite Varredura de código, depois Ativar. A aplicação é imediata em toda a organização.

**Gerenciamento e alterações**

**Como posso ajustar as etiquetas ou a Varredura de código posteriormente?**

Acesse Configurações → Enterprise Guard → Descoberta de dados → Configuração → Bloqueio de prompt → Gerenciar,

- **Etiquetas:** Selecione a caixa de seleção *Selecionar tudo* para selecionar todas as categorias ou escolha caixas de seleção de categorias de etiquetas específicas.
- **Varredura de código:** Ative a Varredura de código para bloquear prompts que incluam código-fonte (mínimo de 5 linhas). Para mais informações, consulte Varredura de Código.

As alterações entram em vigor imediatamente.

**O que acontece com os prompts após a alteração das configurações?**

Itens recém-desbloqueados serão processados. Itens que ainda correspondem a padrões bloqueados permanecem parados.

**Experiência do usuário**

**O que o usuário vê quando um prompt é bloqueado?**

Uma mensagem de política aparece onde o prompt foi inserido, e a solicitação não é enviada para nenhum LLM.

**Conteúdo não textual (por exemplo, imagens) é analisado?**

Não. No momento, o Bloqueio de Prompt suporta apenas conteúdo baseado em texto.

**Interações com outros controles**

**Como o Bloqueio de prompt funciona com proteções e moderação?**

- **Proteções Inteligentes:** Se "Bloquear o uso da Miro AI" se aplica, a IA é desabilitada. O Bloqueio de prompt não é acionado pois os prompts não podem ser enviados.
- **Moderação de IA:** Ambos podem ser aplicados quando a IA está disponível. O Bloqueio de prompt interrompe dados confidenciais; A moderação filtra categorias prejudiciais.
- **Controles granulares de admin:** O acesso à funcionalidade se aplica apenas quando a IA está disponível e o prompt não é bloqueado.

##

## Enterprise Guard e Microsoft Purview DSPM para integração de IA

Para organizações que utilizam o Microsoft Entra ID (anteriormente Azure AD) como seu provedor de identidade, o Enterprise Guard encaminha com segurança prompts e respostas de IA para o Microsoft Purview Data Security Posture Management (DSPM) para IA. As equipes de segurança e conformidade podem então monitorar, auditar e controlar o uso de IA generativa a partir de uma única plataforma confiável, reduzindo a sobrecarga operacional, mitigando riscos como vazamento e uso indevido de dados e fortalecendo a governança de IA em nível empresarial da Miro. Para mais informações, consulte a [documentação sobre a integração do Enterprise Guard e Microsoft Purview DSPM para IA](../integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).

**Propósito e escopo**

**O que é a integração do Microsoft Purview DSPM para IA na Miro?**

Uma integração que encaminha prompts e respostas da Miro AI para o DSPM da Microsoft Purview para IA, para que as equipes de segurança e conformidade possam monitorar, auditar e governar atividades de IA em um único lugar.

**Quem pode usar essa integração?**

Planos Enterprise com Enterprise Guard, geridos por Admins da empresa com acesso a integrações Enterprise. Sua organização na Miro deve usar o Microsoft Entra ID para logon único. Uma licença da Microsoft Purview é necessária.

**Quais são os benefícios?**

Visibilidade centralizada do uso da Miro AI no hub de IA do Purview, auditabilidade de prompts e respostas e alinhamento com suas políticas de governança existentes no Purview.

**Quais atividades da Miro AI estão incluídas hoje?**

No momento, os prompts baseados em texto e as respostas em todas as funcionalidades da Miro AI são encaminhados. O conteúdo de imagem não é encaminhado.

**As atividades de todos os usuários são registradas?**

Apenas a atividade de usuários que iniciam sessão na Miro através do inquilino configurado do Microsoft Entra é encaminhada para o Purview.

**Quanto tempo demora para que a atividade apareça no Purview?**

Normalmente de 10 a 30 minutos após a ação de IA na Miro. Veja no Microsoft Purview → DSPM para IA → Explorador de atividades, ou verifique os logs de auditoria.

**Existem limitações notáveis?**

No momento, apenas um inquilino Entra pode ser configurado por vez. Em ambientes com múltiplos IdP ou múltiplos inquilinos, apenas usuários autenticando via o inquilino configurado são registrados. Imagens não são incluídas.

**Configuração e ajustes**

**Como faço para habilitar a integração?**

Na Miro: Configurações da empresa → Integrações Enterprise → ative Microsoft Purview DSPM para IA → insira seu ID de tenant do Entra → Conectar → entre com uma conta que possa conceder consentimento de admin em todo o tenant → aceite o aplicativo de governança da Miro AI → confirme Conectado na Miro.

**Quais são os pré-requisitos?**

- **Miro:** Plano Enterprise com Enterprise Guard, função de Admin da empresa, Entra ID configurado para logon único. Para habilitar esta funcionalidade, entre em contato com seu Gerente de Sucesso do Cliente.
- **Microsoft:** Licença Microsoft Purview, o ID do tenant Entra utilizado para logon único da Miro, e uma função Entra que possa conceder consentimento de admin em todo o tenant.

**Como verifico se a configuração funciona?**

Execute uma ação simples na Miro AI, aguarde de 10 a 30 minutos e, em seguida, verifique no Microsoft Purview → DSPM para IA → Explorador de atividades para novas entradas da Miro.

**Como desconecto ou troco de locatários?**

Na Miro: Integrações Enterprise → Microsoft Purview para IA → Desconectar. Para alterar locatários, desconecte primeiro e depois reconecte usando o novo ID de locatário.

**Uso e governança**

**Onde posso ver os dados encaminhados no Purview?**

Microsoft Purview → DSPM para IA → Explorer de atividades. Você também pode revisar os detalhes nos logs de auditoria.

**Posso exportar ou arquivar logs de atividades da IA?**

Use as ferramentas de exportação do Microsoft Purview. A Miro encaminha a atividade para o seu inquilino Microsoft, onde as suas políticas são aplicadas.

**Posso aplicar políticas do Purview aos dados da Miro AI?**

Sim. Quando ingeridos, os dados seguem o modelo de governança do Purview da sua organização.

**E quanto às responsabilidades de privacidade e segurança?**

A Miro encaminha prompts e respostas para o seu inquilino Microsoft. Governança e controles de acesso são geridos no Purview dentro do seu ambiente.

**Solução de problemas e suporte**

**O passo de consentimento falha ou entra em loop. O que devo verificar?**

Certifique-se de que a conta usada para o Connect pode conceder consentimento de admin em todo o tenant na Entra, ou envolva um admin global da Microsoft.

**Não vejo atividade no Purview. O que fazer agora?**

Confirme que o Enterprise Guard está ativado e que você tem acesso às integrações Enterprise. Verifique se o ID do tenant corresponde exatamente ao seu tenant de logon único da Miro. Certifique-se de que uma ação de teste de IA foi realizada por um usuário autenticando-se através desse tenant. Verifique a licença e filtros do Purview. Permita até 30 minutos para a ingestão.

**Usamos múltiplos IdPs ou tenants. Todos os usuários serão registrados?**

Não. Somente a atividade de usuários que fazem login através do único tenant configurado na Entra é encaminhada.

**Quem dá suporte ao quê?**

Entre em contato com o Suporte da Miro para configuração ou conectividade na Miro. Para itens dentro do Microsoft Purview, entre em contato com o Suporte da Microsoft.
