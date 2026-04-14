---
title: Importador Whiteboards.io para Miro
article_id: 20624350720402
translation_id: 20624350720402
locale: pt-br
sidebar_position: 3
created_at: '2024-08-07T16:30:40Z'
updated_at: '2026-01-19T14:08:30Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: export-pdf-canvas
---

O Whiteboards.io Importer for Miro da ServiceRocket é uma solução amigável projetada para agilizar a importação de dados do  aplicativo [Whiteboards.io](https://whiteboards.io/)para[o Miro](https://miro.com/app/dashboard/). Carregue seus backups gerados pelo Whiteboard com rapidez e facilidade.

Obtenha acesso ao importador hoje mesmo. Visita `https://www.servicerocket.com/miro/whiteboards-io-miro-migration` para mais detalhes.

## **Exportando boards do Whiteboards.io**

1. Faça login no [Whiteboards.io](https://whiteboards.io/).
2. Na página principal, clique em Exportar boards na mensagem de status de aviso.

*Clique em Exportar boards na mensagem de status de aviso para começar*

3. Em seguida, execute as seguintes etapas para exportar o board.

*Verifique se as configurações estão corretas ao exportar sua board*

1. 1. Selecione somente o formato .json.
   2. Desmarque incluir mídia (imagens, vídeos e outros arquivos).
   3. Clique em Exportar para confirmar as configurações e exportar o board.

4. Um arquivo .zip será gerado com sucesso.

## **Importando boards Whiteboards.io para o Miro**

1. Abra seu board da Miro.
2. Na barra de ferramentas, clique em Mais aplicativos > selecione ou pesquise por Whiteboards.io Miro Importer.
3. Clique em Escolher arquivo para carregar o arquivo (.zip) gerado pelo aplicativo[Whiteboards.io](http://whiteboards.io/) .
4. Em seguida, selecione a board que deseja importar e clique em Importar.
5. Quando a importação estiver concluída, o sistema mostrará o status do board como CONCLUÍDO.
6. Feche o aplicativo e retorne à página principal do Miro. O aplicativo importará os boards selecionados para sua conta de time .

## **Mapeamento de dados do Whiteboards.io no Miro**

O mapeamento de dados é essencial para manter a integridade dos dados, a consistência e as diferenças de esquema durante a transição de um aplicativo para outro. As tabelas abaixo listam toda a terminologia equivalente, estruturas de dados, nomes de campos, formatos e muito mais.

|  |  |  |
| --- | --- | --- |
| **Quadros brancos.io** | **Miro** | **Notas** |
| Texto | [Texto](https://developers.miro.com/docs/text-1) | N/D |
| Forma | [Forma](https://developers.miro.com/docs/shape-1) | - O forma de coração será importado como um forma de nuvem. - O forma paperTape será importado como um forma de fluxograma flowchart_input_output. - Um ícone será importado como uma imagem. |
| Cartão | [Nota adesiva](https://developers.miro.com/docs/stickynote-1) | - A formatação da fonte será perdida ao converter para um cartão. - A cor do cartão será perdida e o alinhamento ficará incorreto. - O tamanho do nota adesiva-it pode ser diferente. |
| Linha | [Conector](https://developers.miro.com/docs/connector_intro) | N/D |
| Quadro, quadro | [Quadro, quadro](https://developers.miro.com/docs/frame-1) | Objetos filhos do quadro não podem ser vinculados ao quadro pai. |
| Sorteio Free | [Imagem](https://developers.miro.com/docs/image-1) (.svg) | N/D |
| Comentários | N/D | Não há nenhum método fornecido no Miro para mapear isso. |
| Arquivo | [Arquivo](../../troubleshooting-technical-questions/technical-guidelines/03-supported-file-formats.md) | Tipo e formato de arquivo:   - Imagens - Tabelas e planilhas - Documentos de texto - Apresentações |
| Imagem | [Imagem](https://developers.miro.com/docs/image-1) | N/D |
| Incorporar iFrame | [Inserir](https://developers.miro.com/docs/embed-2) | N/D |
| Mesa de cartas | [Cartão](https://developers.miro.com/docs/card-1) e [quadro](https://developers.miro.com/docs/frame-1) | Sem o nome da coluna e da raia. |
| Mapa mental | [Mapa mental](https://developers.miro.com/docs/mind-maps) (Experimental) | A cor da borda não é suportada. |
| Cartão GitHub | [Cartão](https://developers.miro.com/docs/card-1) | N/D |
| Cartão do Jira | Texto com URL do problema do Jira | N/D |
