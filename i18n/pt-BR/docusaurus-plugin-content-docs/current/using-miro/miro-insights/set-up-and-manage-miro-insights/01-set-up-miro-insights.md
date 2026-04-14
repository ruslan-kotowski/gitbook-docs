---
title: Configurar o Miro Insights
article_id: 30122381753106
translation_id: 30122381753106
locale: pt-br
sidebar_position: 0
created_at: '2025-10-10T10:26:28Z'
updated_at: '2025-11-25T15:54:01Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Conectar suas ferramentas ao Miro Insights é um primeiro passo crucial para obter valor real. As integrações permitem que o Miro Insights extraia automaticamente feedback de clientes e dados relevantes de seus sistemas. Este guia é para Admins da empresa que habilitarão essas conexões.

Se você é um membro do time procurando usar o Miro Insights após a configuração, veja o artigo sobre [Como usar o Miro Insights](../../miro-insights/use-miro-insights).

## Pré-requisitos

Para configurar integrações do Miro Insights, você precisa atender aos seguintes requisitos:

- Deve ser um **Admin da empresa na Miro**.
- Deve ter **acesso de Admin ou API na plataforma externa** que você está conectando.

:::note
Verifique se o **seu plano Miro inclui o Miro Insights**. Se o Miro Insights for um complemento ou estiver em lançamento limitado, sua conta deve ser elegível. Além disso, algumas integrações podem exigir edições específicas do software externo. Por exemplo, o acesso a API de certos CRMs está disponível em planos de nível superior.
:::

## Prepare suas fontes de dados

Antes de conectar suas fontes de dados ao Miro Insights, é importante preparar seus dados e estabelecer uma taxonomia clara. Essa preparação garantirá que você obtenha insights precisos e acionáveis da plataforma.

### Limpe e otimize seus dados

Antes de sincronizar os dados com o Miro Insights, limpe e otimize suas fontes de dados:

- Remova duplicatas e itens desatualizados.
- Limpe feedbacks inconsistentes ou irrelevantes.
- Garanta a qualidade dos dados em seus sistemas de origem.
- Aborde inconsistências ou lacunas significativas nos dados antecipadamente.

### Estabeleça sua taxonomia

Embora o Miro Insights venha com categorias básicas geradas por IA, é recomendável definir sua própria taxonomia padronizada antes do lançamento. Isso garante consistência e melhora a qualidade dos insights desde o início.

Considere incluir essas categorias padrão:

- Solicitações de funcionalidades
- Bugs
- Pontos de dor de UX
- Segmentos de clientes
- Níveis de prioridade
- Unidades de negócios
- Iniciativas estratégicas

Melhores práticas para taxonomia:

- Use uma terminologia que corresponda à linguagem do seu time.
- Crie diretrizes claras sobre como e quando usar cada categoria.
- Compartilhe a taxonomia com seu time para garantir o uso consistente.
- Revise e refine as categorias regularmente conforme necessário.
- Considere o mapeamento para suas iniciativas estratégicas e OKRs.

:::tip
Entre em contato com o suporte do Miro Insights para obter ajuda na definição de sua taxonomia. Eles podem fornecer exemplos e melhores práticas com base em outros clientes do seu setor.
:::

## Conectar uma integração

Quando seus dados estiverem prontos, você pode conectar suas integrações. O Miro Insights oferece suporte a uma variedade de ferramentas populares em CRM, suporte, chamadas de vendas, gerenciamento de projetos e plataformas de chat.

Na guia **Integrações e Automações** nas configurações, você pode visualizar e gerenciar todas as suas integrações conectadas. Cada integração é listada com seu status de conexão e opções para configurar ou desconectar.

Para conectar uma integração:

1. No aplicativo **Miro Insights**, selecione o ícone **Configurações** no topo da barra lateral esquerda.
2. No painel de **Configurações**, vá até a guia **Integrações e Automações**.
3. Selecione **Conectar** ao lado da integração que você deseja adicionar.
4. **Autorizar acesso**. Um pop-up solicitará que você autorize o Miro Insights a acessar essa ferramenta.
   Isso geralmente envolve fazer login no serviço externo e conceder permissões. Por exemplo, ao conectar-se ao Salesforce, você deve fazer login com sua conta de administrador do Salesforce e aprovar a integração. Para o Slack, selecione um espaço de trabalho e autorize o aplicativo Miro Insights Slack. Siga as instruções na tela para cada um.
5. **Configurar as configurações de importação**. Uma vez conectado, a integração aparecerá como "Conectado" com opções de configuração adicionais. Aqui você pode definir:
   - **Importar conversas de**: Para fontes baseadas em conversas como Gong ou Zendesk, você pode escolher uma data. Isso evita importar dados antigos, a menos que você deseje.
   - **Regras de importação automática**: Ative caso novos itens devam ser importados automaticamente. Você pode habilitar isso para que novas chamadas ou tickets sejam importados continuamente. Se você deixar desativado, talvez precise importar itens manualmente ou seletivamente.
   - **Se a IA detectar pedidos com**: Algumas fontes permitem que você filtre por confiança na detecção por IA.
   - **Detectar itens**: Ativa o Miro Insights para identificar e extrair automaticamente itens do feedback dos clientes. Estes itens podem incluir desafios de usabilidade, problemas de desempenho, preocupações de segurança, etc.

Outras opções podem variar conforme a integração. Por exemplo, no Jira, é possível selecionar de quais projetos importar funcionalidades ou mapear campos personalizados.

### Filtragem por IA

Algumas integrações permitem **filtrar por detecção de IA**. Isso significa que o Insights analisará a transcrição de uma chamada e só criará um item de feedback se houver razoável certeza de que foi mencionado um pedido de produto. Isso reduz o ruído de conversas não relacionadas. Você pode ajustar o limite de confiança ou desligar essa opção para importar tudo.

### Filtros de tag ou campo

Em ferramentas como o Zendesk, você pode especificar uma tag, por exemplo, "feature_request"; assim, apenas tickets com essa tag serão ingeridos. No Jira, você pode selecionar um projeto ou tipo de item específico para importar como funcionalidades.

### Sincronização de itens

Para ferramentas de projeto como o Jira, você pode ter opções para mapear campos. A captura de tela acima mostra um exemplo "Enviar valor monetário da funcionalidade para um campo personalizado" – você pode selecionar um campo personalizado no Jira para preencher com o impacto financeiro calculado pelo Miro Insights, fechando o ciclo de volta para a engenharia. Esta etapa é opcional, mas pode ser poderosa.

Conecte todos os sistemas que são relevantes. Recomendamos, no mínimo, conectar um CRM e uma fonte de suporte ou feedback para começar, garantindo tanto o contexto da conta quanto o feedback bruto. Você pode sempre adicionar mais depois.

Após concluir, você terá conectado com sucesso suas integrações ao Miro Insights. O sistema começará a sincronizar os dados. A sincronização inicial pode levar algum tempo se houver muitos dados históricos (você verá os horários das últimas sincronizações ao lado de cada integração). Você pode monitorar o status da sincronização na lista de Integrações – ela mostra o tempo da última sincronização e oferece uma opção para Desconectar, se necessário.

## Importar itens manualmente

Você também pode importar funcionalidades e itens de feedback manualmente usando um arquivo CSV. Isso é útil para importações únicas ou se você tiver uma lista de solicitações de funcionalidades ou feedback de outra fonte.

Para importar funcionalidades via CSV:

1. No Miro Insights, vá para a visualização **Backlog**.
2. Clique no botão **Importar** no canto superior direito.
3. Selecione **Carregar CSV**.
4. Selecione a coluna na sua fonte de dados CSV que melhor corresponde às propriedades do Miro Insights.
5. Selecione **Importar funcionalidade** para completar o processo.

Suas funcionalidades importadas agora aparecerão na seção [Backlog](../../tools/use-miro-insights/05-backlog.md).

Para importar itens de feedback via CSV:

1. No Miro Insights, vá para a visualização de **Feedback**.
2. Clique no botão **Importar** no canto superior direito.
3. Selecione **Importar CSV**.
4. Mapeie as colunas do seu CSV para as propriedades de feedback do Miro Insights (ex.: título, descrição, fonte).
5. Selecione **Importar feedback** para concluir o processo.

Os itens de feedback importados agora aparecerão na seção [Feedback](../../tools/use-miro-insights/07-feedback.md).

## Conecte ferramentas não suportadas usando Zapier

Se você tem uma ferramenta que não é diretamente suportada, você pode frequentemente usar o [Zapier](http://zapier.com/) para enviar dados para o Miro Insights. Por exemplo, você poderia criar o seguinte fluxo de trabalho no Zapier: quando um Google Form é enviado ou quando uma nova entrada em um banco de dados personalizado aparece, crie um item de feedback no Miro Insights.

Para passos detalhados, consulte o artigo sobre [Usar Zapier com o Miro Insights](../../miro-insights/set-up-and-manage-miro-insights/03-connect-tools-with-zapier.md).

## Passos adicionais

Depois de conectar suas integrações, você pode fazer alguns passos opcionais para garantir que tudo esteja configurado corretamente:

### Importar ou verificar funcionalidades

Se você conectou um rastreador de tarefas como o Jira, verifique o Backlog no Miro Insights para ver se suas funcionalidades ou épicos existentes apareceram. Se não, você pode usar o botão Carregar na visualização do Backlog para carregar um CSV ou acionar uma extração do Jira. Certifique-se de que cada funcionalidade importada tenha um título e uma descrição claros; a IA depende desse texto para associar feedbacks relevantes.

### Configure comandos do Slack ou encaminhamento de e-mails

Se você adicionou o Slack, informe sua equipe sobre como enviar mensagens para o Insights. Por exemplo, clique com o botão direito em uma mensagem > “Enviar para Miro Insights”.

Para e-mail ou outros canais, você pode configurar o encaminhamento. Algumas equipes configuram um endereço de e-mail específico que faz encaminhamento automático para uma ferramenta como o Intercom ou um hook do Zapier para ingestão.

> **Dica**: É uma boa prática revisar periodicamente as configurações de sua integração. Por exemplo, se você perceber que está recebendo muito feedback trivial de uma fonte, ajuste os filtros ou aumente o limite de confiança da IA. Por outro lado, se estiver faltando dados que você esperava, verifique se a integração está conectada com o escopo correto (por exemplo, o projeto ou a tag corretos). Uma configuração de integração bem ajustada mantém o sinal de insights alto e o ruído baixo.

## Desconectar uma integração

Se você precisar desconectar uma integração:

1. Vá para **Configurações** > **Integrações e Automações**.
2. Encontre a integração que deseja remover.
3. Selecione **Desconectar** ao lado dela.
4. Confirme a desconexão no prompt que aparecer.

Isso interromperá qualquer sincronização futura de dados dessa fonte.

> **Importante**: Em alguns casos, por exemplo, Gong, a desconexão pode também remover itens de feedback importados anteriormente. Em outros casos, como Jira, as funcionalidades existentes podem permanecer, mas não receberão atualizações. Revise o comportamento específico de cada integração na documentação ou entre em contato com o suporte se estiver em dúvida.

Certifique-se de comunicar com seu time se você desconectar uma fonte importante, pois isso pode impactar a completude do backlog e do feedback no Miro Insights.

## O que vem a seguir?

Ao conectar integrações, você estabeleceu a base para o Miro Insights oferecer insights ricos e contínuos sobre o produto. Os dados começarão a fluir, e a IA começará a fazer conexões.

Você pode agora prosseguir para [usar o Miro Insights](../../miro-insights/use-miro-insights) ou aprender mais sobre tarefas administrativas em andamento, incluindo configurações gerais, gerenciamento de times, notificações e acesso à API no [guia de administração do Miro Insights](../../miro-insights/set-up-and-manage-miro-insights/02-manage-miro-insights.md).
