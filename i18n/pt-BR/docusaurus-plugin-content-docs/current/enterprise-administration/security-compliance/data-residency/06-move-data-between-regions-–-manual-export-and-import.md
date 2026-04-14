---
title: 'Mover dados entre regiões: exportação e importação manual'
article_id: 24778387087122
translation_id: 24778387087122
locale: pt-br
sidebar_position: 6
created_at: '2025-02-20T09:07:00Z'
updated_at: '2025-11-25T15:49:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Quem pode fazer isso: Titulares e cotitulares de boards, admins de conteúdo,
    Admins da empresa Quais planos: Enterprise Quais plataformas: navegador, desktop'
---

Este artigo descreve o método de exportação e importação manual para mover dados entre as regiões. Para saber mais sobre as opções de transferência de dados entre regiões, inclusive a migração automática, confira [Mover dados entre regiões](../../canvas-25-admin-features/data-residency/03-move-data-between-regions.md).

## Preparar para exportação e importação manual para uma nova região

Se você é Admin da empresa, siga estas práticas recomendadas ao preparar a migração manual para uma nova região:

- Para iniciar uma nova organização na sua região escolhida, fale com seu contato da Miro.
- Verifique todos os domínios que você possui com a verificação de DNS para garantir o gerenciamento de todos os usuários do seu domínio.
- Habilite a política de controle de domínio **Bloquear assinaturas próprias**, para evitar que os usuários criem, sem querer, assinaturas Free da Miro na sua região antiga.
- Consolide times e/ou organizações em uma única organização com uma única assinatura.
- Identifique quais integrações sua organização usa e precisará na nova região, e monte um cronograma para reconfigurar cada uma delas.
- Cheque todas as configurações usadas hoje pela sua organização e defina um cronograma para reconfigurar as que forem necessárias na sua nova região.

## Exportação e importação manual de dados para uma nova região

A Miro provisiona uma nova organização Enterprise na região de destino. Os usuários devem exportar seus boards como backups da região de origem e depois importar seus backups para a região de destino.

**Mais informações:** Confira [Como salvar o backup do board](../../../using-miro/import-and-export/export/05-how-to-save-board-backup.md).

Somente os usuários com as permissões abaixo podem exportar e importar conteúdo manualmente:

- Titular do board
- Cotitulares do board
- Admin da empresa
- Admin de conteúdo

:::note
Todo o compartilhamento de boards foi perdido. Depois de carregar o backup na região de destino, os usuários devem restaurar suas permissões de compartilhamento.
:::

Para iniciar a importação manual de conteúdo, os usuários podem fazer login no seu novo URL regional, que pode ser uma das seguintes opções:

- (Austrália) [au.miro.com](https://au.miro.com/)
- (Estados Unidos) [us.miro.com](https://us.miro.com/)

:::note
Antes de fazer login pela primeira vez como usuário, verifique se sua organização usa o Logon único. Se você usa o logon único, aguarde seu Admin da empresa reconfigurar as definições de SSO para sua nova região.
:::

## O que fazer após uma exportação e importação manual

Após uma migração de dados entre regiões, faça o seguinte:

- Se for o caso, reconfigure imediatamente o logon único para os novos subdomínios regionais. Por exemplo, au.miro.com.
  > ✏️ Para que seus usuários consigam fazer login na nova região, é necessário reconfigurar o logon único no IDP.
- Reconfigure o SCIM para os novos subdomínios regionais. Por exemplo, au.miro.com.
- Confira se a opção **Bloquear assinaturas próprias** está habilitada nas configurações de controle de domínio.
- Valide as demais configurações da organização, controle de domínio e times.
- Reinstale e configure cada aplicativo e integração Enterprise, como SIEM, SAM, eDiscovery, Smarsh e Okta.
- Convide usuários para a organização na nova região.

## Perguntas frequentes sobre a exportação e importação manual de dados para uma nova região

**Como funciona a migração manual para uma nova região?**

Os admins devem reconfigurar a organização e todos os times, configurações de times e usuários. Os usuários finais devem baixar manualmente os backups dos boards da organização antiga e carregá-los na nova organização.

**Quem é elegível e quem não é?**

Os clientes Enterprise podem migrar seus dados para outra região. Para mais informações, fale com seu contato da Miro.

**Quais dados estão incluídos em uma migração manual?**

Somente os boards movidos por usuários. Para mais informações, confira Exportação e importação manual de dados para uma nova região.

**Preciso pagar algo a mais por isso?**

Não. A Miro pode provisionar uma nova organização na Austrália ou nos Estados Unidos através do contrato padrão do plano Enterprise.

**Quanto tempo leva para concluir uma migração manual?**

A duração de uma migração manual depende do tempo que os usuários levam para exportar seus boards salvos como backup e importar esse conteúdo para a região de destino.

**De que forma a Miro garante que vai excluir os dados da minha organização da região de origem?**

Informe o Suporte da Miro após concluir a exportação e importação manual para a nova região, incluindo a reconfiguração, e quando todos os usuários tiverem importado seus backups para a região de destino. O Suporte da Miro excluirá sua organização e todos os dados da região de origem.
