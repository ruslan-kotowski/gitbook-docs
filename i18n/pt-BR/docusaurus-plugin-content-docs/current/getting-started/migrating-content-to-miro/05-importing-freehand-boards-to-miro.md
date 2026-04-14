---
title: Importar boards do Freehand para a Miro
article_id: 18580556555538
translation_id: 18580556555538
locale: pt-br
sidebar_position: 9
created_at: '2024-04-26T16:34:28Z'
updated_at: '2025-11-25T15:42:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Pessoas: Todos os usuários com planos elegíveis Planos: Starter, Business,
    Education e Enterprise Plataformas: Navegador, desktop, dispositivo móvel (para
    acessar a Miro e iniciar a importação)'
---

Este artigo explica como importar boards do Freehand para a Miro, incluindo como preparar seus boards do Freehand, para importações individuais e em massa.

:::note
Edições que você faz no conteúdo importado na Miro não são sincronizadas com seu conteúdo original no Freehand.
:::

:::note
Você só pode importar boards do Freehand que estão sob licenças Gratuita ou Restrita.
:::

## Importar um único board do Freehand para a Miro

Você pode facilmente importar boards individuais do Freehand para a Miro exportando-os no formato de arquivo `.RTB` da Miro. Veja como fazê-lo:

1. Acesse o board do Freehand que deseja exportar para a Miro.
2. Baixe o arquivo em .RTB, formato proprietário da Miro, diretamente do Freehand. Navegue até o menu **Ferramentas** e selecione **Exportar para board da Miro**. O arquivo será salvo em sua pasta de download padrão. O Freehand enviará uma notificação assim que o download for concluído.
3. Abra seu painel da Miro.
4. Na área superior direita do painel da Miro, clique no botão **+ Criar novo**, clique em **Importar** e, em seguida, clique em **Importar backup**.
5. Escolha o arquivo `.RTB` baixado anteriormente do seu sistema.
6. Agora todo o conteúdo foi importado para um novo board da Miro em formato editável.
7. Embora a transição da maior parte do conteúdo seja perfeita, pequenos ajustes podem ser necessários devido a variações nas opções de estilo e formatação entre o Freehand e a Miro. Leia Como os objetos do Freehand aparecem na Miro para mais informações sobre possíveis diferenças.

## Importação em massa de vários arquivos do Freehand para a Miro

Para migrar vários boards do Freehand de uma só vez, a Miro oferece um processo de importação em massa. Primeiro, certifique-se de que seus boards Freehand estejam preparados corretamente.

**Pré-requisitos: Prepare seus boards do Freehand para importação em massa**

Siga estas etapas no Freehand para preparar seus boards:

1. No Freehand, no menu à esquerda, selecione **Documents**. Um menu suspenso é aberto.
2. Selecione **Todos os Documentos** ou **Criados por Mim**, e especifique o período para os boards que deseja importar para a Miro.
3. Para cada board que você deseja importar, selecione os três pontos (**...**) e escolha **Selecionar**.
4. Na caixa de diálogo na parte inferior da tela, selecione **Mover**.
5. Selecione um Espaço para mover seus boards. Isso os consolida para facilitar o processamento pela ferramenta de importação em massa.

   Você preparou com sucesso vários arquivos para importação em massa para a Miro.

Para realizar a importação em massa dos seus boards do Freehand preparados para a Miro, siga as instruções fornecidas no guia incorporado do board Miro a seguir:

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="460" scrolling="no" src="https://miro.com/app/embed/uXjVKB1IT00=/?pres=1&amp;frameId=3458764590689727256&amp;embedId=507813406404&amp;&amp;autoplay=yep" width="100%"></iframe>

:::note
Notas Importantes para Importação em Massa:
- O token do Freehand usado para migração em massa é válido apenas por duas semanas a partir da data em que você o recebeu.
- A partir de 31 de dezembro de 2024, de 23h59 EST em diante, o Freehand e todos os tokens de migração associados serão descontinuados e invalidados. Os usuários não poderão mais gerar novos tokens ou acessar o Freehand para migração.
:::

## Reveja as práticas recomendadas

Para uma experiência de migração fluida, é importante entender as melhores práticas e considerações chave ao mover seu conteúdo do Freehand para a Miro. Revise a orientação detalhada no board inserido da Miro abaixo:

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="460" scrolling="no" src="https://miro.com/app/embed/uXjVKB1FWSM=/?pres=1&amp;frameId=3458764590691451227&amp;embedId=480338444592&amp;autoplay=yep" width="100%"></iframe>

## Mapeamento de objetos na Miro

Esta tabela fornece uma comparação abrangente de como os objetos do Freehand são tipicamente importados e representados na Miro, juntamente com notas sobre quaisquer ajustes manuais que possam ser necessários:

|  |  |  |
| --- | --- | --- |
| **Freehand** | **a Miro** | **Retoques necessários** |
| Boards | Kanban | Nenhum |
| Cartões | Cartões | Os cartões do Jira no Freehand serão importados como cartões do Jira na Miro. No entanto, não serão conectados à instância existente, pois os usuários precisarão autenticar novamente suas contas do Jira na Miro.    Os cartões do ADO, Trello e Asana não são compatíveis. |
| Colaboradores e compartilhamento | Pode ser recriado manualmente | Nenhum |
| Comentários | Pode ser recriado manualmente | Nenhum |
| Conectores/Linhas | Conectores/Linhas | Nenhum |
| Desenhos/Diagramas/Formas | Formas, Texto e Conectores | Nenhum |
| Tabelas de dados dinâmicos | CSV | O conteúdo pode ser baixado e editado como um arquivo .CSV no board da Miro. |
| Inserções:    Google e Microsoft Docs, YouTube, Spotify, Loom | Nome da fonte (por exemplo, Google, YouTube) e o URL para o arquivo incorporado | Se os usuários desejarem reincorporar um documento, poderão [fazer upload via URL](../../using-miro/import-and-export/import/05-uploading-files-to-boards.md). |
| Reações com emoji | Pode ser recriado manualmente | Nenhum |
| Quadros | Quadros | Nenhum |
| Grades (tabelas) | Tabelas | Nenhum |
| Objetos agrupados | Objetos desagrupados | Para reagrupar objetos, selecione todos os objetos relevantes e pressione **Cmd/Ctrl + G** ou clique em **Agrupar objetos** no menu de contexto. |
| Imagens | Imagens | Nenhum |
| Páginas | Documento incorporado | O conteúdo pode ser baixado e editado como um arquivo .docx no board da Miro. |
| Protótipos | Nome da fonte (InVision) e URL do arquivo incorporado. | Se os usuários desejarem incorporar novamente um documento, eles podem Carregar via URL para reincorporar. |
| Widgets inteligentes:    Cartões dupla face, enquete, Isto ou Aquilo, gráficos, contador, placar, roleta, campainha, pessoas, story points, t-shirt size, cronômetro, botões de ação. | O PNG do widget inteligente é criado no momento da importação. | O conteúdo não é editável. |
| Notas adesivas | Notas adesivas | Os tamanhos das fontes do texto nas notas adesivas podem precisar de ajuste. |
| Linha do tempo (Gantt) | CSV | O conteúdo pode ser baixado e editado como um arquivo .CSV no board da Miro. |
| Wireframes | Wireframes | Alguns objetos podem precisar ser redesenhados. |

## Principais limitações

Esteja ciente das seguintes limitações e diferenças estruturais ao migrar seu conteúdo do Freehand para a Miro para garantir uma transição mais suave:

- As caixas de texto da Miro podem acomodar até 6.000 caracteres, incluindo espaços. Qualquer texto adicional será cortado.
- As notas adesivas da Miro são incompatíveis com ajustes de paleta de cores ou texto com marcadores da mesma forma que o Freehand; algumas formatações podem diferir.
- Os widgets Freehand Smart são importados como imagens estáticas (PNGs) e não são editáveis na Miro.
- Comentários, reações de emoji e protótipos do Freehand não são migrados para a Miro.
- O token do Freehand necessário para importação em massa é válido apenas por duas semanas a partir da data em que você o recebeu.
- A partir de 31 de dezembro de 2024, de 23h59 EST em diante, o Freehand e todos os tokens de migração associados serão descontinuados e invalidados. Os usuários não poderão mais gerar novos tokens ou acessar o Freehand.

### Compare a estrutura organizacional entre o Freehand e a Miro

Para planejar efetivamente sua migração, é importante entender como as estruturas organizacionais no Freehand correspondem às da Miro:

**Camadas organizacionais do Freehand**

- Times: Cada subdomínio ao qual você tem acesso no InVision é considerado um time. Se tiver acesso apenas a um subdomínio, você terá apenas um time.
- Grupos: Pastas de documentos que ajudam a agrupar e compartilhar documentos com seu time.
- Espaços: uma camada adicional de organização dentro dos grupos para seus documentos.

:::note
Se o seu time utilizou o recurso de visão geral do Espaço no Freehand, você precisará migrar manualmente esse conteúdo para a Miro. Recomendamos copiar o conteúdo da visão geral do Espaço para um board da Miro.
:::

**Camadas organizacionais da Miro**

- Organizações: Normalmente, você tem acesso a uma única organização na Miro.
- Times: Espaços de trabalho compartilhados onde os usuários colaboram em boards e projetos (anteriormente conhecidos como Espaços em alguns contextos, fique atento à terminologia em evolução da Miro; geralmente, os times são o principal espaço de trabalho colaborativo).
- Projetos: Coleções de boards dentro de um time, facilitando a organização, recuperação e compartilhamento de boards.

Considere seus grupos no InVision aproximadamente equivalentes aos projetos na Miro (ou ao que poderia ter sido conceitualmente semelhante a pastas/espaços para organizar boards dentro de um time). Para cada grupo do InVision que você planeja migrar, recomendamos criar um projeto na Miro com o mesmo nome. Por exemplo, se você tivesse um grupo no InVision chamado "Acme Corp Relaunch Project", sugerimos que crie um Projeto da Miro com o mesmo nome, "Acme Corp Relaunch Project", dentro do time adequado da Miro.

:::tip
Para mais dúvidas sobre a migração do Freehand, entre em contato com [Suporte da Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) ou fale diretamente com seu Gerente de Sucesso do Cliente da Miro.
:::
