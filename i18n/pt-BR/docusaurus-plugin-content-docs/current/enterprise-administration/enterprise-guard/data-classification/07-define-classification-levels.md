---
title: "Definir os n\xEDveis de classifica\xE7\xE3o"
article_id: 16494683650322
translation_id: 16494683650322
locale: pt-br
sidebar_position: 6
created_at: '2024-01-19T18:57:35Z'
updated_at: '2025-11-25T15:40:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Esta é a primeira etapa do fluxo de configuração de classificação automática e guardrails. Nesta etapa do fluxo, você pode definir níveis de classificação, o que envolve adicionar novos níveis de classificação ou atualizar uma configuração de nível de classificação, como nome da classificação, ordem de sensibilidade, cor do selo, link para diretrizes de classificação e muito mais. Ao definir níveis de classificação, você pode:

- [Adicionar ou editar um nível de classificação](07-define-classification-levels.md)
- [Configurar a Classificação de Dados importando rótulos de sensibilidade do Microsoft Purview](07-define-classification-levels.md)
- [Atualizar o nível de classificação padrão para novos boards](07-define-classification-levels.md)
- [Atualizar a ordem de sensibilidade de um nível de classificação](07-define-classification-levels.md)
- [Remover um nível de classificação](07-define-classification-levels.md)

## Pré-requisitos

- Você deve conhecer os detalhes dos níveis de classificação do board que deseja configurar com base em seus requisitos de segurança e governança.
- Você deve ter a [função de admin de conteúdo Sensível](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de conteúdo sensível, entre em contato com seu Admin da empresa.

## Adicionar ou editar um nível de classificação

Você pode adicionar ou editar um nível de classificação executando as seguintes etapas:

1. Vá para as [configurações da Miro](https://miro.com/app/settings).
2. No painel esquerdo, em **Enterprise Guard,** clique em **Classificação de dados**.
3. Se você estiver definindo níveis de classificação pela primeira vez, clique em **Configurar classificação** na parte inferior da tela.
   Se você quiser editar os níveis de classificação, clique em **Editar níveis de classificação**no canto superior direito da tela.
4. Na página **Definir níveis de classificação** :
   Para adicionar um nível de classificação, clique em **Adicionar nível**.
   Para editar um nível de classificação, clique em **Editar níveis de classificação**.
5. Adicione ou edite o nível de classificação de acordo com suas necessidades. A tabela a seguir mostra cada campo e sua descrição.

   |  |  |
   | --- | --- |
   | **Campo** | **Descrição** |
   | **Nível** | Indica a ordem de sensibilidade do board para este nível de classificação.  Atualmente, a ordem de sensibilidade **1** indica o nível de classificação **menos sensível** .  Clique nas setas para cima ou para baixo para atribuir a ordem de sensibilidade do board para este nível de classificação. |
   | **Nome** | Nome do nível de classificação.  Quando os usuários visualizar um board que pertence a esse nível de classificação, esse nome aparece no emblema de classificação do board ao lado do nome do board .  A Figura 1 ilustra um exemplo onde o nome da classificação da board é **INTERNO**.  amostra_board_internal.png Figura 1: Exemplo onde o nome da classificação do board é **INTERNO** |
   | **Descrição** | Descrição deste nível de classificação.  Quando os usuários visualizar um board que pertence a esse nível de classificação e clicam no emblema de classificação do board , a descrição do nível de classificação é exibida.  Recomendamos que você adicione uma descrição significativa que oriente seus usuários sobre a sensibilidade deste board e as precauções ou ações recomendadas.  A Figura 2 ilustra um exemplo da **descrição** adicionada para o nível de classificação INTERNO.   amostra_descrição_interna.png Figura 2: Exemplo da **descrição** adicionada para o nível de classificação INTERNO |
   | **Cor do emblema** | Cor de fundo para o emblema de classificação do board .  A Figura 3 ilustra um exemplo em que o nível de classificação do board INTERNO tem uma cor de emblema **amarela** .  amostra_board_internal.png Figura 3: Exemplo onde o nível de classificação do board INTERNO tem uma cor de emblema **amarela** |
   | **Link para as diretrizes** | URL que fornece mais informações sobre políticas ou instruções aplicáveis a este nível de classificação. Esta pode ser uma página que fornece mais informações para os usuários da sua organização aprenderem mais sobre os níveis de classificação do seu board e como trabalhar com eles. Você deve fornecer a URL no seguinte formato: `http://www.example.com`  Quando o usuário clica no ícone **Saiba mais** (ícone de ponto de interrogação) ao lado do emblema de classificação do board , esta URL é carregada em uma nova aba do navegador. |
   | **Usar como nível padrão para novos boards** | Marque esta caixa de seleção para definir este nível de classificação como a classificação padrão para todos os novos boards. |
   | **Visualização** | Exibe uma prévia do emblema de classificação do board com sua descrição e ícone para saber mais. A pré-visualização mostra exatamente como o emblema de classificação aparece para os usuários em um board. |

   Para salvar a configuração do nível de classificação, clique em **Concluído**.
6. Clique em **Avançar**. Sua configuração será salva, mas só entrará em vigor depois que você clicar em **Publicar** na página [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) .

   Você pode então prosseguir com qualquer uma das seguintes etapas:

   - Definir a classificação automática Isto é opcional. Se você quiser definir a classificação automática posteriormente, clique em **Avançar**.
   - Definir as proteções Isto é opcional. Se você quiser definir guardrails posteriormente, clique em **Avançar**.
   - Revisar impacto Esta é a última etapa do fluxo de trabalho e é obrigatória.

## Configurar a Classificação de Dados importando rótulos de sensibilidade do Microsoft Purview

### Pré-requisitos

- Certifique-se de ter as funções ou privilégios necessários para trabalhar com rótulos de sensibilidade no Microsoft Purview.
- Você deve conhecer os detalhes dos níveis de classificação do board que deseja configurar com base em seus requisitos de segurança e governança.
- Você deve ter a [função de admin de conteúdo Sensível](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de conteúdo sensível, entre em contato com seu Admin da empresa.

:::note
Notas:
- De acordo com a documentação da Microsoft, as atualizações dos rótulos de sensibilidade no Microsoft Purview podem levar até 24 horas para serem replicadas para todos os aplicativos e serviços. Aguarde tempo suficiente para que as alterações ocorram e então importe os rótulos de sensibilidade. Se as atualizações feitas no MS Purview não forem replicadas após 24 horas, entre em contato com a time de Suporte do Microsoft Purview.
- Você pode importar até 50 rótulos de sensibilidade do Microsoft Purview para o Miro.
- Se você já tiver uma configuração de classificação de dados existente, poderá importar rótulos de sensibilidade do Microsoft Purview e transferir rótulos de classificação existentes no Miro. Para obter mais informações, consulte [Importar rótulos de sensibilidade do Microsoft Purview para a configuração de classificação de dados existente no Miro](08-import-microsoft-purview-sensitivity-labels.md).
:::

Para importar rótulos de sensibilidade do Microsoft Purview e configurar a classificação de dados no Miro, execute as seguintes etapas:

1. Vá para as [configurações da Miro](https://miro.com/app/settings).
2. No painel esquerdo, em **Enterprise Guard,** clique em **Classificação de dados**.
3. Na página **Classificação** , na parte inferior da tela, clique em **Começar**.
4. Na caixa **Importar do Microsoft Purview** , clique em **Entrar**.
5. Na página **de login da Microsoft** que aparece em uma nova guia, insira suas credenciais da Microsoft e entre. Depois que você entrar na sua conta da Microsoft, a guia será fechada automaticamente,
6. Na página **Classificação** , na caixa **Importar do Microsoft Purview** , clique em **Importar**.
   A página **Classificação de importação do Microsoft Purview** é exibida.
7. Marque a caixa de seleção para os rótulos de sensibilidade do Microsoft Purview que você deseja usar como níveis de classificação no Miro e clique em **Avançar**.
   > ✏️ De acordo com a documentação da Microsoft, as atualizações dos rótulos de sensibilidade no Microsoft Purview podem levar até 24 horas para serem replicadas para todos os aplicativos e serviços. Aguarde tempo suficiente para que as alterações ocorram e então importe os rótulos de sensibilidade. Se as atualizações feitas no MS Purview não forem replicadas após 24 horas, entre em contato com a time de Suporte do Microsoft Purview.
8. Na página **Definir níveis de classificação** , você pode editar os níveis de classificação para atribuir o nível de classificação padrão ou adicionar um link para as diretrizes. A tabela a seguir mostra cada campo e sua descrição.

   |  |  |
   | --- | --- |
   | **Campo** | **Descrição** |
   | **Link para as diretrizes** | URL que fornece mais informações sobre políticas ou instruções aplicáveis a este nível de classificação. Esta pode ser uma página que fornece mais informações para os usuários da sua organização aprenderem mais sobre os níveis de classificação do seu board e como trabalhar com eles. Você deve fornecer a URL no seguinte formato: `http://www.example.com`  Quando o usuário clica no ícone **Saiba mais** (ícone de ponto de interrogação) ao lado do emblema de classificação do board , esta URL é carregada em uma nova aba do navegador. |
   | **Usar como nível padrão para novos boards** | Marque esta caixa de seleção para definir este nível de classificação como a classificação padrão para todos os novos boards. |
   | **Visualização** | Exibe uma prévia do emblema de classificação do board com sua descrição e ícone para saber mais. A pré-visualização mostra exatamente como o emblema de classificação aparece para os usuários em um board. |

   Para salvar a configuração do nível de classificação, clique em **Concluído**.
9. Clique em **Avançar**. Sua configuração será salva, mas só entrará em vigor depois que você clicar em **Publicar** na página [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) .

   Você pode então prosseguir com qualquer uma das seguintes etapas:

   - Definir a classificação automática Isto é opcional. Se você quiser definir a classificação automática posteriormente, clique em **Avançar**.
   - Definir as proteções Isto é opcional. Se você quiser definir guardrails posteriormente, clique em **Avançar**.
   - Revisar impacto Esta é a última etapa do fluxo de trabalho e é obrigatória.

## Atualizar o nível de classificação padrão para novos boards

Você pode atualizar o nível de classificação padrão executando as seguintes etapas:

1. Vá para as [configurações da Miro](https://miro.com/app/settings).
2. No painel esquerdo, em **Enterprise Guard,** clique em **Classificação de dados**.
3. Clique em **Editar níveis de classificação**no canto superior direito da tela.
4. Na página **Definir níveis de classificação** , clique em **Editar níveis de classificação**.
5. Clique no ícone **Editar** (![Captura de tela 2024-01-22 em 23.20.18.png](images/21017417818770_Screenshot%202024-01-22%20at%2023.20.18.png)) para o nível que você deseja definir como o nível de classificação padrão.
6. Marque a caixa de seleção **Usar como nível padrão para novos boards** .
7. 5. Clique em **Concluído**.
   Sua configuração será salva, mas só entrará em vigor depois que você clicar em **Publicar** na página [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) .
8. Clique em **Avançar**. Sua configuração será salva, mas só entrará em vigor depois que você clicar em **Publicar** na página [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) .

   Você pode então prosseguir com qualquer uma das seguintes etapas:

   - Definir a classificação automática Isto é opcional. Se você quiser definir a classificação automática posteriormente, clique em **Avançar**.
   - Definir as proteções Isto é opcional. Se você quiser definir guardrails posteriormente, clique em **Avançar**.
   - Revisar impacto Esta é a última etapa do fluxo de trabalho e é obrigatória.

## Atualizar a ordem de sensibilidade de um nível de classificação

Você pode atualizar a ordem de sensibilidade de um nível de classificação executando as seguintes etapas:

1. Vá para as [configurações da Miro](https://miro.com/app/settings).
2. No painel esquerdo, em **Enterprise Guard,** clique em **Classificação de dados**.
3. Clique em **Editar níveis de classificação**no canto superior direito da tela.
4. Na página **Definir níveis de classificação** , clique em **Editar níveis de classificação**.
5. Os níveis de classificação aparecem com sua ordem de sensibilidade atual. Clique nas setas para cima ou para baixo dos níveis de classificação para os quais você deseja atualizar a ordem de sensibilidade.

   > ✏️ Atualmente, a ordem de sensibilidade **1** indica o nível de classificação **menos sensível** .

   Sua configuração será salva, mas só entrará em vigor depois que você clicar em **Publicar** na página **[Revisar impacto](https://help.miro.com/hc/articles/16494764223378)** .
6. Clique em **Avançar**. Sua configuração será salva, mas só entrará em vigor depois que você clicar em **Publicar** na página [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) .

   Você pode então prosseguir com qualquer uma das seguintes etapas:

   - Definir a classificação automática Isto é opcional. Se você quiser definir a classificação automática posteriormente, clique em **Avançar**.
   - Definir as proteções Isto é opcional. Se você quiser definir guardrails posteriormente, clique em **Avançar**.
   - Revisar impacto Esta é a última etapa do fluxo de trabalho e é obrigatória.

## Remover um nível de classificação

:::note
Você não pode remover um nível de classificação se ele estiver associado a uma [política de retenção](https://help.miro.com/hc/sections/19180529348754).
:::

Você pode remover um nível de classificação executando as seguintes etapas:

1. Vá para as [configurações da Miro](https://miro.com/app/settings).
2. No painel esquerdo, em **Enterprise Guard,** clique em **Classificação de dados**.
3. Clique em **Editar níveis de classificação**no canto superior direito da tela.
4. Na página **Definir níveis de classificação** , clique em **Editar níveis de classificação**.
5. Clique no ícone de exclusão para o nível de classificação que você deseja remover.
6. Se o nível de classificação que você deseja excluir já tiver sido aplicado a 1 ou mais boards, uma janela de notificação será exibida informando sobre o número de boards aos quais o nível de classificação foi aplicado.
   Selecione o novo nível de classificação que você deseja aplicar aos boards afetados.
7. 5. Clique em **Concluído**.
   Sua configuração será salva, mas só entrará em vigor depois que você clicar em **Publicar** na página [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) .
8. Clique em **Avançar**. Sua configuração será salva, mas só entrará em vigor depois que você clicar em **Publicar** na página [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) .

   Você pode então prosseguir com qualquer uma das seguintes etapas:

   - Definir a classificação automática Isto é opcional. Se você quiser definir a classificação automática posteriormente, clique em **Avançar**.
   - Definir as proteções Isto é opcional. Se você quiser definir guardrails posteriormente, clique em **Avançar**.
   - Revisar impacto Esta é a última etapa do fluxo de trabalho e é obrigatória.
