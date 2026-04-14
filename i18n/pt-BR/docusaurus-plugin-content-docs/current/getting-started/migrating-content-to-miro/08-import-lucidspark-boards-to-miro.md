---
title: Importe boards do Lucidspark para a Miro
article_id: 9549014537490
translation_id: 9549014537490
locale: pt-br
sidebar_position: 7
created_at: '2023-01-12T09:05:07Z'
updated_at: '2026-01-19T14:30:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Pessoas: Qualquer usuário com acesso de edição a ambos os boards do Lucidspark
    e da Miro Planos: Free, Starter, Business, Education e Enterprise Plataformas:
    Navegador, Desktop'
---

Migre seu conteúdo do Lucidspark facilmente para a Miro para uma experiência de colaboração mais poderosa. Este guia descreve como importar seus boards e o que esperar durante o processo.

> **Aviso:** A edição do conteúdo importado é unidirecional. As alterações feitas na Miro não serão sincronizadas com o Lucidspark.

> **Nota:** Os boards do Lucidspark sob licenças Free ou Restritas podem ser migrados.

## Como importar boards do Lucidspark via exportação em PDF

Siga estas etapas para importar seus boards do Lucidspark para o Miro usando o método de exportação em PDF:

1. Certifique-se de exportar o conteúdo **Lucidspark** que você deseja importar para o Miro como um PDF.
2. No **painel** inicial do Miro, clique em **+ Criar novo**.
3. Selecione **Importar** e depois **Importar do Lucidspark**.
   O modal de **Importar do Lucidspark** será aberto. Você pode importar em massa vários PDFs do Lucidspark.
4. Siga as instruções na tela fornecidas pelo modal.
5. Selecione **Importar boards**.
6. Revise o conteúdo importado e faça os ajustes necessários. Embora o Lucidspark e a Miro tenham funcionalidades semelhantes, ainda pode haver diferenças nas opções de estilo e formatação. Consulte [Como os objetos do Lucidspark aparecem na Miro (Método de Importação em Massa de PDF)](#lucidspark-object-mapping-bulk-import) para obter orientação sobre como os objetos são traduzidos.

## Método alternativo: Copiar e colar conteúdo

Como uma alternativa mais rápida para menores volumes de conteúdo, você pode copiar diretamente elementos de um board aberto do Lucidspark e colá-los em um board da Miro.

> **Nota:** Qualquer usuário com acesso de edição aos boards do Lucidspark e da Miro poderá copiar o conteúdo do Lucidspark e colá-lo na Miro. Para detalhes sobre como os objetos são transformados com este método, consulte [Como os objetos do Lucidspark aparecem na Miro (Método de Copiar/Colar)](#lucidspark-object-mapping-copy-paste).

## Como os objetos do Lucidspark aparecem na Miro (Método de Copiar/Colar)

Esta tabela oferece uma comparação abrangente de como os objetos são transformados quando você copia conteúdo diretamente do Lucidspark e cola na Miro.

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Cartões do Azure | Os cartões do Azure são migrados como cartões da Miro: 1. Configure a integração do Azure na Miro. 2. Converta os cartões da Miro para [cartões do Azure](../../integrations-apps/microsoft/03-azure-cards.md). |
| Colaboradores e compartilhamento | 🟠 Podem ser recriados manualmente |
| Comentários | 🟠 Podem ser recriados manualmente |
| Conectores e divisores | Conectores |
| Contêineres | Formas |
| Documentos de arquivos e URLs | 🟠 Pode ser recriado manualmente |
| URLs de documentos (PDF) | Documentos incorporados |
| Desenhos | Imagens |
| Tabelas dinâmicas | Tabelas |
| Emojis | Imagens |
| Quadros | Quadros |
| GIFs da Barra de ferramentas | Imagens |
| GIFs de arquivos | Imagens |
| GIFs de URLs | GIFs |
| Imagens | Imagens |
| Cartões do Jira | Os cartões do Jira são migrados como cartões da Miro:  1. Configure a integração do Jira na Miro 2. Converta os cartões da Miro em [cartões do Jira](../../integrations-apps/atlassian/03-jira-cards.md). |
| Cartões Lucid | Cartões |
| Mapa mental | Mapa mental |
| Formas | Formas |
| Nota adesiva | Notas adesivas |
| Tabelas | Tabelas |
| Texto | Texto |
| Linha do tempo | 🟠 Pode ser recriado manualmente |
| Vídeos e outros URLs | Pré-visualizações |

## Como os objetos do Lucidspark aparecem na Miro (Método de Importação de PDF em Massa)

Esta tabela fornece uma comparação abrangente de objetos entre o Lucidspark e a Miro após a importação em massa do conteúdo via PDF.

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Cartões do Azure | Imagens |
| Colaboradores e compartilhamento | 🟠 Pode ser recriado manualmente |
| Comentários | 🟠 Pode ser recriado manualmente |
| Conectores e Divisores | Conectores |
| Containers | Formas |
| Documentos | 🟠 Pode ser recriado manualmente |
| Desenhar | Linhas |
| Tabelas dinâmicas | Formas e Conectores |
| Emojis | Imagens |
| Quadros | Quadros e Formas |
| GIFs | Imagens |
| Imagens | Imagens |
| Cartões do Jira | Formas |
| Cartões Lucid | Formas |
| Mapa mental | Formas e Conectores |
| Formas | Formas |
| Nota adesiva | Notas adesivas |
| Tabelas | Tabelas/Formas e Conectores |
| Texto | Texto |
| Linha do tempo | Formas e conectores |
| Vídeos e outras URLs | 🟠 Podem ser recriados manualmente |

## Limitações da importação

Embora Lucidspark e Miro ofereçam funcionalidades semelhantes, esteja ciente das seguintes diferenças e limitações ao importar conteúdo:

- As caixas de texto da Miro podem acomodar até 6.000 caracteres, incluindo espaços. Qualquer texto adicional será cortado.
- As cores e os estilos são mapeados para as correspondências mais próximas na Miro.
- Os valores de opacidade do Lucidspark não são extraídos com precisão durante a importação.
- As notas adesivas da Miro são incompatíveis com rotação, ajustes de paleta de cores ou texto com marcadores que possam ter sido aplicados no Lucidspark.

## Obtendo ajuda

> **Nota:** Para mais dúvidas e suporte sobre a migração do Lucidspark, entre em contato com o [Suporte da Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) ou fale diretamente com seu Gerente de Sucesso do Cliente da Miro.
