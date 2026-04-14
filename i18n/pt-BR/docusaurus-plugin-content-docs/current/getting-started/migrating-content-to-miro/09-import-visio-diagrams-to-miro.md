---
title: Importar diagramas do Visio para a Miro
article_id: 11842818558738
translation_id: 11842818558738
locale: pt-br
sidebar_position: 8
created_at: '2023-06-06T10:11:36Z'
updated_at: '2026-02-16T14:27:52Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Pessoas: Todos os usuários com planos elegíveis Planos: Business e Enterprise
    Plataformas: navegador, desktop, dispositivo móvel'
---

Transfira facilmente seus diagramas do MS Visio para a Miro e comece a colaborar em uma ferramenta unificada.

Os diagramas importados são totalmente funcionais para que você possa editar, colorir, mover e redesenhar conforme necessário.

:::warning
A edição de diagramas importados é unidirecional. As alterações feitas na Miro não serão refletidas no Visio.
:::

## Importar um único diagrama do Visio para um novo board da Miro

Siga estas etapas para importar um diagrama individual do Visio. O diagrama importado criará um novo board da Miro:

1. No Visio, abra o diagrama que deseja exportar.
2. Selecione o menu **Arquivo** e escolha **Salvar como**. Selecione um local e salve seu arquivo no formato `.vsdx`.
3. Navegue até o board da Miro de onde você quer iniciar a importação. Pode ser qualquer board, pois a importação criará um novo.
4. Na barra de ferramentas de criação à esquerda, selecione **Formas** > **Mais formas**, e então selecione o ícone **Importar diagrama** localizado no canto superior direito do painel da galeria de formas de diagramação.
5. Na caixa de diálogo que aparece, arraste e solte o arquivo `.vsdx` do Visio ou clique no botão **Escolher arquivo** e navegue para selecionar o arquivo no seu sistema.
6. Selecione **Importar**.
   Quando o processo de importação terminar, você verá um diálogo de **Arquivo importado**.
7. Clique em **Ir para o board** para abrir o novo board da Miro contendo seu diagrama importado.

## Importação em massa de múltiplos diagramas do Visio

Você também pode importar vários diagramas do Visio para a Miro simultaneamente a partir do seu painel. Cada diagrama será importado para um novo board da Miro, nomeado de acordo com o nome do arquivo original:

1. Vá para o seu [painel da Miro](https://miro.com/app/dashboard/).
2. Selecione **+ Criar novo** > **Importar** > **Importar diagrama**.
3. Arraste seus arquivos `.vsdx` para a área designada ou use o link **escolher arquivos** para selecionar vários diagramas do Visio. Observe que você ainda pode remover arquivos antes de importar.
4. Selecione **Importar arquivos**.
   Quando o processo de importação terminar, você verá um diálogo **Arquivos importados**.
5. Selecione **Concluir**.

Isso cria um novo board para cada diagrama, nomeado a partir do nome original do arquivo.

## Entenda o mapeamento de objetos Visio na Miro

A tabela a seguir compara como objetos e formas do Visio são normalmente representados após serem importados para a Miro. Observe que, embora a Miro se esforce para uma alta fidelidade, alguns ajustes manuais ou recriações podem ser necessários para elementos complexos.

| **Visio** | **Miro** |
| --- | --- |
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
| Notas/anotações | 🟠 Pode ser recriado manualmente |
| **Formas** | |
| **Formas Visio** | **Formas da Miro** |
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
| Kubernetes | Formas > Kubernetes |
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
