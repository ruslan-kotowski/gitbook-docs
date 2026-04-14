---
title: Números visuais em Tabelas (Beta)
article_id: 31356870414610
translation_id: 31356870414610
locale: pt-br
sidebar_position: 18
created_at: '2025-11-25T19:40:55Z'
updated_at: '2026-03-13T12:26:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: tables
availability:
  notes: 'Quem pode fazer: Editores de boards Quais planos: Business, Enterprise Quais
    plataformas: Navegador, Desktop, Mobile'
---

O Visual Numbers permite que os usuários transformem números em barras de progresso visuais. Os usuários podem definir regras de formatação condicional com cores personalizadas e definir intervalos mínimo/máximo para melhor visualização de dados. O Visual Numbers também permite formatação em porcentagem ou moeda.

## Formate números visualmente

A formatação de números visuais transforma dados numéricos em barras de progresso, facilitando a identificação de tendências e o acompanhamento do progresso de forma rápida. Você pode exibir números como porcentagens ou moedas, definir intervalos personalizados e aplicar regras de formatação condicional.

Aplicar formatação visual a um campo numérico:

1. Passe o cursor sobre o nome de um campo de número ou fórmula para exibir o ícone **três pontos** (**...**).
2. Clique no ícone **três pontos** (**...**) e selecione **Editar campo**.
3. Na seção **Exibição** da caixa de diálogo, clique em **Barra**.
   Os números serão exibidos como barras de progresso.
4. Escolha o seu formato:
   1. Porcentagem (%): Melhor para taxas de conclusão, acompanhamento de progresso.
   2. Moeda: Selecione entre as principais moedas ($, €, £, ¥ e mais).
5. Defina o intervalo de **Mín** e **Máx** para suas barras de progresso. Para percentuais, normalmente use 0-100. Para moeda, defina valores mínimos/máximos apropriados para seus dados.
6. Escolha uma cor de barra no seletor de cores.
7. Ative ou desative as etiquetas numéricas:
   1. Ligado: Mostra o valor numérico juntamente com a barra de progresso.
   2. Desligado: Mostra apenas a barra de progresso para uma visualização mais limpa.
8. Clique em **Salvar**.

## Aplicar formatação condicional

O formato condicional aplica cores automaticamente às suas barras de progresso com base em regras que você define, ajudando a identificar rapidamente os valores que precisam de atenção.

1. Abra as **Configurações de campo** para um campo numérico ou de fórmula.
2. Ative as **Cores condicionais**.
3. Clique em **Adicionar regra**.
4. Defina sua regra:
   1. Selecione uma condição (igual a, diferente de, maior que, menor que, maior ou igual a, menor ou igual a, está vazio, não está vazio).
   2. Insira o valor para comparar (se aplicável).
   3. Escolha uma cor para valores que correspondem a esta regra.
5. Adicione várias regras conforme necessário. Arraste e solte regras para definir sua prioridade. Regras no topo têm precedência.
6. Clique em **Salvar**.

A formatação condicional aparece tanto na visualização de tabelas como no painel lateral ao visualizar registros individuais.

O formato visual de números está disponível atualmente apenas na visualização de Tabelas e no painel lateral.

As visualizações de Timeline, Kanban e cartões exibirão formatação numérica padrão.
