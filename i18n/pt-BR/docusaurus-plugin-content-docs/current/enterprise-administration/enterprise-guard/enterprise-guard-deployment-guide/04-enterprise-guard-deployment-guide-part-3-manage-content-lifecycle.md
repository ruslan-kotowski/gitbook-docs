---
title: 'Guia de implantação do Enterprise Guard Parte 3: Gerenciar o ciclo de vida
  do conteúdo'
article_id: 17121851926546
translation_id: 17121851926546
locale: pt-br
sidebar_position: 3
created_at: '2024-02-19T10:01:34Z'
updated_at: '2025-11-25T15:41:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
availability:
  notes: 'times relevantes: ** Exemplos de times com as quais você pode precisar fazer
    parceria para implantar recursos do Ciclo de Vida do Conteúdo incluem GRC (governança,
    risco, conformidade), Gerenciamento de Conformidade, Jurídico e/ou Gerenciamento
    de Registros.'
---

## Visão geral do gerenciamento do ciclo de vida do conteúdo

Na maioria das empresas, o conteúdo está crescendo exponencialmente em volume e complexidade. A gestão e governança adequadas dos boards da Miro são essenciais por vários motivos, incluindo:

- Aderir proativamente aos regulamentos específicos do setor ou às diretrizes internas da organização
- Minimizar riscos em cenários como disputas legais ou violações de segurança
- Manter a eficiência organizacional

Atualmente, oferecemos suporte aos seguintes recursos:

- [Políticas de lixeira](https://help.miro.com/hc/articles/13860817985426-Trash-Policy)
- [Políticas de retenção](https://help.miro.com/hc/articles/16855776325778-Retention-policies)

## Visão geral da implantação do gerenciamento do ciclo de vida do conteúdo

Embora o processo recomendado de [Parte 2: Implantar Segurança de Dados](03-enterprise-guard-deployment-guide-part-2-deploy-data-security.md)inclui configuração progressiva e comunicação com o usuário final, o Content Lifecycle Management não.

Nem as políticas de lixeira nem as políticas de retenção provavelmente interromperão a atividade do usuário final no Miro e, portanto, podem ser configuradas imediatamente.

## Implementar uma política de retenção global

Atualmente, apenas uma política de retenção global é suportada pelo Enterprise Guard. Opções de configuração adicionais estarão disponíveis e oferecerão maior flexibilidade no futuro. Considere os requisitos regulatórios do seu setor e as políticas organizacionais para determinar qual deve ser a duração da sua política de retenção global.

Como indisponível, pode ser benéfico configurar sua política de retenção global para corresponder ao requisito mais longo esperado pela sua organização. Por exemplo, se determinado conteúdo no Miro precisar ser retido por 5 anos devido a um requisito regulatório, sua política de retenção global deverá ser definida para 5 anos.

Você pode reduzir o escopo dos boards mantidos sob esta política de retenção de 5 anos posteriormente, quando o Miro liberar escopos de retenção mais granulares, como nível de classificação ou time.

[Como configurar políticas de retenção](https://help.miro.com/hc/articles/16855776325778-Retention-policies)

## Configurar a política de lixeira

Por padrão, os boards da Miro são excluídos da lixeira de forma automática e permanente após 90 dias. Você pode atualizar a configuração padrão e optar por excluir automaticamente e permanentemente os boards da lixeira em 30, 60, 90 ou 180 dias.

Quando o período de exclusão automática e permanente do board é atualizado, o novo prazo é aplicado apenas aos boards que foram recém-movidos para a lixeira. Os boards devem ser movidos manualmente para a lixeira pelos titulares ou cotitulares dos board .

Quando um board está na lixeira , mas a política de lixeira não terminou, alguns usuários podem excluir os boards manualmente e permanentemente. Escolha quem pode fazer isso nas configurações da lixeira entre titulares do board ou admins.

[Como configurar políticas de lixeira](https://help.miro.com/hc/articles/13860817985426-Trash-settings)

## retenção e lixeira trabalhando juntos

As políticas de retenção substituem as políticas de lixeira e a exclusão manual e permanente. Veja os exemplos e o diagrama abaixo.

Exemplos:

- Se um board for movido para a lixeira e excluído manualmente e permanentemente pelo titular do board , mas o board estiver sob uma política de retenção , o board será retido. No final do período de retenção , o board será imediatamente e permanentemente excluído.
- Se um board for movido para a lixeira e o período de exclusão permanente terminar, mas o board estiver sob uma política de retenção , o board será retido. No final do período de retenção , o board será imediatamente e permanentemente excluído.

![Enterprise-Guard-Trash-Policies.png](images/21017013750034_Enterprise-Guard-Trash-Policies.png)
*retenção e lixo trabalhando juntos*
