---
title: Monitorar o status do gerenciamento de chaves de criptografia
article_id: 31325531757970
translation_id: 31325531757970
locale: pt-br
sidebar_position: 1
created_at: '2025-11-24T17:59:06Z'
updated_at: '2026-02-04T20:46:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: enterprise-key-management
---

Os admins podem monitorar e acompanhar o status da configuração do seu gerenciamento de chaves de criptografia (EKM) no console de admin da Miro. Isso traz maior transparência ao processo de integração de chaves e ao andamento da criptografia, ajudando-o a se manter informado sem precisar de suporte adicional.

## Verificar status do EKM

1. No console de admin da Miro, vá para **Enterprise Guard**.
2. Selecione **gerenciamento de chaves de criptografia**.
3. Na seção **Status**, revise o status atual e a mensagem.

## Entender status do EKM

A seção **Status** mostra onde você está no processo de configuração do EKM e de criptografia.

| Status | Significado |
| --- | --- |
| **Chaves personalizadas adicionadas** | A Miro está configurando a criptografia com suas chaves personalizadas. Assim que estiver pronto, suas chaves começarão automaticamente a criptografar o conteúdo. |
| **Ativação de chave em andamento** | Novos conteúdos são criptografados com suas chaves personalizadas. A recriptação de conteúdos existentes está em andamento. |
| **Chaves personalizadas ativas** | Todo o conteúdo está criptografado com suas chaves personalizadas. |
| **Retornando para chaves padrão** | A Miro está alterando sua criptografia de volta para as chaves padrão da Miro. Suas chaves personalizadas serão removidas. |

## Revisar chaves configuradas

Na seção de Chaves, você pode visualizar os identificadores das chaves atualmente configuradas para o gerenciamento de chaves de criptografia. Se a Miro gerencia suas chaves personalizadas, poderá ver uma notificação em vez de um ARN de chave.

- **Chave principal**

  Encripta os boards, comentários e outros conteúdos da sua organização.
- **Chave de armazenamento de backup**

  Encripta versões arquivadas e backups.
- **ARN de chave**

  O identificador da chave no [AWS KMS](https://aws.amazon.com/kms/). Se a Miro gerencia suas chaves personalizadas, poderá ver uma notificação em vez de um ARN de chave.

(Opcional) Para fazer alterações em suas chaves (por exemplo, se você vir a chave errada ou quiser voltar para a criptografia padrão), entre em contato com seu Gerente de Sucesso do Cliente ou [support@miro.com](mailto:support@miro.com).
