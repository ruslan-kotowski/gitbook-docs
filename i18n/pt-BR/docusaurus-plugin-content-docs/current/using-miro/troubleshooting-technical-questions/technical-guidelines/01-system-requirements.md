---
title: Requisitos de sistema
article_id: 360017731553
translation_id: 360017731553
locale: pt-br
sidebar_position: 1
created_at: '2019-02-11T10:14:54Z'
updated_at: '2026-03-06T14:57:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Este artigo descreve os requisitos de sistema para usar Miro, incluindo dispositivo, GPU e WebAssembly.

Para trabalhar na Miro, certifique-se de que seu dispositivo atenda aos seguintes requisitos mínimos ou recomendados de sistema.

No entanto, lembre-se de que os parâmetros mencionados abaixo não são definitivos, pois o desempenho da Miro pode estar relacionado a vários outros fatores, tais como:

- Tarefas em segundo plano
- Número de guias no navegador e a frequência com que você alterna entre elas
- A resolução do monitor onde você abre o Miro
- Estabilidade da conexão Wi-Fi
- Número de usuários no board
- Sistema de refrigeração do dispositivo

Se você estiver enfrentando problemas de desempenho/acesso, por favor, consulte os [guias de solução de problemas](../troubleshooting) e as [dicas para otimizar o desempenho do board](../../tools/troubleshooting/04-board-performance-and-loading-issues.md).

|  |  |  |
| --- | --- | --- |
|  | **Mínimo** | **Recomendado** |
| **CPU** | 3 GHz (2 núcleos/4 threads) | 2,8 GHz (4 núcleos/8 threads) |
| **Memória RAM** | 8 GB | 16 GB (DDR4) |
| **Largura de banda da rede** | 8 Mb/s | 32 Mb/s |

**Observe que executar a Miro em hardware de ponta, que está muito acima das especificações recomendadas, pode não proporcionar o aumento de desempenho esperado, pois a Miro é um aplicativo web que opera usando o motor do navegador. O motor do navegador não é capaz de utilizar todo o potencial do dispositivo como um software que é instalado localmente no seu computador, projetado para um sistema operacional e arquitetura de CPU específicos.*

Os requisitos mínimos de sistema para o uso confortável do Miro em [tablets](../../../getting-started/apps-for-devices/11-tablet-app.md) são 6 GB de RAM.

O Miro pode ser usado em diferentes tipos de dispositivos. Você pode abrir o Miro em um navegador, baixar a versão para [Desktop](../../../getting-started/apps-for-devices/05-desktop-app.md), [Tablet](../../../getting-started/apps-for-devices/11-tablet-app.md), [aplicativo móvel](../../../getting-started/apps-for-devices/08-mobile-app.md) ou [usar o Miro em um display interativo](../../../getting-started/apps-for-devices/07-interactive-displays.md).

**Modo offline**

Como a Miro depende da visão de uma solução em nuvem perfeita para *colaboração online*, o modo *offline* da ferramenta atualmente não está em nosso radar. No entanto, oferecemos diversas opções de exportação. [Saiba mais](../../import-and-export/export/03-how-to-export-your-board.md).

## Requisitos de GPU e WebAssembly

A Miro usa aceleração de hardware de GPU e WebAssembly (WASM) para renderização suave e para suportar certas funcionalidades avançadas.

### Usando a Miro sem GPU

Para um desempenho ideal, a Miro exige aceleração de hardware de GPU.

Se a aceleração de hardware de GPU não estiver disponível, por exemplo, em algumas máquinas virtuais, ou quando a aceleração de hardware estiver desabilitada, a Miro alterna automaticamente para um renderizador baseado em CPU.

:::tip
Para ter a melhor experiência com a Miro, mantenha a aceleração de hardware habilitada sempre que possível.
:::

Sem aceleração de hardware da GPU, você pode manter os seguintes impactos de desempenho:

- Algumas funcionalidades dependentes da GPU podem estar indisponíveis ou mostradas como espaços reservados
- Deslocamento e zoom mais lentos, especialmente em boards grandes ou com muitos arquivos de mídia
- Funcionalidade principal do board pode não se comportar conforme esperado
- Maior uso de CPU

### Usando a Miro sem WebAssembly (WASM)

Algumas funcionalidades da Miro dependem de módulos de WebAssembly (WASM).

A maioria dos navegadores modernos habilita o WASM por padrão. Se o WASM estiver indisponível, por exemplo, bloqueado em conformidade com políticas empresariais, desabilitado no navegador ou não suportado em ambientes mais antigos, a Miro muda automaticamente para caminhos de renderização baseados em JavaScript quando possível.

**Mais informações:** Consulte [Como verificar se o WASM é suportado no seu navegador](https://help.miro.com/hc/articles/33769132852498).

:::tip
Para a melhor experiência na Miro, mantenha o WebAssembly habilitado. Em um ambiente gerenciado, se você suspeitar que o WASM está bloqueado, verifique com seu time de TI.
:::

Sem o WASM, você pode experimentar as seguintes mudanças de desempenho:

- Funcionalidades que exigem WASM podem não inicializar e são ocultadas ou exibidas como espaços reservados
- Boards que dependem de funcionalidades baseadas em WASM podem não carregar completamente ou não carregar de forma alguma
