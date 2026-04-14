---
title: Conecte ferramentas com o Zapier
article_id: 30124629305106
translation_id: 30124629305106
locale: pt-br
sidebar_position: 2
created_at: '2025-10-10T11:48:03Z'
updated_at: '2025-10-14T12:37:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Conecte o Miro Insights com centenas de ferramentas através do [Zapier](http://zapier.com/) para capturar automaticamente feedbacks e dados de fontes que não têm integrações diretas. Isso permite centralizar insights do cliente em toda a sua pilha de tecnologia.

A integração com o Zapier permite que você:

- Crie automaticamente itens de feedback a partir de tickets de suporte ao cliente, pesquisas ou conversas de chat.
- Capture dados de qualquer ferramenta que o Zapier suporte, mesmo que o Miro Insights não tenha uma integração direta.
- Reduza a entrada manual de dados configurando fluxos de trabalho automatizados.

## Criar feedback

O Zapier oferece duas ações principais para a criação de itens de feedback no Miro Insights.

### Criar feedback

A ação padrão para criar itens de feedback gerais no Miro Insights com os seguintes campos:

- **Título do feedback**: Resumo breve do feedback.
- **Conteúdo**: Conteúdo detalhado do feedback ou descrição.
- **Nome do relator**: Nome da pessoa que está fornecendo o feedback.
- **E-mail do relator**: Endereço de e-mail do provedor de feedback.
- **E-mail do titular**: Titular ou responsável interno pelo feedback.
- **Data e hora fornecidas**: Quando o feedback foi originalmente dado.
- **URL de origem**: Link para a fonte original (ticket, resposta de pesquisa, etc.).
- **Nome da empresa**: Organização à qual o feedback está associado.
- **Domínio da empresa**: Domínio do site da empresa.

### Criar feedback (Chamada)

Uma ação especializada projetada especificamente para capturar feedback de chamadas e conversas com esses campos:

- **Título da chamada**: Título ou assunto da chamada.
- **Transcrição da chamada**: Transcrição completa ou notas da chamada.
- **URL de origem**: Link para a gravação da chamada ou detalhes da reunião.
- **Participantes**: Informações sobre os participantes da chamada.
  - **E-mail**: Endereço de e-mail do participante.
  - **Nome**: Nome do participante.
- **E-mail do titular**: Responsável interno ou designado para o feedback da chamada.
- **Data e hora de início**: Quando a chamada ocorreu.
- **Nome da empresa**: Organização associada à chamada.
- **Domínio da empresa**: Domínio do site da empresa.

## Configurando a integração com o Zapier

Para começar a usar o Zapier e o Miro Insights, siga estas etapas.

### Pré-requisitos

- Conta ativa no Miro Insights
- Conta no Zapier (gratuita ou paga)
- Acesso à ferramenta de origem que você deseja conectar

### Comece com templates

A Miro Insights oferece templates predefinidos para o Zapier de ferramentas populares de inteligência em conversação, como Grain, Fathom e Fireflies.

Para configurar um Zap usando um template:

1. Vá para as configurações da Miro Insights > seção **Integrações e Automações**.
2. Selecione sua ferramenta de conversação. Por exemplo, Grain.
3. Faça login no Zapier, se necessário.
4. Conecte sua conta do Grain.
5. Mapeie campos do Grain para os campos do Miro Insights.
6. Teste e ative a integração pré-configurada.

Os templates oferecem uma experiência de configuração mais rápida com mapeamentos de campos otimizados para cada ferramenta específica, facilitando o início da captura de feedback dos clientes a partir de suas conversas gravadas.

### Configuração básica

1. **Crie um novo Zap** no seu painel do Zapier.
2. Escolha seu **aplicativo de disparo**. A ferramenta de onde o feedback se origina.
3. Selecione o **Miro Insights** como seu aplicativo de ação.
4. Escolha o seu **evento de ação**:
   - **"Criar feedback"** para itens de feedback geral.
   - **"Criar feedback (chamada)"** para feedback específico de chamadas.
5. Conecte sua **conta do Miro Insights** quando solicitado.
6. **Mapeie os campos** do seu aplicativo de gatilho para os campos do Miro Insights.
7. Teste a integração para garantir que os dados fluam corretamente.
8. **Ative o Zap** para iniciar a coleta automática de dados.

### Melhores práticas de mapeamento de campos

Ao mapear campos da sua ferramenta de origem para o Miro Insights, considere as seguintes práticas recomendadas para garantir a captura de dados de alta qualidade.

**Campos obrigatórios:**

- **Título do feedback**: Utilize títulos claros e descritivos a partir dos seus dados de origem.
- **Conteúdo**: Mapeie o conteúdo principal do feedback ou combine vários campos.

**Campos recomendados:**

- **Informações do repórter**: Capture os detalhes de contato do cliente quando disponíveis.
- **Dados da empresa**: Essenciais para a gestão de produtos baseados em contas.
- **URL de origem**: Mantenha a rastreabilidade de volta às fontes originais.
- **Data fornecida**: Utilize a data real do feedback, e não a data de processamento.

**Dicas de mapeamento de campos:**

- Use as ferramentas de formatação do Zapier para combinar vários campos de origem.
- Inclua o nome da ferramenta de origem no título ou no conteúdo para maior clareza.
- Use formatos consistentes para datas, nomes de empresas e categorias.
- Defina valores padrão para campos opcionais.
