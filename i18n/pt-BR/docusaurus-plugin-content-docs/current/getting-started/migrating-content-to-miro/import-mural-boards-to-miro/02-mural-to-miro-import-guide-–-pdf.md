---
title: Guia de importação de Mural para Miro – PDF
article_id: 22856050009362
translation_id: 22856050009362
locale: pt-br
sidebar_position: 2
created_at: '2024-11-25T14:36:20Z'
updated_at: '2026-01-19T14:43:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Pessoas: Usuários com acesso de edição Planos: Business, Education, Enterprise,
    Starter Plataformas: Navegador, Desktop'
---

Você pode importar seus boards existentes do Mural para a Miro exportando-os do Mural como arquivos PDF e, em seguida, importando esses PDFs para a Miro. Este artigo fornece orientações para obter os melhores resultados com importações de PDF, explica o procedimento de importação e descreve o que você pode esperar quando vários elementos do Mural são importados para a Miro usando este método.

O método de importação de PDF é particularmente eficaz para conteúdo que pode não ser transferido bem via copiar e colar ou importações baseadas em API. O importador de PDF da Miro analisa as formas e suas coordenadas dentro do PDF do Mural e tenta reconstruir o layout original. Por exemplo, ele pode interpretar linhas que se cruzam como uma estrutura de tabela.

Observe que alguns objetos podem parecer diferentes no Miro após a importação, e o ajuste de estilo ou layout precisos pode exigir ajustes manuais ou recriações dentro do Miro. Em geral, conteúdos mais simples, com menos estilizações complexas, tendem a apresentar resultados de importação mais precisos.

## Diretrizes para importação do Mural

Para obter os melhores resultados ao importar conteúdo do Mural como PDFs, é útil entender como o importador funciona e que conteúdo é transferido de forma mais eficaz. O importador de PDF se concentra principalmente em corresponder formas básicas e linhas.

:::note
**Nota:** Para importar conteúdo para o Miro, seu conteúdo Mural deve estar sob uma licença completa ou gratuita limitada no Mural.
:::

Espaçamentos claros entre os elementos no seu Mural permitem que o importador do Miro processe o conteúdo de forma mais precisa. Um board Mural com muitos elementos muito próximos pode gerar resultados de importação mistos ou menos precisos.

Para garantir a maior fidelidade na importação, certifique-se de que seu conteúdo do Mural **não** contém os seguintes atributos, pois eles podem não ser transferidos bem via PDF:

- Fontes personalizadas
- Estilos complexos que transformam formas básicas (por exemplo, cantos fortemente arredondados em retângulos, setas com curvatura única)
- Numerosas formas e linhas sobrepostas
- Elementos rotacionados

:::tip
**Dica:** Se você precisa preservar o estilo exato, layouts complexos ou coordenadas precisas do seu conteúdo do Mural, o método mais confiável é exportar o conteúdo do Mural como imagem estática (por exemplo, PNG, JPG) e depois importar essa imagem para o seu board do Miro.
:::

## Importar boards do Mural para a Miro como PDFs

Esta seção explica como importar seu conteúdo do Mural para a Miro usando a funcionalidade de importação de PDF.

### Pré-requisitos para importação de PDF

Antes de iniciar o processo de importação, certifique-se de atender aos seguintes pré-requisitos:

- Você deve ter acesso de edição ao board de origem no Mural (para exportá-lo como PDF).
- Você deve ter acesso de edição ao board de destino na Miro onde pretende importar o conteúdo.
- Você precisa já ter baixado seus boards do Mural como arquivos PDF.

**Mais informações:** Para instruções sobre como exportar do Mural, consulte a documentação do Mural em [Exportar e baixar o conteúdo do seu mural](https://support.mural.co/s/article/export-and-download-your-mural-s-content) (link externo).

### Importar o PDF

Siga estas etapas para importar os PDFs do Mural para o Miro:

1. No seu painel do Miro, clique no botão **+ Criar novo**.
2. No menu suspenso, selecione **Importar** e, em seguida, escolha **Importar do Mural**.
   A caixa de diálogo modal **Importar boards do Mural** será aberta.
3. Siga as instruções na tela dentro do modal. Você será solicitado a carregar seus arquivos PDF do Mural.
   Opcionalmente, você pode escolher adicionar o conteúdo importado a um Espaço específico do Miro. Se não especificar um Espaço, o conteúdo importado será adicionado à área principal do seu time.
4. Após carregar seus arquivos e configurar as opções, selecione **Importar boards**.
   O processo de importação começará. Você receberá uma notificação por e-mail da Miro quando a importação for concluída.

Você agora importou com sucesso o conteúdo do Mural para a Miro via PDF.

## Resultados esperados

Quando os objetos do Mural são importados para o Miro via PDF, algumas variações de estilo e formatação são esperadas devido às diferenças entre as plataformas e à natureza da conversão para PDF. Esta seção descreve os resultados típicos de importação para objetos comuns do Mural e oferece algumas práticas recomendadas.

### Áreas

A área mais externa na sua exportação do Mural normalmente será importada como um quadro no Miro. Outras áreas internas são geralmente importadas como formas regulares no Miro.

:::note
**Nota:** Áreas aninhadas (áreas dentro de áreas) podem às vezes ser identificadas ou estruturadas incorretamente durante a importação. O importador de PDF depende de coordenadas visuais para determinar as relações pai-filho dos widgets, o que pode ser ambíguo com aninhamentos complexos.
:::

### Conectores

O importador de PDF reconhece e recria principalmente conectores de linha sólida. Conectores pontilhados ou tracejados podem não ser importados como esperado.

Se um conector no Mural incluir texto incorporado diretamente na linha, o importador de PDF pode interpretar isso como duas linhas separadas com o objeto de texto próximo, em vez de um único conector com texto.

![A connector with text that the PDF importer breaks into two lines.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*A connector with text that the PDF importer "breaks" into two lines.*

### Desenhos

Elementos desenhados à mão do Mural geralmente são importados como uma coleção de linhas ou curvas na Miro.

Para desenhos complexos, o importador de PDF pode, às vezes, vincular incorretamente partes do desenho a objetos sobrepostos ou próximos, interpretando-os como conectores onde não havia intenção disso.

![A drawing may import as linked to a nearby or overlapping object.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Um desenho pode ser importado como vinculado a um objeto próximo ou sobreposto.*

### GIFs

O importador de PDF reconhecerá os GIFs do Mural, mas os importará como imagens estáticas (normalmente o primeiro quadro do GIF).

:::note
**Nota:** O formato de arquivo PDF em si não suporta GIFs animados. Esta é uma limitação do PDF, não do importador da Miro.
:::

### Imagens

Imagens do seu board do Mural serão importadas como imagens para o Miro. No entanto, a posição exata delas no board pode mudar ligeiramente devido às diferenças nos sistemas de coordenadas entre Mural e Miro, e pelo processo de conversão para PDF.

### Listas

Listas (tanto numeradas quanto com marcadores) do Mural geralmente são importadas como listas no Miro. Para obter os melhores resultados, certifique-se de que suas listas no Mural usem marcadores padrão (números usuais para listas ordenadas e pontos básicos para listas não ordenadas).

![A numbered list, and a bulleted list, with default markers, numerals and bullets respectively.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Uma lista numerada e uma lista com marcadores padrão, números e pontos respectivamente.*

### Mapas mentais

O método de importação em PDF funciona melhor para mapas mentais no Mural que possuem um único nó raiz e bordas visíveis em todos os nós. Mapas mentais complexos com múltiplas raízes ou bordas ocultas podem não ser importados com precisão.

![A basic Mind map is easier to import as PDF.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Um mapa mental básico é mais fácil de importar como PDF*

O importador de PDF pode ter dificuldades para interpretar corretamente mapas mentais porque frequentemente contêm muitas linhas e objetos em proximidade. Se o seu mapa mental em PDF estiver mal importado, considere tentar copiar e colar o conteúdo do mapa mental diretamente do Mural para o Miro. Embora o método de copiar e colar possa exigir ajustes manuais de estilo e escala no Miro, a fidelidade estrutural geral pode ser maior para alguns mapas mentais.

### Formas

O importador de PDF é projetado para importar formas básicas do Mural (por exemplo, retângulos, ovais, triângulos) como formas editáveis no Miro.

![Only basic shapes import as editable content.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Somente formas básicas são importadas como conteúdo editável*

Formas mais avançadas, personalizadas ou com estilo pesado do Mural, assim como formas rotacionadas, podem ser importadas como imagens estáticas em vez de formas editáveis no Miro.

### Notas Adesivas

Notas adesivas padrão do Mural geralmente são importadas como notas adesivas do Miro. Para obter a maior fidelidade, use notas adesivas do Mural com taxas de proporção padrão (por exemplo, tamanhos comuns de 3x3 ou 5x3).

![Sticky notes with the default size can be easily imported.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Notas adesivas com o tamanho padrão podem ser facilmente importadas*

:::note
**Nota:** Notas adesivas redondas do Mural serão importadas como formas normais no Miro, pois o Miro não possui um objeto de nota adesiva redonda nativa.
:::

Notas adesivas sobrepostas ou rotacionadas podem não ser importadas com alta fidelidade e podem exigir reposicionamento ou ajustes manuais no Miro.

![Import results vary for rotated sticky notes, and sticky notes that overlap.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Os resultados da importação variam para notas adesivas rotacionadas e notas adesivas sobrepostas.*

### Tabelas

Tabelas simples do Mural com linhas de grade claras geralmente são importadas com alta fidelidade como tabelas do Miro ou uma coleção de formas e linhas que formam uma estrutura de tabela.

Tabelas com geometria complexa podem ser importadas como uma série de linhas desconectadas e caixas de texto. Para obter os melhores resultados ao importar tabelas, assegure-se de que as tabelas no seu export do Mural **não** possuam os seguintes atributos:

- Células mescladas
- Bordas invisíveis ou ocultas
- Cantoneiras arredondadas nas células ou na borda da tabela

![Complex tables do not import with high fidelity.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Tabelas complexas não são importadas com alta fidelidade.*

### Texto

Objetos de texto do Mural geralmente são importados como texto editável na Miro, frequentemente dentro de um único bloco de texto ou forma que corresponde à caixa de texto original do Mural.

Para obter a maior fidelidade na importação de texto, utilize fontes padrão e margens padrão no Mural.

:::note
**Nota:** O tamanho da fonte pode variar após a importação, e talvez seja necessário ajustá-lo manualmente na Miro.
:::

O importador de PDF pode separar texto que utiliza fontes personalizadas ou possui formatação complexa (por exemplo, múltiplos estilos dentro de uma única caixa de texto) em vários blocos de texto menores.
