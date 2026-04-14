---
title: Guia de importação do Mural para a Miro – Copiar-colar
article_id: 22957521683986
translation_id: 22957521683986
locale: pt-br
sidebar_position: 1
created_at: '2024-11-29T13:36:36Z'
updated_at: '2025-11-25T15:49:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Pessoas: Usuários com acesso de edição Planos: Free, Starter, Business,
    Enterprise e Education Plataformas: Navegador, Desktop, Dispositivo móvel'
---

Você pode transferir conteúdo dos seus boards do Mural para a Miro usando o método de copiar e colar. Este guia fornece as melhores práticas para este método de importação, explica o processo passo a passo e detalha o que você pode esperar em relação à aparência e comportamento de vários objetos, uma vez colados na Miro.

## Diretrizes para importar do Mural

Seguir estas diretrizes ajudará você a obter os melhores resultados ao transferir conteúdo do Mural para a Miro.

Para dados estruturados, como mapas mentais do Mural, o método de copiar e colar é geralmente a melhor abordagem para evitar quebrar as conexões entre os elementos.

:::note
Para importar conteúdo para a Miro usando este método, o conteúdo do Mural deve estar sob uma licença completa ou gratuita limitada no Mural.
:::

O método de copiar e colar também é recomendado para importar widgets individuais que não são suportados pelo [guia de importação de Mural para Miro (PDF)](02-mural-to-miro-import-guide-–-pdf.md), ou para widgets que não são importados com alta fidelidade usando o método PDF.

Esteja ciente de algumas limitações com o método copiar e colar: certos atributos de estilo e quaisquer imagens que foram originalmente carregadas no Mural (em vez de vinculadas via URL) não serão copiadas para sua área de transferência e, portanto, não serão transferidas para a Miro.

## Copiar e colar conteúdo do Mural para a Miro

O procedimento a seguir explica como copiar conteúdo de um board do Mural e colá-lo em um board da Miro.

**Pré-requisitos**

Certifique-se de ter acesso de edição tanto ao board de origem no Mural quanto ao board de destino na Miro.

Para copiar conteúdo de um board do Mural e colá-lo em um board da Miro:

1. No Mural, selecione os objetos que deseja copiar.
   > 💡 Para selecionar todos os objetos no board da Mural, use o atalho de teclado **Ctrl+A** (Windows) ou **Cmd+A** (Mac).
2. Para copiar os objetos selecionados, use o atalho de teclado **Ctrl+C** (Windows) ou **Cmd+C** (Mac).
   Seus objetos Mural foram copiados para a sua área de transferência.
3. Na Miro, abra o board onde deseja colar o conteúdo. Use o atalho de teclado **Ctrl+V** (Windows) ou **Cmd+V** (Mac) para colar.

   Você copiou e colou conteúdo com sucesso do Mural para a Miro.
   > ✏️ Conteúdo colado do Mural pode exigir alguns ajustes manuais na Miro. Certos aspectos de estilo e formatação podem parecer diferentes após a colagem.

## Aparência do objeto após colar

Os objetos do Mural geralmente copiam e colam na Miro com algumas variações em relação ao seu estado original. Esta seção descreve os resultados esperados para alguns objetos comuns e fornece as melhores práticas quando aplicável.

### Áreas

Áreas do Muro copiar/colar como quadros e formas da Miro.

Uma área do Mural com 100% de transparência mostrará uma borda transparente mas visível quando colada na Miro. Se a área do Mural tiver um título, esse título aparece e se comporta na Miro como o título de um quadro.

![Área do mural com título e fundo e borda 100% transparentes.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Uma área livre de Mural com título e fundo e borda 100% transparentes*

![Uma área colada do Mural para o Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Uma área colada do Mural para a Miro*

### Conectores

Conectores do Mural copiam e colam como conectores da Miro.

As etiquetas dos conectores, posições verticais e horizontais serão coladas na Miro como centralizadas. A Miro oferece suporte apenas para uma posição centralizada para etiquetas de conectores.

Em relação aos tipos de conector, a Miro oferece suporte a linhas *sólidas*, *pontilhadas* e *tracejadas*. A Mural inclui adicionalmente um tipo de conector *tracejado frouxamente*. Os tipos de conectores do Miro mapeiam os tipos colados do Mural da seguinte forma: *solid* mapeia para *solid*, e o tipo *loosely dashed* do Mural mapeia para o tipo *dashed* do Miro. Outras correspondências diretas (como pontilhado para pontilhado) também são preservadas.

A Miro oferece suporte a cada tipo de curva de conector Mural, embora sua aparência na Miro possa diferir ligeiramente.

![Uma curva de conector do Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Curva do conector do mural*

![Um conector curvo da Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Curva do conector Miro*

### GIFs e imagens

GIFs e imagens que foram originalmente adicionados ao Mural de um URL podem ser copiados e colados na Miro.

:::note
Um GIF ou imagem no Mural que foi carregado diretamente de um dispositivo ou adicionado a partir da barra de ferramentas do Mural não pode ser copiado e colado na Miro usando este método.
:::

### mapas mentais

Mapas mentais do Mural são copiados e colados como mapas mentais da Miro, incluindo o nó raiz, cada nó filho e seu texto.

A formatação do nó raiz é geralmente preservada. No entanto, o raio da forma pode diferir, e o tamanho da fonte do texto não é preservado ao passar do Mural para a Miro.

Os nós filhos do Mural são colados como nós de texto da Miro, e sua formatação não é preservada.

A cor e espessura do conector no mapa mental também podem diferir.

![Um mapa mental copiado no Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)
*Mapa mental copiado no Mural*

![Um mapa mental copiado do Mural para o Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mapa mental copiado para a Miro*

Para mapas mentais do Mural que possuem múltiplos níveis de nós, a ordem dos nós pode mudar ao serem colados na Miro.

![Um mapa mental em Mural com múltiplos níveis de nós.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mapa mental no Mural com múltiplos níveis de nós*

![Um mapa mental com múltiplos níveis de nós copiados do Mural para a Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mapa mental com múltiplos níveis de nós copiados do Mural para a Miro*

:::tip
Mapas mentais copiados do Mural para a Miro podem perder sua escala original. Para redimensionar o mapa mental após colá-lo, você pode esticá-lo manualmente no board da Miro.
:::

### Formas

Formas do Mural geralmente são coladas como formas da Miro. A Miro é compatível com a maioria das formas do Mural diretamente.

No entanto, o Mural inclui 16 formas específicas que não têm um equivalente direto na Miro. Essas formas serão coladas na Miro como retângulos.

![Todas as 16 formas que ao copiar-colar do Mural para o Miro se transformam em retângulos.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*As 16 formas que copiam e colam do Mural para a Miro como retângulos*

### Notas adesivas

Notas adesivas do Mural colam como notas adesivas da Miro.

Miro mapeará a cor e o nível de opacidade da nota adesiva para as correspondências mais próximas disponíveis na Miro.

As seguintes diferenças também podem aparecer ao copiar e colar notas adesivas do Mural para a Miro:

- Notas adesivas circulares do Mural serão coladas na Miro como notas adesivas quadradas.
- Listas dentro de notas adesivas não são preservadas como listas interativas, embora itens individuais apareçam em linhas separadas dentro da nota adesiva da Miro.
- O tamanho da fonte do texto não é preservado, pois as notas adesivas da Miro ajustam automaticamente o tamanho da fonte com base no conteúdo e no tamanho da nota adesiva.
- A rotação aplicada às notas adesivas no Mural não é preservada ao colar.

![Notas adesivas copiadas na Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Notas adesivas copiadas no Mural*

![Notas adesivas copiadas do Mural para o Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Notas adesivas copiadas para Miro*

### Tabelas

Tabelas do Mural colam como tabelas da Miro.

As seguintes diferenças podem aparecer quando você copia e cola tabelas do Mural para a Miro. Para cada um desses itens, você pode normalmente restaurar suas preferências manualmente na Miro após colar:

- Tabelas posicionadas em cima de outros objetos no Mural (como áreas, formas ou imagens) podem ficar parcialmente ocultas atrás desses objetos quando coladas na Miro. Pode ser necessário ajustar o empilhamento (trazer para a frente).
- A cor da borda é ignorada; as bordas serão coladas como cinza.
- A opacidade do plano de fundo é ignorada. Células transparentes no Mural serão coladas como células brancas na Miro. No entanto, a própria cor de fundo (se não for transparente) é geralmente preservada.
- A família de fontes de texto é ignorada; o texto será colado usando a fonte padrão de tabela da Miro (RobertPro).
- A formatação de texto inline, como negrito e itálico, é ignorada dentro de células de tabela.

![](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)Uma tabela com formatação mista copiada em Mural." >

*Tabela com formatação mista copiada no Mural*

![Tabela com formatação mista copiada e colada do Mural para Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Tabela com formatação misturada copiada para a Miro*

### Texto

Objetos de texto do Mural colam como objetos de texto da Miro. As famílias de fontes originais do Mural não são preservadas. A Miro mapeia a família de fontes Mural para a fonte mais próxima disponível na Miro e dimensiona o texto colado para resultados ótimos no board da Miro.
