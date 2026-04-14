---
title: Importar etiquetas de sensibilidade do Microsoft Purview
article_id: 22161930709010
translation_id: 22161930709010
locale: pt-br
sidebar_position: 7
created_at: '2024-10-23T15:05:49Z'
updated_at: '2025-12-01T16:32:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Para organizações que utilizam o Microsoft Purview, manter a segurança de dados e a classificação consistentes em várias plataformas é essencial. A integração do Miro com o Microsoft Purview permite que os admins importem etiquetas de sensibilidade diretamente do Microsoft Purview para o Miro, simplificando o gerenciamento dos esquemas de classificação em ambas as plataformas.

Ao aproveitar esta integração, as organizações podem garantir que o conteúdo dentro do Miro seja classificado de forma consistente com o framework já estabelecido pelo Microsoft Purview. Isso não apenas reduz a sobrecarga operacional de recriar ou atualizar manualmente as etiquetas de classificação, mas também fortalece a segurança de dados. Ao alinhar as funcionalidades de proteção de dados do Miro com o Microsoft Purview, os admins podem gerenciar com confiança informações sensíveis em todo o seu ecossistema digital.

## Importar etiquetas de sensibilidade do Microsoft Purview para a Miro

Se a sua organização não possui uma configuração de classificação de dados existente na Miro, você pode facilmente configurar a Classificação de Dados na Miro importando diretamente as etiquetas de sensibilidade existentes do Microsoft Purview.

Se você já possui uma configuração de classificação de dados, pode importar etiquetas de sensibilidade do Microsoft Purview e transferir as etiquetas de classificação existentes na Miro.

## Configurar a Classificação de Dados importando etiquetas de sensibilidade do Microsoft Purview

### Pré-requisitos

- Certifique-se de que você tenha os papéis ou privilégios necessários para trabalhar com etiquetas de sensibilidade no Microsoft Purview.
- Você deve conhecer os detalhes dos níveis de classificação do board que deseja configurar com base nos seus requisitos de segurança e governança.
- Você deve ter a [função de admin de conteúdo sensível](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de conteúdo sensível, fale com seu Admin da empresa.

:::note
Notas:
- Conforme a documentação da Microsoft, as atualizações das etiquetas de sensibilidade no Microsoft Purview podem levar até 24 horas para se replicar em todos os aplicativos e serviços. Por favor, aguarde tempo suficiente para que as alterações ocorram e, em seguida, importe etiquetas de sensibilidade. Se as atualizações feitas no MS Purview não forem replicadas após 24 horas, entre em contato com a equipe de Suporte do Microsoft Purview.
- Você pode importar até 50 etiquetas de sensibilidade do Microsoft Purview para a Miro.
- Se você já possui uma configuração de classificação de dados existente, pode importar etiquetas de sensibilidade do Microsoft Purview e transferir etiquetas de classificação existentes na Miro. Para mais informações, consulte [Importar etiquetas de sensibilidade do Microsoft Purview para uma configuração de classificação de dados existente na Miro](08-import-microsoft-purview-sensitivity-labels.md).
:::

Para importar etiquetas de sensibilidade do Microsoft Purview e configurar a classificação de dados na Miro, execute as seguintes etapas:

1. Acesse suas [Configurações da Miro](https://miro.com/app/settings).
2. No painel à esquerda, em **Enterprise Guard,** clique em **Classificação de dados**.
3. Na página **Classificação**, na parte inferior da tela, clique em **Começar**.
4. Na caixa **Importar do Microsoft Purview**, clique em **Entrar**.
5. Na página **Entrar no Microsoft** que aparece em uma nova guia, insira suas credenciais da Microsoft e faça login. Quando você estiver conectado à sua conta da Microsoft, a guia é fechada automaticamente.
6. Na página de **classificação**, na caixa **Importar do Microsoft Purview**, clique em **Importar**.
   A página **Importar classificação do Microsoft Purview** aparece.
7. Selecione a caixa de seleção das etiquetas de sensibilidade do Microsoft Purview que deseja usar como níveis de classificação na Miro e, em seguida, clique em **Avançar**.

   > ✏️ Conforme a documentação da Microsoft, as atualizações das etiquetas de sensibilidade no Microsoft Purview podem levar até 24 horas para serem replicadas em todos os aplicativos e serviços. Por favor, permita tempo suficiente para que as alterações ocorram e, em seguida, importe as etiquetas de sensibilidade. Caso as atualizações feitas no MS Purview não sejam replicadas após 24 horas, entre em contato com a equipe de Suporte do Microsoft Purview.
8. Na página **Definir níveis de classificação**, você pode editar os níveis de classificação para atribuir o nível de classificação padrão ou adicionar um link para as diretrizes. A tabela a seguir lista cada campo e sua descrição.

   |  |  |
   | --- | --- |
   | **Campo** | **Descrição** |
   | **Link para as diretrizes** | URL que fornece mais informações sobre políticas ou instruções aplicáveis para este nível de classificação. Pode ser uma página onde os usuários da sua organização obtenham mais informações sobre os níveis de classificação dos seus boards e como trabalhar com eles.  Você deve fornecer a URL no seguinte formato: `http://www.example.com`  Quando o usuário clicar no ícone **Saiba mais** (ícone de ponto de interrogação) ao lado do selo de classificação do board, essa URL será carregada em uma nova guia do navegador. |
   | **Usar como nível padrão para novos boards** | Marque esta caixa de seleção para definir este nível de classificação como o padrão para todos os novos boards. |
   | **Pré-visualização** | Exibe uma pré-visualização do selo de classificação do board com sua descrição e ícone para saber mais. A pré-visualização mostra exatamente como o selo de classificação aparece para os usuários em um board. |
9. Para salvar a configuração do nível de classificação, clique em **Concluído**.
10. Clique em **Próximo**. Sua configuração está salva, mas só terá efeito após você clicar em **Publicar** na página [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378).

    Você pode então prosseguir com um dos seguintes passos:

    - [Definir classificação automática](09-define-auto-classification.md). Isso é opcional. Se você quiser definir a classificação automática mais tarde, clique em **Avançar**.
    - [Definir proteções](05-define-guardrails.md). É opcional. Se desejar definir as proteções mais tarde, clique em **Avançar**.
    - [Revisar impacto](https://help.miro.com/hc/articles/16494764223378). Este é o último passo do fluxo de trabalho e é obrigatório.

## Importar etiquetas de sensibilidade do Microsoft Purview para a configuração de classificação de dados existente na Miro

### **Pré-requisitos**

- Certifique-se de que você tenha as funções ou privilégios necessários para trabalhar com as etiquetas de sensibilidade no Microsoft Purview.
- É necessário conhecer os detalhes dos níveis de classificação dos boards que deseja configurar com base em seus requisitos de segurança e governança.
- Você deve ter a [função de admin de conteúdo sensível](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de conteúdo sensível, entre em contato com seu Admin da empresa.

:::note
Notas:
- De acordo com a documentação da Microsoft, atualizações nas etiquetas de sensibilidade no Microsoft Purview podem levar até 24 horas para se replicarem em todos os aplicativos e serviços. Por favor, permita tempo suficiente para que as mudanças ocorram e então importe as etiquetas de sensibilidade. Se as atualizações feitas no MS Purview não forem replicadas após 24 horas, entre em contato com o suporte do Microsoft Purview.
- Você pode importar até 50 etiquetas de sensibilidade do Microsoft Purview para o Miro.
- Você não pode transferir níveis de classificação que estão sendo usados em políticas de retenção. Você deve garantir que os níveis de classificação não estão sendo usados em nenhuma política de retenção antes de prosseguir. Para mais informações, veja [Editar política de retenção](../content-lifecycle-management/11-edit-retention-policy.md).
:::

Para importar etiquetas de sensibilidade do Microsoft Purview e transferir/mapear para as etiquetas de classificação existentes na Miro, siga os passos abaixo:

1. Vá para as suas [configurações da Miro](https://miro.com/app/settings).
2. No painel à esquerda, em **Enterprise Guard,** clique em **Classificação de dados**.
3. Na página de **Classificação**, no topo da tela, clique em **Importar**.
4. Se você já estiver conectado à Microsoft, pule esta etapa e vá para a próxima.
   Se você não estiver conectado à Microsoft, clique em **Entrar**. Na página **Entrar na Microsoft** que aparece em uma nova guia, insira suas credenciais da Microsoft e faça login. Após fazer login na sua conta Microsoft, a guia é fechada automaticamente.
5. Na caixa **Importar do Microsoft Purview**, clique em **Importar** ao lado de Importar etiquetas de sensibilidade para a Miro. A página **Importar classificação do Microsoft Purview** aparece.
6. Na página **Importar Níveis**, marque a caixa de seleção para as etiquetas de sensibilidade do Microsoft Purview que você deseja usar como níveis de classificação na Miro e, em seguida, clique em **Avançar**. A página **Transferir níveis existentes** aparece.

   > ✏️ De acordo com a documentação da Microsoft, as atualizações nas etiquetas de sensibilidade no Microsoft Purview podem levar até 24 horas para replicar em todos os aplicativos e serviços. Aguarde tempo suficiente para que as mudanças ocorram e depois importe as etiquetas de sensibilidade. Se as atualizações feitas no MS Purview não forem replicadas após 24 horas, entre em contato com a equipe de Suporte do Microsoft Purview.
7. Para garantir que o conteúdo seja classificado corretamente, você deve transferir os níveis de classificação existentes na Miro para os novos níveis importados do Microsoft Purview. Os níveis listados à esquerda são os níveis de classificação existentes na Miro e os que estão listados na lista suspensa à direita são as etiquetas de sensibilidade importadas do Microsoft Purview. Quando terminar, clique em **Próximo**.
8. Na página **Definir níveis de classificação**, você pode editar os níveis de classificação para atribuir o nível de classificação padrão ou adicionar um link para as diretrizes. A tabela a seguir lista cada campo e sua descrição.

   |  |  |
   | --- | --- |
   | **Campo** | **Descrição** |
   | **Link para as diretrizes** | URL que fornece mais informações sobre políticas ou instruções aplicáveis a este nível de classificação. Pode ser uma página que oferece mais informações para os usuários da sua organização aprenderem mais sobre os níveis de classificação do seu board e como trabalhar com eles. Você deve fornecer a URL no seguinte formato: `http://www.example.com`  Quando o usuário clica no ícone **Saiba mais** (ícone de ponto de interrogação) ao lado do selo de classificação do board, essa URL é carregada em uma nova guia do navegador. |
   | **Usar como nível padrão para novos boards** | Selecione esta caixa para definir este nível de classificação como a classificação padrão para todos os novos boards. |
   | **Visualizar** | Exibe uma prévia do selo de classificação do board com sua descrição e ícone de mais informações. A visualização mostra exatamente como o selo de classificação aparece para os usuários em um board. |

   Para salvar a configuração do nível de classificação, clique em **Concluído**.
9. Clique em **Próximo**. Sua configuração é salva, mas só entrará em vigor após você clicar em **Publicar** na página [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378).

   Você pode então prosseguir com um dos seguintes passos:

   - [Definir classificação automática](09-define-auto-classification.md). Isso é opcional. Se você quiser definir a classificação automática posteriormente, clique em **Próximo**.
   - [Definir proteções](05-define-guardrails.md). É opcional. Se quiser definir proteções mais tarde, clique em **Próximo**.
   - [Revisar impacto](https://help.miro.com/hc/articles/16494764223378). Este é o último passo do fluxo de trabalho e é obrigatório.

## Desconectar do Microsoft Purview

Quando estiver conectado ao Purview, você não pode adicionar ou editar nomes de classificações, atualizar níveis de classificação, entre outras ações. Se quiser realizar essas ações, é necessário se desconectar do Microsoft Purview. Você não pode importar atualizações do Microsoft Purview para a Miro após se desconectar do Purview.

Para se desconectar do Microsoft Purview, siga os seguintes passos:

1. Vá para as suas [configurações da Miro](https://miro.com/app/settings).
2. No painel à esquerda, em **Enterprise Guard,** clique em **classificação de dados**.
3. Na página de **classificação**, na parte superior da tela, clique no botão **Última Importação** na parte superior da tela e, em seguida, clique em **Desconectar do Purview**.
