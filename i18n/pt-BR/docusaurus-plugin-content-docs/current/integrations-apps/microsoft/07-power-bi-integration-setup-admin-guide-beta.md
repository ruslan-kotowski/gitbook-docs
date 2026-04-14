---
title: Configuração de integração do Power BI (guia do admin) (Beta)
article_id: 18945328862994
translation_id: 18945328862994
locale: pt-br
sidebar_position: 8
created_at: '2024-05-15T12:57:57Z'
updated_at: '2025-11-25T15:42:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: powerbi
availability:
  notes: 'Disponível para: planos Free, Starter, Business, Education e Enterprise
    Disponível em: navegador, aplicativo para desktop Função necessária: Admin da
    empresa'
---

Para empresas que queiram integrar o Microsoft Power BI à Miro, este guia fornece instruções passo a passo sobre como configurar a integração e habilitá-la para times, além de tratar das questões de segurança.

Principais funcionalidades:

- Inserir relatórios e painéis do Power BI nos boards da Miro.
- Especificar quais gráficos devem ser importados para os boards da Miro.
- Solicitar conteúdo atualizado do Power BI diretamente dos boards da Miro.

:::tip
No momento, a integração do Power BI está em Beta privado.
:::

### Implementação técnica

A Miro se integra ao Power BI por meio da [API REST](https://learn.microsoft.com/rest/api/power-bi/) e das [APIs do cliente com análise integrada do Power Bi](https://learn.microsoft.com/javascript/api/overview/powerbi/). Os usuários podem facilmente vincular seus relatórios ou painéis do Power BI aos boards da Miro autorizando o acesso. Para a autenticação, usamos o [OAuth2.0](https://learn.microsoft.com/entra/identity-platform/v2-protocols).

### Requisitos de integração

Verifique se sua assinatura inclui:

- Power BI na nuvem
- Assinaturas compatíveis:
  - SKU do Power BI Premium por capacidade
  - SKU de Reserva de Capacidade do Fabric

## Configurar a integração do Power BI

1. Faça login no Microsoft Entra como admin.
2. Vá até **Aplicativos empresariais** > **Consentimento e permissões** > **Configurações de consentimento do administrador**.
3. Em **Solicitações de consentimento do administrador**, selecione **Sim** para **os usuários podem solicitar o consentimento do administrador para aplicativos com os quais eles não podem consentir**.
4. Em **Quem pode revisar as solicitações de consentimento do administrador**, selecione os usuários, funções e grupos designados como revisores para solicitações de consentimento do administrador.
5. Assim, os usuários poderão solicitar a aprovação. Para ver a tela de solicitação de aprovação, um usuário que não seja admin deve colar um link do Power BI em um board da Miro do time habilitado para os testes de integração da Miro com o Power BI.
6. Os admins selecionados no passo 4 podem navegar até a tela de solicitações de consentimento do administrador e aprovar a solicitação pendente.
7. Uma vez aprovada, a integração da Miro e Power BI permite que qualquer usuário realize a autorização.
8. Para conferir se a integração funciona, cole um link em um painel do Power BI ou um relatório em um board da Miro, que pertença a um time para o qual você habilitou a integração.
9. Clique em **Conectar** para confirmar a autorização no site do Power BI.
10. Uma caixa de diálogo será aberta solicitando que você selecione os gráficos a serem inseridos. Selecione um gráfico e clique em **Adicionar gráfico**.
11. Os gráficos serão adicionados como imagens ao seu board da Miro.

## Como desabilitar a integração do Power BI

Admins podem revogar a permissão excluindo o aplicativo da Miro dos aplicativos empresariais no Microsoft Entra.

1. Faça login no Microsoft Entra.
2. Clique em **Aplicativos empresariais**  > **Consentimento e permissões**.
3. Na lista de aplicativos, localize e selecione **Todos os aplicativos**.
4. Encontre o aplicativo **Contenthub Microsoft Power BI Integration (Integração do Microsoft Power BI pelo hub de conteúdo)** na lista.
5. Clique no aplicativo para acessar suas propriedades.
6. Nas propriedades do aplicativo, clique em **Excluir**.

## Limites da integração

- Não é possível inserir boards públicos.
- Não é possível inserir links de conjuntos de dados.
- Não é possível inserir links do menu Compartilhar.

## Retenção de dados

Os dados inseridos do Power BI seguem a política padrão de retenção de dados da Miro, aplicada a todos os dados dos clientes. Leia o [Adendo de Processamento de Dados da Miro](https://miro.com/legal/documents/Miro-Data-Processing-Addendum.pdf).

Os seguintes tipos de dados de links colados do Power BI são recuperados como imagem e armazenados na Miro:

- Imagens de blocos dos painéis do Power BI
- Imagens de elementos visuais dos relatórios do Power BI
- Títulos de painéis, relatórios, elementos visuais e blocos do Power BI
- Nomes das páginas dos relatórios do Power BI
- Nomes e valores de filtros dos relatórios do Power BI

## Perguntas frequentes

Por que a integração do Power BI está em Beta?

A fase Beta visa coletar feedback para melhorar a estabilidade e a experiência do usuário. A segurança continua sendo nossa prioridade.
