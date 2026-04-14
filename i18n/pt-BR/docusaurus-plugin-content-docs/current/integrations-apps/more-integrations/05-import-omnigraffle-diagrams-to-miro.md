---
title: Importar diagramas do OmniGraffle para a Miro
article_id: 33541520646674
translation_id: 33541520646674
locale: pt-br
sidebar_position: 11
created_at: '2026-02-23T15:00:35Z'
updated_at: '2026-02-26T09:55:26Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: diagramming
---

Importe facilmente seus diagramas do OmniGraffle para a Miro e comece a colaborar em uma ferramenta unificada. Como o OmniGraffle e a Miro usam modelos de objetos e sistemas de estilo diferentes, os boards importados podem não ter a mesma aparência que os arquivos originais. Você pode precisar revisar e ajustar a formatação após a importação. Para mais informações, consulte as seções [Entenda o mapeamento de objetos do OmniGraffle na Miro](#h_omni_mapping) e [Limitações conhecidas](#h_omni_known_limitations).

## Antes de começar

- Garanta que você pode criar boards na Miro.
- Use o OmniGraffle 7.25.1 (setembro de 2025) ou posterior. Para verificar sua versão, vá para **OmniGraffle > Sobre o OmniGraffle**.
- Revise o conteúdo oculto e as camadas antes de importá-las. Elementos ocultos e em camadas também são importados e aparecerão no board. Se os elementos se sobrepuserem, reorganize-os após a importação.
- Converta preenchimentos de gradiente em cores sólidas antes de exportar. Gradientes não são suportados.

## Importar um arquivo do OmniGraffle para um board da Miro

1. Abra o OmniGraffle, exporte o diagrama no formato
   **.graffle Single File (Zipped)** e salve o
   arquivo
   no seu dispositivo.

   **Nota:** Nós oferecemos suporte apenas para o formato
   **Single File (Zipped)**. Os formatos
   **Package**
   e **Legacy** não são suportados. Se você tiver
   um arquivo exportado não suportado salvo anteriormente, poderá abrir o arquivo no
   OmniGraffle,
   e então exportar para o formato **.graffle Single File (Zipped)**.
2. Abra o board da Miro onde deseja adicionar o diagrama.
3. Arraste e solte o arquivo no formato **.graffle Single File (Zipped)**
   no board do Miro.

## Importar múltiplos arquivos OmniGraffle em massa para o painel do Miro

1. Abra seu painel da Miro.
2. Clique em **+ Criar novo** no canto superior direito.
3. Clique em **Importar** > **Importar do OmniGraffle**.
4. No diálogo de importação, em **Importar para**, selecione o Espaço onde deseja criar os boards da Miro para seus arquivos OmniGraffle importados.
5. Solte seus arquivos **.graffle** na área de carregamento ou clique em **procurar** para selecionar arquivos do seu computador.

   **Nota:** Suportamos apenas o formato **Arquivo Único (Compactado)**. Os formatos **Pacote** e **Legado** não são suportados. Se você tem um arquivo exportado não suportado salvo anteriormente, você pode abri-lo no OmniGraffle e depois exportar para o formato **.graffle Arquivo Único (Compactado)**.
6. Clique em **Importar [X] arquivos**, onde **[X]** é o número real de arquivos que você está importando.
7. Quando você vir a mensagem **Estamos importando seus boards**, clique em **Voltar ao painel**.

### Após iniciar a importação

- A importação ocorre em segundo plano.
- Novos boards aparecem no Espaço que você selecionou durante o processo de importação assim que o processamento for concluído.
- Você receberá uma notificação por e-mail assim que os boards forem criados, incluindo um link direto para o Espaço para que você possa acessá-los rapidamente.

## Verifique o conteúdo importado

Após a conclusão da importação, verifique o seguinte:

- O número esperado de boards foi criado.
- O conteúdo está legível e devidamente posicionado.
- Os conectores estão devidamente conectados.
- A formatação do texto aparece como esperado.
- As principais seções visuais estão intactas.

Para diagramas que evoluirão ao longo do tempo, considere reconstruir áreas altamente complexas usando objetos nativos do Miro para uma melhor editabilidade a longo prazo.

## Perguntas frequentes

Posso importar vários arquivos de uma vez?

Sim. Você pode importar vários arquivos no formato **.graffle Single File (Zipped)** de uma vez. Para mais informações, veja [Importar vários arquivos OmniGraffle para o painel da Miro](#h_omni_bulk_import).

Onde estão os boards para minha importação em massa?

Os boards para sua importação em massa são criados no Espaço que você selecionou durante o [processo de importação](#h_omni_bulk_import). Você também pode clicar no link do e-mail de notificação que recebeu quando os boards foram criados para acessá-los rapidamente. Por fim, se você não especificou o Espaço durante o processo de importação e não tem o e-mail de notificação em mãos, pode procurar seus boards no Espaço de **Arquivos Importados**.

Meu diagrama ficará exatamente igual após a importação?

Na maioria das vezes, sim, mas nem sempre. Fontes, conectores e formatações complexas podem mudar durante a importação. Para mais informações, consulte as seções de [Limitações conhecidas](#h_omni_known_limitations) e [Entender o mapeamento de objetos OmniGraffle no Miro](#h_omni_mapping).

Quanto tempo leva a importação?

O tempo de processamento depende do tamanho e da complexidade do arquivo. Você receberá um e-mail assim que seus boards forem criados, incluindo um link direto para o Espaço para que possa acessá-los rapidamente.

Como saber se minha importação em massa foi bem-sucedida ou falhou?

**Se sua importação em massa for bem-sucedida**, você receberá uma notificação por e-mail assim que os boards forem criados, incluindo um link direto para o Espaço para que você possa acessá-los rapidamente.

**Se sua importação em massa falhar**, você receberá um e-mail informando sobre os arquivos que apresentaram erros na importação.

Próximos passos:

- Entre em contato com o admin do Miro ou com a equipe de Suporte do Miro e informe sobre esse erro.
- Se possível, forneça uma versão **redigida** do arquivo OmniGraffle ao seu admin do Miro, pois isso ajudará na resolução do erro de importação.

Posso desfazer uma importação?

Você não pode desfazer uma importação. Você pode excluir os boards criados, se necessário.

## Solução de problemas

Não vejo a opção Import from OmniGraffle no menu Import

- Confirme que você tem permissão para criar boards na Miro.
- Limpe o cache, atualize o navegador e tente novamente.
- Entre em contato com o Admin da empresa para confirmar que a funcionalidade está ativada para sua organização.

Meu arquivo não carrega

- Certifique-se de exportar o arquivo do OmniGraffle no formato **.graffle Single File (Zipped)**.

  **Nota:** Suportamos apenas o formato **Single File (Zipped)**. Os formatos **Package** e **Legacy** não são suportados. Se você tiver um arquivo exportado não suportado salvo anteriormente, abra o arquivo no OmniGraffle e exporte para o formato **.graffle Single File (Zipped)**.
- Tente carregar um arquivo único em vez de múltiplos arquivos de uma vez.
- Divida diagramas maiores do OmniGraffle em itens menores.

Não recebi um e-mail

- [Verifique a caixa de spam ou de e-mails filtrados.](../../using-miro/tools/troubleshooting/02-allowlist-miro-mailers.md)
- Verifique o Espaço selecionado para boards recém-criados.

O layout parece incorreto

- Reaplique as fontes se houveram substituições.
- Reconecte conectores ou linhas manualmente.
- Edite seções críticas usando formas nativas do Miro, se necessário.

## Compreender o mapeamento de objetos OmniGraffle na Miro

| Funcionalidade nativa de forma na Miro | Disponível para formas importadas do OmniGraffle |
| --- | --- |
| **Estilizando formas**  Você pode personalizar o visual de suas formas usando várias opções de estilização para adaptá-las às suas necessidades e adicionar um toque pessoal aos seus boards. Selecione uma forma para alterar seu estilo, cor e transparência. Você pode selecionar diversas formas de uma só vez e estilizar todas elas. Você também pode estilizar as bordas ao escolher a cor, transparência, espessura, raio dos cantos arredondados e tipo. | Espessura ✅  Opacidade/transparência ✅  Cor ✅  Funcionalidades de seleção múltipla (exceto) transparência ❌  (Transparência pode ser ajustada na seleção múltipla)  Cor da borda ✅  Transparência da borda ✅  Espessura da borda ✅  Tipo de borda ✅ (pontilhada)  Raio da borda das quinas arredondadas ❌ |
| **Alteração de tamanho ou rotação da forma**  Use os nós brancos para alterar as dimensões de uma forma. Arraste o ícone da seta para girar a forma. | ✅ |
| **Convertendo formas**  Você pode converter uma forma em um cartão, caixa de texto, nota adesiva ou qualquer outra forma. | ❌ |
| **Enviar forma para trás ou trazer para frente**  Para enviar a forma para trás e trazer para frente: clique nos três pontos do menu de contexto e escolha uma opção. Ou use os atalhos **Pg Up** e **Pg Dn** (para Windows)/**fn + ↑** e **fn + ↓** (para Mac). | ✅ |
| **Adicionando texto a formas**  Para adicionar texto a uma forma, selecione-a e comece a digitar. As formas têm um limite de 6.000 caracteres. Sinta-se à vontade para usar diferentes opções de formatação de texto: você pode alterar o tamanho do texto, fonte, estilo, alinhamento, cor e destacar o texto.  **Nota:** Marcadores não são compatíveis em formas. Use texto em vez disso. | 🟠  Não é possível adicionar novo texto a formas importadas do OmniGraffle. No entanto, se uma forma importada já contiver texto, você pode editá-lo normalmente (fonte, tamanho, cor, alinhamento e destaque). |
| **Criação rápida de diagramas**  Assim que você selecionar uma forma, uma nota adesiva ou um cartão e passar o mouse sobre um ponto azul perto do objeto, ele mostrará onde uma nova forma ou linha de conexão será criada. Clique no ponto para criar a linha ou o objeto. Se você quiser conectar o objeto a um que seja diferente do sugerido, arraste o ponto e desenhe uma linha de conexão. | ✅  Replica a mesma forma |
| **Dimensões do objeto**  Use as dimensões para criar formas do mesmo tamanho com precisão em todo o seu board. Você pode habilitar as dimensões do objeto nas configurações do seu board. | ✅ |

## Restrições conhecidas

Nesta versão, ao importar arquivos do OmniGraffle para a Miro, você pode notar diferenças na estrutura, estilo ou comportamento devido às diferenças entre as duas plataformas.

### Mapeamento de formas e geometria

**Restrições**

- As formas do OmniGraffle são importadas para a Miro como SVGs ou formas personalizadas, que não suportam a funcionalidade de alternância de tipo da Miro. Se uma forma não puder ser reconhecida e não houver geometria alternativa, ela será padronizada para um retângulo.

**Soluções alternativas**

- Substitua formas críticas por formas nativas da Miro após a importação para restaurar o suporte completo de edição e QDC.
- Tente usar as bibliotecas internas de formas e de prototipagem da Miro, que possuem centenas de formas para muitos casos de uso.
- Revise diagramas complexos após a importação e ajuste manualmente as formas que foram padronizadas para retângulos.

### Fidelidade visual e estilo

**Limitações**

- Gradientes não são suportados. Preenchimentos degradê são achatados durante a importação.
- Sombras não são suportadas e são removidas durante a importação.
- Fontes não suportadas são substituídas por uma fonte do sistema.

**Soluções alternativas**

- Use cores de preenchimento sólido em vez de gradientes antes de exportar.
- Remova efeitos de sombra no OmniGraffle antes de exportar se a precisão visual for crítica.
- Use fontes do sistema amplamente suportadas para reduzir a substituição de fontes.
- Revise tipografia e espaçamento após a importação e ajuste os estilos diretamente no Miro.

### Conectores e anotações

**Limitações**

- As legendas das linhas podem não ser detectadas ou posicionadas corretamente após a importação.
- As linhas podem aparecer divididas, ligeiramente desalinhadas ou passar através de formas.
- As setas direcionais dentro de formas em grupo podem ocasionalmente se perder durante a conversão.

**Soluções Alternativas**

- Reposicione manualmente as etiquetas de texto nas linhas de conexão após a importação.
- Reconecte ou ajuste os conectores no Miro se ocorrerem problemas de alinhamento.

### Formatos de arquivo

**Limitações**

- Suportamos apenas o formato **Arquivo Único (Compactado)**. Os formatos **Pacote** e **Legado** não são suportados.
- Exportações em PNG são importadas como imagens planas, não editáveis.

**Soluções Alternativas**

- Use o formato de exportação **Arquivo Único (Compactado)** para obter os melhores resultados.
- Se você tiver um arquivo exportado não suportado salvo anteriormente, pode abrir o arquivo no OmniGraffle e exportar para o formato **.graffle Arquivo Único (Compactado)**.
- Evite exportações em PNG se precisar de objetos editáveis.

### Comportamento de importação em massa

**Limitações**

- Notificações por e-mail para importações em massa podem ocasionalmente falhar devido a falhas permanentes de entrega.
- Após a conclusão de uma importação em massa, o conteúdo importado pode não aparecer imediatamente no board.

**Soluções alternativas**

- Verifique as regras de spam ou de filtro de e-mails se as notificações não forem recebidas.
- Atualize seu navegador após a conclusão da importação em massa.
