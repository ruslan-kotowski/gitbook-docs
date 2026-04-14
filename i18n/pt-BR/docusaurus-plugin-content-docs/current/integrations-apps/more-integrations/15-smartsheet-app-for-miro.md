---
title: Aplicativo Smartsheet para Miro
article_id: 5753415785618
translation_id: 5753415785618
locale: pt-br
sidebar_position: 16
created_at: '2022-05-25T06:41:50Z'
updated_at: '2025-01-13T14:57:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: smartsheet
---

Principais funcionalidades:

- Exportar notas adesivas do Miro para linhas em uma planilha nova ou existente no Smartsheet
- Importar linhas do Smartsheet para um board da Miro como cartões
- Atualize o trabalho no Miro e no Smartsheet com sincronização bidirecional

> **Disponível para:** todos os planos da Miro
> **Disponível em**: versão do navegador no desktop

:::warning
Para que o aplicativo funcione no Safari, desative a opção **Impedir rastreamento entre sites** nas configurações do navegador
:::

### Como instalar o aplicativo

Você pode instalar o aplicativo do [Marketplace da Miro](https://miro.com/marketplace/smartsheet/). Encontrar **Smartsheet para Miro** e clique em **Obter aplicativo**. Você será redirecionado para a página para selecionar a time à qual deseja adicionar o aplicativo Smartsheet. Selecione a time no seletor e clique **Instalar e autorizar.**

:::warning
**Usuários não administradores não podem instalar o aplicativo se ele não for permitido nas [configurações](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).** **⚠️ plano Enterprise Os Admins da empresa podem precisar aprovar o aplicativo nas configurações. Saiba mais.**
:::

![instalando_smartsheet_app.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017653534098_installing%20smartsheet%20app.jpg)
*Selecionando uma time Miro para instalar o aplicativo*

Você também pode instalar **o Smartsheet** a partir de uma board da Miro:

1. Na barra de criação, selecione **Ferramentas, mídia e integrações** (**+**).O painel **Ferramentas, mídia e integrações** será exibido.
2. Na aba **Ferramentas** , pesquise e selecione Smartsheet.
   O modal **Smartsheet** abre e você será solicitado a permitir permissões

![smartsheet-ponto-de-entrada.png](../../../../../../docs/integrations-apps/more-integrations/images/21537438852626_smartsheet-entry-point.png)
*Instalando o aplicativo de dentro de uma board da Miro*

**Quando for perguntado se você deseja conectar sua conta Miro e Smartsheet, faça login na sua conta Smartsheet e permita o acesso ao aplicativo.**

![permitir_acesso_ao_Miro.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017683153682_allow%20access%20to%20Miro.jpg)
***Permitir que o aplicativo acesse sua conta Smartsheet***

### Como exportar notas adesivas ou cartões Miro para linhas Smartsheet

1. Abra o aplicativo Smartsheet na barra de ferramentas. Se você ainda não fez login no Smartsheet, precisará fazer isso primeiro. Em seguida, selecione as notas adesivas que você gostaria de converter.
2. Selecione o espaço de trabalho do Smartsheet, a planilha (nova ou existente) e a linha à qual você gostaria de adicionar o conteúdo das notas adesivas . Você também pode criar uma nova planilha e exportar os notas adesivas para ela.
3. Por fim, selecione **Converter em linha do Smartsheet**. O conteúdo agora será exportado para o Smartsheet. As notas adesivas serão automaticamente convertidas em cartões Smartsheet.
   Observe que os cartões não serão sincronizados com o Smartsheet a menos que você importe as linhas correspondentes do Smartsheet para o Miro (em breve). Veja abaixo como você pode importar dados do Smartsheet para o Miro.
   ![smartsheet_export.gif](../../../../../../docs/integrations-apps/more-integrations/images/21017683165842_smartsheet%20export.gif)
   *Exportando notas adesivas do Miro para o Smartsheet*

### Como importar linhas do Smartsheet para o Miro

1. Abra o aplicativo Smartsheet no Miro e altere a guia de **Converter do Miro** para **Escolher do Smartsheet**.
2. Clique em **Escolher no Smartsheet** e você verá o seletor com suas planilhas existentes. Você terá a opção de filtrar linhas com base em um espaço de trabalho específico e escolher uma planilha.
3. Selecione todas as linhas que deseja importar marcando a caixa e selecionando **Importar**.
4. As linhas serão importadas como cartões.
   ![importar_de_smartsheet.gif](../../../../../../docs/integrations-apps/more-integrations/images/21017683161874_import%20from%20smartsheet.gif)
   *Importando dados do Smartsheet para o Miro*
5. Você pode editar as linhas diretamente no Miro: selecione um cartão, clique no ícone de expansão, aplique as alterações e clique em **Salvar alterações**. Quaisquer atualizações nos cartões serão refletidas no Miro e no Smartsheet.
   ![edit_Smartsheet_card.gif](../../../../../../docs/integrations-apps/more-integrations/images/21017683164818_edit%20Smartsheet%20card.gif)
   *Editando um cartão Smartsheet no Miro*
