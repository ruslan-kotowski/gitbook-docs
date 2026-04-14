---
title: Aplicativo para desktop
article_id: 360017572854
translation_id: 360017572854
locale: pt-br
sidebar_position: 5
created_at: '2019-02-11T10:15:04Z'
updated_at: '2025-11-25T16:00:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: desktop-mobile-tablet-app
---

Comece a usar o aplicativo para desktop da Miro em segundos diretamente da sua tela inicial e trabalhe nos boards sem distrações. O aplicativo é compatível com todas as funcionalidades básicas da versão para navegador.

:::tip
Baixe o aplicativo da Miro a partir do [nosso site](https://miro.com/apps/).
:::

## Baixar o aplicativo para desktop da Miro

### Windows

- Windows 64-bit - [baixe o aplicativo](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-setup.exe)

:::note
Windows 32-bit é obsoleto e não está mais disponível.
:::

### macOS

- Macs com chips Apple silicon — [baixe o aplicativo](https://desktop.miro.com/platforms/darwin-arm64/Install-Miro.dmg)
- Macs com chips Intel — [baixe o aplicativo](https://desktop.miro.com/platforms/darwin/Install-Miro.dmg)

Para descobrir que tipo de processador você tem, siga estas etapas:

1. Clique no ícone da Apple no canto superior esquerdo do seu Mac.
2. Um menu suspenso será exibido. Clique na opção **Sobre este Mac**.

A janela deve mostrar as informações que você precisa, incluindo o tipo de processador (Intel ou Apple silicon).

## Implantar a Miro em vários dispositivos

A Miro oferece várias versões de instalador que os admins de TI podem usar para implantar a Miro em milhares de máquinas. Há duas formas básicas de fazer isso: instalar por usuário ou por máquina. Cada uma dessas formas fornece versões com e sem atualizações automáticas. A versão com atualizações automáticas significa que seus usuários receberão a versão atualizada do aplicativo assim que for publicada. A versão sem atualizações automáticas oferece mais controle sobre a versão da Miro que os seus funcionários estão usando.

### Para Windows

#### Implante a Miro no Arquivos de Programas

A Miro também pode ser instalada no diretório Arquivos de Programas, ficando disponível para todos os usuários de um dispositivo, mas com seus perfis separados. Uma única instalação em uma máquina significa um espaço menor no disco rígido em escala, ao mesmo tempo em que disponibiliza a Miro para todos os usuários da máquina. Se você optar pela versão com atualizações automáticas, observe que são necessárias permissões administrativas para instalar uma atualização.

- Windows MSI 64 bits com atualizações automáticas - [baixe o aplicativo](https://desktop.miro.com/platforms/win-nsis/Miro-setup.msi)
- Windows MSI 64 bits sem atualizações automáticas - [baixe o aplicativo](https://desktop.miro.com/platforms/win-nsis/Miro-no-updates.msi)

#### Instale a Miro para um usuário específico

Oferecemos várias versões de instalador que os admins de TI podem usar para implantar a Miro para um único usuário. Esta versão pode ser atualizada sem permissões administrativas e instalada apenas para usuários específicos.

- Windows MSI 64 bit com atualizações automáticas - [baixar o app](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-setup.msi)
- Windows MSI 64 bit sem atualizações automáticas - [baixar o app](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-no-updates.msi)

### Para macOS

- Mac com Apple silicon sem atualizações automáticas - [baixar o app](https://desktop.miro.com/platforms/darwin-arm64/Install-Miro-no-updates.dmg)
- Mac Intel sem atualizações automáticas - [baixar o app](https://desktop.miro.com/platforms/darwin/Install-Miro-no-updates.dmg)

## Requisitos de sistema para o app

### Para Windows

|  |  |  |
| --- | --- | --- |
|  | **Mínimo** | **Recomendado** |
| **CPU** | 3 GHz (2 núcleos/4 threads) | 2,8 GHz (4 núcleos/8 threads) |
| **RAM** | 8 GB | 16 GB (DDR4) |
| **SO** | Windows 10 ou superior para o aplicativo da Microsoft Store + Microsoft .NET Framework 4.5 (Observe que a versão ARM do Windows não é suportada) | SO mais recente |
| **Rede** | 8 Mb/s ou mais rápido | 32 Mb/s |

### Para macOS

|  |  |  |
| --- | --- | --- |
|  | **Mínimo** | **Recomendado** |
| **CPU** | Intel de 64 bits ou Apple M1 |  |
| **Sistema Operacional (OS)** | MacOS 12 (Monterey) ou superior | Última versão do OS |
| **Rede** | 8 Mb/s ou mais rápido | 32 Mb/s |

Observe que o aplicativo terá várias instâncias rodando no seu dispositivo:

- processo principal
- processo de janela (renderização de UI)
- aceleração de hardware
- gestão de incidentes
- + 1 processo por cada guia aberta (porque cada guia tem uma visualização da web)

Por exemplo, se você tiver três guias abertas durante o seu trabalho, verá sete instâncias do Miro.exe. Mais informações sobre esta arquitetura podem ser encontradas [aqui](https://www.electronjs.org/docs/glossary#process) e [aqui](https://www.chromium.org/developers/design-documents/multi-process-architecture).

## Atalhos específicos do aplicativo

O aplicativo para desktop tem [atalhos](../../using-miro/working-on-the-board/06-shortcuts-and-hotkeys.md) adicionais:

- **Ctrl + R** *(para Windows)* / **Cmd + R** *(para Mac)* para recarregar a guia
- **Ctrl + W** *(para Windows)* / **Cmd + W** *(para Mac)* para fechar a guia
- **Ctrl + Q** *(para Windows)* / **Cmd + Q** *(para Mac)* para sair do aplicativo
- **Ctrl + Shift + L** *(para Windows)* / **Cmd + Shift + L** *(para Mac)* para copiar o link do board
- **Ctrl + ~** *(para Windows)* **/ Cmd + ~** *(para Mac)* para fazer zoom

## Ações do aplicativo

A tabela a seguir mostra quais ações disponíveis no aplicativo para desktop da Miro podem ter uma experiência diferente do navegador:

| Ação | **Apps Win & Mac da**  [**Miro Apps**](https://miro.com/apps/) |
| --- | --- |
| Salvar como imagem (baixa, média, alta) | ✔ |
| Salvar como imagem (vetor) | ✔ |
| Salvar como PDF (baixa) | ✔ |
| Salvar como PDF (vetor) | ✔ |
| Exportar para uma planilha (CSV) | ✔ |
| Videoconferência | ✔ |
| Colar de uma planilha | ✔ |
| Plugin para Confluence | ✔ |

### Ações indisponíveis

As seguintes ações estão indisponíveis no aplicativo para desktop da Miro:

- Visitantes não podem fazer login.

  > ✏️ Apenas usuários registrados da Miro podem fazer login no aplicativo para desktop.
- Nenhuma opção de copiar/colar do Sketch.
- Para algumas versões do Jira Server, você não pode editar cartões do Jira por motivos de segurança.

## Verificação ortográfica

Se você quiser desabilitar a funcionalidade de verificação ortográfica automática no aplicativo para desktop, siga estas etapas:

- Pressione **Alt** (*apenas para Windows*)
- Clique em **Ver** na barra de navegação principal na parte superior
- Desmarque o botão **Mostrar verificação ortográfica**

Observe que a opção de desabilitar a verificação ortográfica não está disponível no aplicativo baixado da Microsoft Store.

## Possíveis problemas e como resolvê-los

### Como redefinir os dados do aplicativo

Em muitos casos em que um problema surge (especialmente se você estiver tendo dificuldades com o procedimento de login), pode ser útil **redefinir os dados do aplicativo**, limpando a memória do aplicativo.

:::tip
Se o problema persistir após a redefinição dos dados, você também pode querer excluir o aplicativo e reinstalá-lo [baixando a versão mais recente](https://miro.com/apps/).
:::

#### Para Windows

Pressione **Alt > Ajuda** e escolha redefinir os dados do aplicativo como mostrado na captura de tela abaixo:

![reset app data on Windows.png](../../../../../../docs/getting-started/apps-for-devices/images/21016134171922_reset%20app%20data%20on%20Windows.png)
*Reiniciando os dados do aplicativo para desktop no Windows*

Se você não conseguir encontrar o menu, provavelmente usa o aplicativo baixado da MS Store. Nesse caso, para redefinir os dados do aplicativo, abra as **Configurações** do Windows > **Aplicativos** > **Aplicativos e Recursos** > encontre **Miro** na lista > **Opções avançadas** > **Redefinir**.

Se isso não ajudar imediatamente, prossiga para excluir todos os arquivos do aplicativo de **C:\Users\username\AppData\Roaming\RealtimeBoard** e **C:\Users\username\AppData\Local\Programs\RealtimeBoard**

> **✏️** Se a pasta **Appdata** estiver oculta, veja [aqui](https://support.microsoft.com/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5) como revelá-la.

#### Para macOS

Clique em Miro no menu superior e escolha **Redefinir os dados do aplicativo** conforme mostrado na captura de tela abaixo:

![reset app data on Mac.png](../../../../../../docs/getting-started/apps-for-devices/images/21016120799378_reset%20app%20data%20on%20Mac.png)
*Redefinindo os dados do aplicativo no Mac*

Depois disso, tente fazer login no aplicativo novamente e verifique se o problema foi resolvido.

Se a redefinição não ajudar imediatamente, abra uma janela do Finder > pressione **Command + Shift + G** > cole **~/Library/Application Support/RealtimeBoard**e exclua todos os arquivos do aplicativo.

Se você usar MDM para Mac

Se você enfrentar um problema quando o aplicativo não conseguir carregar, ficando em um loop, certifique-se de que sua configuração permita que nosso atualizador automático funcione. `https://github.com/Squirrel/Squirrel.Mac` deve ter permissões para:

- ler, gravar e executar para o diretório `Application`,
- ler e gravar para `~/Application Support/Caches/` para trabalhar com o diretório `com.electron.realtimeboard.ShipIt` e também funciona com o diretório temporário `private/var/folders`.

Se algo der errado durante o processo de atualização, o Squirrel cria `ShipIt_stderr.log` em `~/Application Support/Caches/com.electron.realtimeboard.ShipIt`. Mais informações sobre o problema podem ser encontradas lá.
Observe que o Skype e o Slack usam um processo de atualização semelhante, então, se você já configurou o MDM para eles, pode aplicar as mesmas configurações para o aplicativo para desktop da Miro.

## Perguntas frequentes

1. *Onde posso baixar o aplicativo para desktop?*
   - Baixe-o em [nosso site](https://miro.com/apps/).
2. *Como posso remover o pop-up para abrir o aplicativo para desktop quando inicio a Miro em um navegador?*
   - Tente as etapas deste [artigo](../../using-miro/troubleshooting-technical-questions/technical-guidelines/04-how-to-disable-miro-desktop-app-pop-up-in-your-browser.md).
3. *Tem uma versão do aplicativo para desktop para Linux?*
   - Não, no momento, não temos esta versão.
4. *Como posso copiar o link de um board aberto no aplicativo para desktop?*
   - Você pode abrir o menu **Compartilhar** do board e copiar o link do board de lá. Outra maneira é clicar em **Arquivo** no canto superior direito > **Copiar link do board**. Você também pode usar o atalho **Ctrl + Shift + L** *(para Windows) /* **Cmd + Shift + L** *(para Mac).*
5. *Quando pressiono **Alt** no meu aplicativo para desktop do Windows, o menu não aparece. Como posso obtê-lo?*
   - Observe que o menu não é compatível com o aplicativo baixado da Microsoft Store. Você pode redefinir os dados do aplicativo pelas configurações do Windows (**Sistema > Aplicativos & Funcionalidades > Encontrar Miro > Opções Avançadas > Redefinir**) ou [instalar a versão original do aplicativo](https://miro.com/apps/).
6. *Se eu remover o aplicativo para desktop, meus boards serão excluídos?*
   - Não, seu conteúdo está vinculado ao seu perfil da Miro. Você também pode acessá-lo em um navegador, [aplicativo para tablet](11-tablet-app.md), [aplicativo móvel](08-mobile-app.md).
