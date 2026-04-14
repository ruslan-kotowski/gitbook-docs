---
title: Impostos
article_id: 4408846055314
translation_id: 4408846055314
locale: pt-br
sidebar_position: 6
created_at: '2021-10-28T10:32:02Z'
updated_at: '2025-06-23T06:42:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
---

## Imposto sobre Vendas , imposto sobre valor agregado e imposto sobre bens e serviços

A Miro avalia os impostos aplicáveis ​​às taxas de assinatura , conforme exigido pela lei local. Dependendo da sua localização, você poderá ser cobrado por impostos ao adquirir um plano pago do Miro . Quando a Miro coleta esses impostos, o valor total é remetido às autoridades fiscais relevantes em seu nome.

- Imposto sobre Vendas , imposto sobre bens e serviços (GST) ou imposto sobre valor agregado (IVA) não estão incluídos nos preços exibidos em nossa página de preços
- O *endereço da empresa* fornecido na seção de informações de cobrança do seu perfil é usado para determinar a taxa de imposto correta, se aplicável
- Somente os admins do time no plano Starter , Admins da empresa no plano Business e [admins de cobrança](../../administration/admin-faq/01-admin-faq.md) podem atualizar informações como o país de cobrança e o número de identificação fiscal associados à sua assinatura.

## Imposto sobre Valor Acrescentado (IVA)

Se sua organização estiver localizada na União Europeia, Noruega, Turquia ou Reino Unido, o imposto sobre valor agregado (ou IVA) será adicionado às suas compras (por exemplo, assinaturas, licenças adicionais e renovações), e você verá o imposto como um item de linha separado em suas faturas.

### Isenção de IVA

Se você for uma empresa registrada, poderá estar isento de IVA (ou seja, poderá ser aplicada cobrança reversa) em suas compras futuras se um ID de IVA válido for inserido na página [Configurações de cobrança](../manage-your-subscription-and-plan/01-manage-your-subscription.md) .

Se o seu endereço de cobrança estiver na UE, observe que o número de identificação fiscal fornecido deve estar registrado no [banco de dados VIES](https://ec.europa.eu/taxation_customs/vies/) para ser considerado válido. Pode ser necessário solicitar à autoridade fiscal relevante que seu número de IVA seja incluído no banco de dados VIES em certos países da UE onde esse processo não é automático.

### Como inserir seu número de IVA no ponto de compra

Após selecionar o tamanho da sua time , ciclo de cobrança e método de pagamento:

1. Insira seu país na seção de informações de cobrança (um campo de ID de IVA será exibido).
2. Insira seu número de identificação fiscal (IVA).

### Como atualizar seu ID de IVA

1. Clique no avatar do seu perfil e depois em **Console de admin**.
2. Na barra lateral esquerda, clique em **Faturamento** e depois clique na guia **Informações de faturamento** .
3. Preencha o endereço da empresa e insira o número de identificação fiscal (certifique-se de incluir o código de país de duas letras associado ao seu número de identificação fiscal).

### Número de identificação fiscal do Miro

A Miro está registrada para IVA por meio do esquema One Stop Shop ('OSS') na UE e não possui registro de IVA em cada Estado-Membro da UE. O esquema OSS está disponível para sujeitos passivos não estabelecidos na UE para cobrar e remeter IVA sobre serviços fornecidos eletronicamente a clientes não comerciais em Estados-Membros da UE. Miro selecionou a Holanda como seu país de identificação para o OSS.

## Imposto sobre bens e serviços (GST)

Se sua organização estiver localizada na Austrália ou na Nova Zelândia, o imposto sobre bens e serviços ou GST será adicionado às suas compras (assinaturas, licenças adicionais e renovações) e você verá o imposto como um item de linha separado em suas faturas.

### Isenção de GST

Se você for uma empresa registrada e seu endereço comercial for na Austrália ou Nova Zelândia, você poderá estar isento do pagamento de GST em compras na Miro por meio do mecanismo de "Cobrança Reversa".

### Como inserir seu número de identificação fiscal

Se um Número Business Australiano (ABN) válido ou um número de GST da Nova Zelândia for inserido na finalização da compra ou na página de configurações de cobrança, o GST não será cobrado para compras atuais ou futuras.

Se nenhuma informação da empresa ou número de identificação fiscal for fornecida, o GST será cobrado em todas as compras.

#### **No checkout**

Depois de selecionar o tamanho da sua time , o ciclo de faturamento e os detalhes do método de pagamento, você terá a chance de adicionar os detalhes da sua empresa (opcionalmente):

1. Clique no botão **+ Adicionar informações da empresa** e preencha os campos exibidos. Você precisará selecionar "Austrália" ou "Nova Zelândia" como país.
   ![Impostos_faturamento_info_formatado.png](../../../../../../docs/plans-billing/billing-and-payments/images/21019603651218_Taxes_billing_info_formatted.png)
   *Campos de informações da empresa nas configurações de cobrança*
2. Preencha os detalhes do **nome** e **endereço** da empresa e adicione seu ABN ou GST ID (NZ) ao campo **Tax ID** .
   - Se você estiver na Austrália, precisará clicar na caixa de seleção se estiver registrado no GST para ter direito ao mecanismo de cobrança reversa.
   - Os clientes da Nova Zelândia não verão esta caixa de seleção.![impostos_informacoes_da_empresa_e_id_fiscal_formatado.png](../../../../../../docs/plans-billing/billing-and-payments/images/21019592631826_taxes_company_info_and_tax_id_formatted.png)
     *Informações da empresa com caixa de registro GST*
3. Agora, o Miro fará uma verificação automática com nosso provedor de impostos para garantir que o ID fiscal fornecido seja válido. Se válido, o valor do imposto mostrado no resumo de pagamento será reduzido a zero.
   - IDs inválidos ou quando uma caixa de seleção não for fornecida resultarão na cobrança de GST.![impostos_faturamento_pedido_resumo_formatado.png](../../../../../../docs/plans-billing/billing-and-payments/images/21019603655442_taxes_billing_order_summary_formatted.png)
     *Resumo do Pedido com impostos excluídos*

### Como atualizar seu ID fiscal

1. [Abra as](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md) Configurações do time. Você precisará ser um admin de cobrança.
2. Acesse a aba **Faturamento** **> Informações de faturamento**.
3. Preencha os campos Endereço da empresa e Número de identificação fiscal.
4. Selecione a caixa para declarar que sua empresa está registrada para GST (somente Austrália)
5. O Miro realizará uma verificação com nosso provedor de impostos automaticamente para garantir que o ID fiscal fornecido seja válido. Se válido, compras futuras não terão impostos aplicados.
   - IDs inválidos ou quando uma caixa de seleção não for fornecida resultarão na cobrança de GST.
   - O Miro não ajustará compras históricas se os IDs fiscais não tiverem sido fornecidos no momento da compra.![taxes_billing_VAT_ID_formatted.png](../../../../../../docs/plans-billing/billing-and-payments/images/21019592626450_taxes_billing_VAT_ID_formatted.png)*Declaração de registro de GST da empresa*

### ID do GST de Miro

A Miro está registrada no GST por meio do processo de registro simplificado como uma empresa não residente que fornece serviços eletronicamente. Por isso, a Miro tem um Número de Referência ATO (ARN) e só cobrará GST sobre suprimentos para clientes não comerciais.
