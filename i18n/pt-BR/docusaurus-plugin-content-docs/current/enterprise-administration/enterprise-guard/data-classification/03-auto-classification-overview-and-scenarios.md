---
title: "Vis\xE3o geral e cen\xE1rios da classifica\xE7\xE3o autom\xE1tica"
article_id: 15431302000914
translation_id: 15431302000914
locale: pt-br
sidebar_position: 2
created_at: '2023-11-29T16:42:42Z'
updated_at: '2025-11-25T15:39:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Para proteger seu conteúdo sensível, o Enterprise Guard inclui a funcionalidade de classificação automática, um processo de classificação automática de dados, que categoriza os boards da Miro com base no seu nível de conteúdo sensível. A classificação automática representa um avanço importante na maneira como você gerencia e protege seus dados confidenciais. A automação do processo de classificação permite que sua organização reforce o nível de segurança dos dados, atenda aos requisitos regulatórios e forneça uma melhor experiência de admin de segurança. A transição da classificação manual para a automática é um passo estratégico em prol de uma estrutura de segurança de dados mais precisa, segura e eficiente.

## Entenda os cenários de classificação automática

### Pré-requisitos

Para usar a funcionalidade de classificação automática, você deve:

- [Habilitar a descoberta de dados](../data-discovery/13-activate-privacy-related-data-discovery.md).
- [Definir os níveis de classificação](07-define-classification-levels.md).

### Exemplo de configuração da classificação automática e das proteções

Você deve [configurar a classificação automática e as proteções](https://help.miro.com/hc/articles/15853672236946) com base nos seus requisitos de segurança e governança. A tabela a seguir mostra a configuração usada para todos os exemplos de cenários desta página, sendo apenas para fins explicativos.

|  |  |  |  |
| --- | --- | --- | --- |
| **Classificação de boards** | **Grau de sensibilidade** | **Critérios de classificação automática** | **Proteções** |
| PÚBLICO | 1  (menos sensível) | Nenhum | Nenhum |
| INTERNO (padrão) | 2 | TELECOMUNICAÇÕES | - Bloquear o compartilhamento público |
| CONFIDENCIAL | 3 | GDPR  PCI DSS | - Bloquear o compartilhamento público  - Bloquear o compartilhamento com os times |
| RESTRITO | 4 (mais sensível) | HIPAA  CREDENCIAIS | - Bloquear o compartilhamento público  - Bloquear o compartilhamento com os times  - Bloquear o compartilhamento com a organização |

*Tabela 1: exemplo de configuração apenas para fins explicativos.*

## Atualização manual da classificação do board para substituir a classificação automática

Somente os titulares, cotitulares ou editores do board podem atualizar a classificação para substituir o nível de classificação automática. Se a pessoa titular, cotitulares ou editores atualizarem a classificação do board para um nível de classificação menos sensível, eles deverão selecionar ou fornecer um motivo para essa alteração e essas informações serão adicionadas nos logs de auditoria.

### Atualização manual para um nível de classificação sensível inferior

**Cenário**
Considere um cenário em que João Silva é titular de um board que foi classificado automaticamente como **Confidencial**, cujo grau de sensibilidade é **3** na nossa configuração.

João verifica as informações e decide atualizar o nível da classificação para **Interno**, que tem o nível de sensibilidade **2**, sendo inferior ao atribuído pela classificação automática (**Confidencial**, nível **3**).

:::note
Somente os titulares, cotitulares ou editores de boards podem atualizar manualmente o nível de classificação.
:::

**Resultado**

Por ser titular do board, João pode atualizar sua classificação para um nível de sensibilidade inferior (**Interno**, nível **2**). Neste cenário, João é solicitado a explicar por que deseja alterar o nível de classificação do board para um nível menos sensível (Figura 1). João pode selecionar o motivo e clicar em **Atualizar**.

O nível de classificação do board é atualizado e as informações sobre esta atualização são adicionadas aos logs de auditoria.

### Atualização manual para um nível de classificação sensível superior

**Cenário**

Considere um cenário em que João Silva é titular de um board que foi classificado automaticamente como **Confidencial**, cujo grau de sensibilidade é **3** na nossa configuração.

João verifica as informações e decide atualizar o nível de classificação para **Restrito**, que tem o nível de sensibilidade **4** (mais alto), sendo superior ao atribuído pela classificação automática do board (**Confidencial**, nível **3**).

:::note
Somente os titulares, cotitulares ou editores de boards podem atualizar manualmente o nível de classificação.
:::

**Resultado**

Por ser titular do board, João pode atualizar sua classificação para um nível de sensibilidade superior.

A tabela a seguir resume vários cenários e seus resultados, considerando que o board já tinha sido classificado automaticamente em algum momento, mas um titular, cotitular ou editor do board resolve atualizar manualmente a classificação.

|  |  |  |
| --- | --- | --- |
| **Nível de classificação automática** | **Ação do titular do board** | **Novo nível de classificação** |
| CONFIDENCIAL | **Atualização para um nível de classificação inferior**  João, titular do board, atualiza manualmente a classificação do board para:  **INTERNO**, que tem o nível de sensibilidade 2, ou seja, inferior ao atribuído pela classificação automática (CONFIDENCIAL, nível 3). | Como João é titular do board, ele pode atualizar sua classificação para um nível de sensibilidade inferior: **INTERNO**.  Neste cenário, o titular do board é solicitado a explicar por que deseja alterar o nível de classificação do board para um nível menos sensível. João pode selecionar o motivo e clicar em **Atualizar**.  O nível de classificação do board é atualizado para **Interno** e as informações sobre esta atualização são adicionadas aos logs de auditoria. |
| CONFIDENCIAL | **Atualização para um nível de classificação superior**  João, titular do board, decide atualizar a classificação do board para **RESTRITO**, que tem o nível de sensibilidade mais alto (4), cujo nível é superior ao atribuído pela classificação automática (CONFIDENCIAL, nível 3). | Por ser titular do board, João pode atualizar sua classificação para um nível de sensibilidade superior. |

*Tabela 2: cenários e resultados dos níveis de classificação automática*

## Atualização automática da classificação do board

O ciclo de descoberta de dados é executado de hora em hora. Se o conteúdo do board for alterado, por adição ou remoção de dados altamente confidenciais, os boards com essas atualizações serão reclassificados automaticamente, com base no conteúdo atualizado e no nível de classificação não automática mais recente. As seções a seguir fornecem exemplos de cenários para atualizações automáticas do nível de classificação.

### Dados altamente confidenciais removidos do board

Após a conclusão do próximo ciclo de descoberta de dados, a classificação do board é atualizada automaticamente para o nível de sensibilidade aplicável.

**Exemplo do conteúdo do board neste cenário**

O board contém dados altamente confidenciais com informações relativas às seguintes etiquetas de sensibilidade: CREDENCIAIS, HIPAA, GDPR, PCI DSS. Portanto, após a conclusão do ciclo de descoberta de dados, a classificação automática classificou este board como **RESTRITO**, nível 4, cujo grau de sensibilidade é o mais alto com base no nosso exemplo de configuração de classificação automática. A tabela a seguir descreve as seguintes informações:

- **Última classificação não automática:** é a classificação não automática mais recente do board. Isso poderia ter sido feito [manualmente](03-auto-classification-overview-and-scenarios.md) através de uma [classificação padrão](../data-security/02-data-classification.md) ou pelas APIs [de atualização](https://developers.miro.com/reference/enterprise-dataclassification-board-set)/[atualização em massa de classificação do board](https://developers.miro.com/reference/enterprise-dataclassification-team-boards-bulk).

- **Classificação automática:** o nível de classificação automática aplicado ao board após a conclusão do ciclo de descoberta de dados.

- **Ação realizada:** a ação realizada e as atualizações feitas no conteúdo do board após a classificação automática.

- **Nova classificação:** a nova classificação considerando a ação realizada e todos os outros aspectos, como o conteúdo do board e a última classificação não automática.

|  |  |  |  |
| --- | --- | --- | --- |
| **Última classificação não automática** | **Classificação automática** | **Ação do usuário** | **Novo nível de classificação automática** |
| INTERNO (pela classificação padrão do board) | RESTRITO | Todos os dados confidenciais removidos do board | Após a conclusão do próximo ciclo de descoberta de dados, a classificação do board é atualizada automaticamente para o nível **INTERNO**, já que o board não contém mais informações confidenciais. Entretanto, a classificação não automática anterior era de nível INTERNO, que foi atribuída pela classificação padrão do board. |
| CONFIDENCIAL | RESTRITO | Todos os dados confidenciais são removidos do board | Após a conclusão do próximo ciclo de descoberta de dados, a classificação do board é atualizada automaticamente para o nível **CONFIDENCIAL**, grau de sensibilidade 3, mesmo que o board não contenha mais informações confidenciais, porque o nível de classificação não automática anterior era CONFIDENCIAL, nível 3. |
| NÃO CLASSIFICADO | RESTRITO | Os conteúdos de CREDENCIAIS e HIPAA, que são de nível RESTRITO e grau de sensibilidade 4, são removidos do board. | Após a conclusão do próximo ciclo de descoberta de dados, a classificação do board é atualizada automaticamente para **CONFIDENCIAL** (nível de sensibilidade 3), porque: - O board não contém mais as informações de CREDENCIAIS E HIPAA, mas ainda contém dados confidenciais de PCI DSS, que correspondem ao nível **CONFIDENCIAL**. - O board não foi classificado antes da classificação automática. |
| RESTRITO | RESTRITO | Os conteúdos de CREDENCIAIS e HIPAA, que são de nível RESTRITO e grau de sensibilidade 4, são removidos do board. | Após a conclusão do próximo ciclo de descoberta de dados, o board permanece no nível **RESTRITO** (grau de sensibilidade 4), mesmo que o board não contenha mais informações de CREDENCIAIS e HIPAA, porque o nível de classificação não automática anterior era RESTRITO (nível 4). |
| NÃO CLASSIFICADO | RESTRITO | Todos os dados confidenciais são removidos do board | Após a conclusão do próximo ciclo de descoberta de dados, a classificação do board é atualizada automaticamente para o nível **NÃO CLASSIFICADO**, já que o board não contém mais informações confidenciais e não foi classificado antes da classificação automática. |

*Tabela 3: cenários e resultados dos níveis de classificação automática*

### Dados altamente confidenciais adicionados ao board

Após a conclusão do próximo ciclo de descoberta de dados, a classificação do board é atualizada automaticamente para o nível de sensibilidade aplicável, com base no nível mais alto de dados confidenciais encontrados.

|  |  |  |
| --- | --- | --- |
| **Nível de classificação automática mais recente** | **Ação do usuário** | **Novo nível de classificação automática** |
| PÚBLICO | Um colaborador adicionou o número de cartão de crédito. | **CONFIDENCIAL** PCI DSS |
| INTERNO | Um colaborador adicionou o token de autenticação. | **RESTRITO** Credenciais |
| RESTRITO | Um colaborador adicionou o token de autenticação. | **RESTRITO** Permanece igual. |
| INTERNO | Um colaborador adicionou o número da carteira de motorista da Alemanha. | **CONFIDENCIAL**  GDPR |
| CONFIDENCIAL | Um colaborador adicionou o endereço MAC. | **RESTRITO**  Credenciais |

*Tabela 4: cenários e resultados dos níveis de classificação automática*
