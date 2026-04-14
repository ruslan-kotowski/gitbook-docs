---
title: Como desabilitar o pop-up do aplicativo Miro aplicativo para desktop no seu
  navegador
article_id: 360019244239
translation_id: 360019244239
locale: pt-br
sidebar_position: 5
created_at: '2021-01-29T12:48:31Z'
updated_at: '2026-03-06T13:37:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Se você tiver [o aplicativo Miro Desktop](../../../getting-started/apps-for-devices/05-desktop-app.md) instalado no seu dispositivo, ao abrir um board da Miro em um navegador, você poderá ver o pop-up que sugere que você abra o board no aplicativo.

![navegador_pop-up.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/technical-guidelines/images/21017042611090_browser%20pop-up.jpg)
*O pop-up do navegador que leva você ao aplicativo para desktop Miro Desktop*

Se você quiser desativar o pop-up, siga as instruções abaixo.

- Para usuários de Mac
- Para usuários do Windows
- Navegador Safari

### Para usuários de Mac

**Passo 1.** Exclua (desinstale) o aplicativo para desktop do seu computador.

**Passo 2.** Reverta a configuração 'Sempre abrir URL no aplicativo Miro ' no seu navegador. Veja como você pode fazer isso no Chrome e no Firefox.

Para Chrome

1. Feche todas as janelas do Chrome + Miro antes de iniciar (use **C****md + Q** para sair do navegador).
2. Abra o Finder no seu Mac > pressione**Command + Shift + G** > digite o seguinte caminho na caixa de pesquisa: **~/Library/Application Suporte/Google/Chrome**. Abra sua pasta de perfil do Chrome e encontre **Preferências**.

   Pode haver várias pastas com o arquivo, tente as próximas sugestões:

   - abra e pesquise **Preferências**dentro da pasta **Padrão** , se você tiver apenas um perfil no Google Chrome
   - abra e pesquise **Preferências**dentro da pasta **Perfil X** , se você tiver vários perfis no Google Chrome, onde **X**é um número da lista de perfis
   - abrir e pesquisar**Preferências** dentro de cada pasta (**Padrão, Perfil de Convidado , Perfil X**), se existirem
3. Abra **Preferências** em um editor de texto.
4. Pesquise por **`https://miro.com":\{"miroapp":true\}`** .
5. Remova **`https://miro.com":\{"miroapp":true\}`** .
6. Salvar alterações
7. Reinicie o navegador Chrome.

Se você usar vários perfis do Google, precisará editar as Preferências em todos os catálogos. Para isso, no passo 2, você precisará abrir **~/Library/Application Suporte/Google/Chrome** e alterar **as Preferências** nas pastas **Perfil 1, Perfil 2**, etc.

Para Firefox

1. Abra as configurações do navegador.
2. Na seção **Geral,** role para baixo até **Aplicativos.**
3. Encontre **o miroapp** e altere **Usar Miro** (padrão) para **Sempre perguntar** selecionando a opção no menu suspenso.

### Para usuários do Windows

**Passo 1.** Exclua (desinstale) o aplicativo para desktop do seu computador.

**Passo 2: Use o script disponível [neste link](https://desktop.miro.com/platforms/Miro_DeleteAppSchema.reg) para limpar o valor do registro do Windows*.* Feito isso, a notificação não deverá mais aparecer no seu navegador. Se o pop-up ainda estiver lá, siga a etapa 3.**

**Passo 3.** Reverta a configuração 'Sempre abrir URL no aplicativo Miro ' no seu navegador. Veja como você pode fazer isso no Chrome e no Firefox.

Para Chrome

1. Feche todas as janelas do Chrome + Miro antes de começar.
2. *Navegue*até**PC** > **Usuários > \{current_user\} > AppData > Local > Google > Chrome > UserData > Padrão > Preferências.**
3. Abra **Preferências** em um editor de texto.
4. Pesquise por **`https://miro.com":\{"miroapp":true\}`** .
5. Remova **`https://miro.com":\{"miroapp":true\}`** .
6. Salvar alterações
7. Reinicie o navegador Chrome.

Se você usar vários perfis do Google, precisará editar as Preferências em todos os catálogos. Para isso, navegue até **PC** > **Usuários > \{current_user\} > AppData > Local > Google > Chrome > UserData**e altere **as Preferências** nas pastas **Perfil 1, Perfil 2**, etc.

Para Firefox

1. Abra as configurações do navegador.
2. Na seção **Geral,** role para baixo até **Aplicativos.**
3. Encontre **o miroapp** e altere **Usar Miro** (padrão) para **Sempre perguntar** selecionando a opção no menu suspenso.

### Navegador Safari

Se você precisar desabilitar o pop-up no Safari, exclua o aplicativo para desktop Miro Desktop do seu dispositivo.
