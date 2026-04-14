---
title: Importe diagramas do Lucidchart para a Miro
article_id: 11840840023058
translation_id: 11840840023058
locale: pt-br
sidebar_position: 6
created_at: '2023-06-06T08:50:22Z'
updated_at: '2025-11-25T15:37:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Pessoas: Todos os usuários Planos: Starter, Business, Enterprise, Education
    Plataformas: navegador, desktop'
---

Você pode importar seus diagramas do Lucidchart para a Miro para colaborar com seu time e usar os extensos recursos da Miro. Este guia mostra duas maneiras de importar seu conteúdo: de um board da Miro ou diretamente do seu painel.

:::warning
A edição do conteúdo importado é um processo unidirecional. As alterações que você fizer na Miro não serão sincronizadas de volta para o Lucidchart.
:::

:::note
Você pode migrar boards do Lucidchart que estão sob uma licença Free ou Limitada.
:::

## Importar de um board da Miro

Siga estas etapas para importar seus diagramas do Lucidchart enquanto trabalha em um board da Miro.

1. No Lucidchart, exporte o diagrama que deseja no formato **VSDX** e salve o arquivo no seu dispositivo.
2. Abra o board da Miro onde deseja adicionar o diagrama.
3. Na barra de ferramentas de criação à esquerda, clique em **Formas** (![icon-shapes.svg](../../../../../../docs/getting-started/migrating-content-to-miro/images/25121485636114_icon-shapes.svg)), selecione **Mais formas** e clique no ícone **Importar diagrama** no canto superior direito do painel de diagramas.
4. Na caixa de diálogo de importação, arraste e solte o arquivo `.vsdx` exportado do Lucidchart, ou clique em **Escolher arquivo** para selecioná-lo manualmente. Você pode importar vários arquivos de uma só vez.
5. Clique em **Importar**. Um novo board é criado para cada arquivo `.vsdx` importado.

> Embora a maior parte do conteúdo seja transferida suavemente, você pode precisar fazer ajustes menores no estilo e formatação. Veja a seção Como os objetos do Lucidchart aparecem na Miro para mais detalhes.

## Importar do painel da Miro

Você também pode importar seus diagramas diretamente do painel da Miro sem abrir um board primeiro.

1. No Lucidchart, exporte seu diagrama como um arquivo `.vsdx` indo para **Arquivo > Exportar >** `.vsdx`.
2. Vá para o painel da Miro.
3. Clique no botão **Criar novo**, selecione **Importar** e, em seguida, escolha **Importar do Lucidchart**.
4. Na janela que se abre, arraste e solte seu(s) arquivo(s) `.vsdx` ou clique em **Procurar** para selecioná-los.
5. (Opcional) Use o **menu suspenso Escolher Espaço** para selecionar um [Espaço](../../using-miro/spaces/01-spaces.md) para os seus boards importados. Se você não escolher um, os boards serão adicionados ao seu espaço principal do time.
6. Clique em **Criar boards** para iniciar a importação.
7. Uma mensagem confirmará que a importação está em andamento. Você receberá uma notificação por e-mail quando seus novos boards da Miro estiverem prontos.

## Como os objetos do Lucidchart aparecem na Miro

Devido às diferenças entre as plataformas, alguns objetos do Lucidchart são convertidos em tipos diferentes de objetos na Miro. Esta tabela fornece uma comparação abrangente.

|  |  |
| --- | --- |
| **Lucidchart** | **Miro** |
| Bloco | Texto, Formas |
| Contêineres | Formas |
| Documentos | 🟠 Pode ser recriado manualmente |
| Chave de diagrama | Texto, Formas |
| Quadros | Quadros e Formas |
| GIFs | Imagens |
| Hotspot | Link para |
| Imagens | Imagens |
| Linha | Conectores |
| Organogramas | Formas, imagens |
| Formas | Formas |
| Contêineres inteligentes | Formas |
| Tabelas inteligentes | Formas |
| Nota adesiva | Notas adesivas |
| Tabelas | Formas |
| Texto | Texto |
| Linha do tempo | Formas |
| Atividades visuais | Formas |
| **Outras propriedades** | |
| Autores | 🟠 Pode ser recriado manualmente |
| Colaboradores e compartilhamento | 🟠 Pode ser recriado manualmente |
| Comentários | 🟠 Pode ser recriado manualmente |
| Agrupamento | Importado |
| Conjuntos de ícones | Anexado a Formas |
| Camadas | 🟠 Pode ser recriado manualmente |
| Link para | Importado |
| Bloquear | 🟠 Pode ser recriado manualmente |
| Notas/Anotações | 🟠 Pode ser recriado manualmente |
| **Formas** | |
| **Pacotes de formas do Lucidchart** | **Formas da Miro** |
| Arquitetura AWS | Formas > AWS |
| Azure | Formas > Azure |
| BPMN 2.0 | Formas > BPMN |
| Diagramas de circuito | Importado e editável, mas indisponível na galeria de formas da Miro |
| Fluxo de dados | Formas > Fluxo de dados |
| Formas dinâmicas | Importado e editável, mas indisponível na galeria de formas da Miro |
| Arquitetura Enterprise | Importado e editável, mas indisponível na galeria de formas da Miro |
| Integrações Enterprise | Importado e editável, mas indisponível na galeria de formas da Miro |
| Entidade e Relacionamento | Formas > ERD |
| Equações | Importado e editável, mas indisponível na galeria de formas da Miro |
| Plantas baixas | Importado e editável, mas indisponível na galeria de formas da Miro |
| Formas de fluxograma | Formas > Fluxograma |
| Formas geométricas | Formas |
| Plataforma Google Cloud | Formas > GCP |
| Kubernetes | Formas > Kuberenetes |
| Mapas mentais | Mapas mentais |
| Infraestrutura de rede | Importado e editável, mas indisponível na galeria de formas da Miro |
| Engenharia de Processos | Importado e editável, mas indisponível na galeria de formas da Miro |
| Arquitetura Salesforce | Formas > Salesforce |
| Diagramas de rack de servidor | Importado e editável, mas indisponível na galeria de formas da Miro |
| Mapas do site | Importado e editável, mas indisponível na galeria de formas da Miro |
| Formas padrão | Formas |
| Clipart de tecnologia | Importado e editável, mas indisponível na galeria de formas da Miro |
| Mockups de UI | Importado e editável, mas indisponível na galeria de formas da Miro |
| Linguagem de modelagem unificada (UML) | Formas > UML |
| Fluxo de valor | Formas > Mapeamento de fluxo de valor |
| Diagramas de Venn | Importado e editável, mas indisponível na galeria de formas da Miro |

## Restrições

Embora o Lucidchart e a Miro ofereçam funcionalidades semelhantes, podem existir algumas diferenças:

- As caixas de texto da Miro podem acomodar até 6.000 caracteres, incluindo espaços. Qualquer texto adicional será cortado.
- As notas adesivas da Miro são incompatíveis com rotação, ajustes de paleta de cores ou texto com marcadores.
- Alguns pacotes de formas disponíveis no Lucidchart não estão disponíveis na Miro. Eles ainda podem ser importados, e os usuários podem duplicar e editar essas formas. No entanto, não estarão disponíveis na galeria de formas da Miro.
- Comentários, notas e anotações não podem ser migrados do Lucidchart para a Miro, pois o Lucidchart não os exporta.

:::note
Para mais dúvidas e suporte sobre a migração do Lucidchart, entre em contato com o [Suporte da Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) ou fale diretamente com seu Gerente de Sucesso do Cliente da Miro.
:::
