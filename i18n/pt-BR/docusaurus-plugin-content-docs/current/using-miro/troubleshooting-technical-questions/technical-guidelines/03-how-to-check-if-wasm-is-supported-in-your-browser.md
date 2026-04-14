---
title: Como verificar se o WASM é suportado no seu navegador
article_id: 33769132852498
translation_id: 33769132852498
locale: pt-br
sidebar_position: 3
created_at: '2026-03-04T12:47:24Z'
updated_at: '2026-03-16T13:02:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Quem pode fazer: Todos os usuários Quais planos: Free, Starter, Business,
    Enterprise, Education Plataformas: Navegador'
---

WebAssembly (WASM) pode estar desabilitado por motivos que incluem conformidade com políticas de segurança estabelecidas por sua organização ou falta de suporte em ambientes mais antigos, por exemplo.

> **DICA:** A [tabela de comparação do WebAssembly](https://webassembly.org/features/?categories=browsers) mostra quais funcionalidades do WASM são suportadas no seu navegador.

Você pode verificar se o seu navegador suporta WASM.

Siga estas etapas:

1. Abra as Ferramentas de Desenvolvedor.
   - No seu navegador:
     - (MacOS) Chrome, Edge, Firefox: `⌘ + ⌥ + I`
     - (Linux, Windows) Chrome, Edge, Firefox: `Ctrl + Shift + I`, ou `F12`
     - (MacOS) Safari: Vá para **Ajustes** > **Avançado**. Ative **Mostrar menu Desenvolvimento na barra de menu** | **Mostrar funcionalidades para desenvolvedores**. Abra **Desenvolvimento** > **Mostrar console JavaScript**.
   - No aplicativo para desktop da Miro:
     - No canto superior esquerdo, clique em **Ajuda** > **Abrir ferramentas de desenvolvedor**.
2. No DevTools, clique na guia **Console**.
3. Na linha de entrada do console, digite ou cole `typeof WebAssembly`.
4. No teclado, pressione **ENTER**.
5. Interprete o resultado:
   - Se o console retornar `undefined`, então o WebAssembly não é suportado ou está desabilitado.
   - Se o console retornar `object`, então WebAssembly é suportado.![](../../../../../../../docs/using-miro/troubleshooting-technical-questions/technical-guidelines/images/33770259460626_image.png)
     *O console do DevTools mostra* `object` *quando o WASM está disponível no seu navegador.*

     > **NOTA:** Se o console retornar `object` e você ainda não conseguir acessar a Miro, pode revisar outros [possíveis problemas e soluções](../troubleshooting), ou entrar em contato com o [Suporte da Miro](../../tools/troubleshooting/06-contacting-miro-support.md).
