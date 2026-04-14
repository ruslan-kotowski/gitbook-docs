---
title: "Vis\xE3o geral do gerenciamento de chaves de criptografia"
article_id: 14634334255250
translation_id: 14634334255250
locale: pt-br
sidebar_position: 0
created_at: '2023-10-24T14:24:53Z'
updated_at: '2026-02-05T15:17:37Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: enterprise-key-management
---

O complemento Enterprise Guard inclui uma opção para o Gerenciamento de Chaves de Criptografia (EKM). O EKM proporciona controle centralizado sobre as chaves de criptografia para ajudar a proteger seus dados. Esta solução baseada em nuvem permite o monitoramento de logs de atividades associados às chaves de criptografia e autoriza a revogação de acesso às chaves de seus dados.

Para controle e visibilidade adicionais sobre como as chaves de criptografia são utilizadas no Miro, você também pode usar o Bring Your Own Key (BYOK). Com o BYOK, você gerencia a criptografia dos dados da sua organização na plataforma da Miro.

## Conheça as vantagens do EKM

- **Implementação sem complicações:** Integre facilmente o EKM ao seu sistema, sem a necessidade de instalação ou manutenção de hardware, graças a uma solução 100% baseada em nuvem.

- **Controle total de acesso às chaves:** Desfrute de autoridade completa sobre suas chaves de criptografia. Você tem a capacidade de revogar sua chave, tornando todos os dados criptografados inacessíveis tanto para a Miro quanto para os usuários finais.

- **Visibilidade aprimorada de acesso:** Obtenha insights sobre as atividades relacionadas às chaves com visibilidade de acesso. Monitore e rastreie logs por meio do AWS CloudTrail para uma compreensão completa do uso da sua chave de criptografia.

![Enterprise Key Management Diagram](images/21016121496338_EKM.png)

## Como o EKM protege os dados dos clientes

A Miro disponibiliza o EKM oferecendo criptografia de seus dados de produção e dados de backup em repouso com chave de criptografia personalizada, enquanto o cliente concede à Miro acesso à chave de criptografia personalizada. A Miro oferece suporte ao EKM com uma chave hospedada em sua própria conta AWS via AWS KMS. Com o EKM, você ganha maior visibilidade de auditoria e maior controle de acesso aos dados (conteúdo gerado pelo usuário), como formas, widgets e arquivos carregados.

## Criptografia de dados na Miro

A segurança máxima dos seus dados é uma preocupação primordial para a Miro. Por padrão, empregamos medidas de criptografia para dados de clientes, tanto em trânsito quanto em repouso, independentemente do plano de assinatura. Ao acessar a Miro pela internet, seus dados contam com proteção por meio de criptografia TLS 1.3 e certificados PKI emitidos pela Amazon Web Services (AWS). Ao chegar aos nossos servidores, seus dados ficam ainda mais protegidos por meio da criptografia AES-256 em repouso, utilizando chaves gerenciadas pela Miro por meio do AWS Key Management Serviço (KMS). [Saiba mais sobre segurança na Miro.](https://miro.com/trust/security/)

> Observação: Você é o único responsável pela segurança e proteção de todos e quaisquer dados de backup baixados ou transferidos por você para seus sistemas ou sistemas de terceiros. Você é o único responsável por sua chave de criptografia personalizada. Se perder sua chave de criptografia personalizada, a Miro não poderá ajudar você a recuperar o acesso aos dados. Depois que seus Dados de produção ou Dados de backup estiverem em trânsito ou fora do controle da Miro, a Miro não poderá garantir a proteção dos mesmos.

## Como habilito o gerenciamento de chaves de criptografia?

A configuração e implantação do gerenciamento de chaves de criptografia requer a assistência de times internos da Miro. Se precisar de assistência, entre em contato com seu representante da Miro ou [solicite assistência à equipe de Suporte da Miro aqui](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).

## Glossário

- **Dados de backup:** Um instantâneo (snapshot) do seu conteúdo criado ou enviado ao serviço da Miro, armazenado pela Miro para recuperação e outros fins.

- **Chave de criptografia personalizada:**  Uma chave de segurança exclusiva, personalizada e implementada por você, necessária para que os indivíduos acessem seus Dados de produção e Dados de backup.

- **Dados de produção:** Todos os dados que você e seus usuários acessam durante o uso e a operação diária dos serviços da Miro.
