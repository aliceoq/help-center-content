---
title: 'Eventos disponíveis no Audit'
id: 6r1Mzcu5NmkmmDLJlz9CCZ
status: PUBLISHED
createdAt: 2022-06-22T16:05:16.214Z
updatedAt: 2024-01-18T20:46:19.490Z
publishedAt: 2024-01-18T20:46:19.490Z
firstPublishedAt: 2022-06-22T16:28:52.801Z
contentType: tutorial
productTeam: Master Data
author: 2Gy429C47ie3tL9XUEjeFL
slug: eventos-disponiveis-no-audit
locale: pt
legacySlug: eventos-disponiveis-no-audit
subcategory: 2TNXiKzLZOPxjMTyGiEeJu
---

Confira a seguir a lista dos possíveis eventos disponíveis no [Audit](https://help.vtex.com/pt/tutorial/searching-for-events-on-audit--5RXf9WJ5YLFBcS8q8KcxTA) por aplicação.

* [OMS](#oms)
* [Pedidos](#pedidos)
* [Estoque e entrega](#estoque-e-entrega)
* [Catálogo (Admin)](#catalogo-admin)
* [Catálogo (API)](#catalogo-api)
* [Preços](#precos)
* [Promoções](#promocoes)
* [Carteiras](#carteiras)
* [Checkout](#checkout)
* [Portal CMS](#portal-cms)
* [License Manager](#license-manager)
* [VTEX ID](#vtex-id)
* [Headless CMS](#headless-cms)

<div class = "alert alert-info">
  Caso você visualize no Audit algum evento que não esteja listado aqui, por favor nos informe usando a <a href="https://docs.google.com/forms/d/e/1FAIpQLSfmnotPvPjw-SjiE7lt2Nt3RQgNUe10ixXZmuO2v9enOJReoQ/viewform">página de feedback de documentação</a>.
  </div>

<div class="alert alert-warning">
  <p>Nas opções de filtros do Audit, você pode encontrar <strong>Opções de envio</strong>, <strong>Profile System</strong> e <strong>Billing</strong> além das aplicações citadas abaixo. Essas opções se referem a recursos internos ou funcionalidades em fase beta fechada, portanto, a maior parte das contas não terão eventos associados.</p>
</div>

## OMS

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Ação</strong>
    </td>
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Descrição do evento</strong>
    </td>
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Detalhes do evento</strong>
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Start Handling
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Ação que sinaliza para a VTEX que a loja iniciou o manuseio de um
      dado pedido. Isso desencadeia a continuidade do fluxo deste pedido.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID do pedido.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Change Status
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Mudança de status de um pedido.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID do pedido.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Shipping Notification
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Notificação de envio para um dado pedido.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID do pedido.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Payment Notification
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Envio de notificação de pagamento para um dado pedido.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID do pedido.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Save Configuration
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Alteração de configuração do módulo de Pedidos.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Descrição curta da alteração.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Resend Last Email
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Reenvio do último email relacionado àquele pedido no Message Center.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID do pedido.
    </td>
  </tr>
</table>

## Pedidos

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Action</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event description</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event details</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Change State
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Mudança de status do pedido.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do pedido.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Order Cancellation
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Cancelamento de pedido.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do pedido.
   </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Start Handling
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Ação que sinaliza para a VTEX que a loja iniciou o manuseio de um dado pedido. Isso desencadeia a continuidade do fluxo deste pedido.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID do pedido.
    </td>
   </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Notify Payment
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Envio de notificação de pagamento para um dado pedido.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do pedido.
   </td>
  </tr>
</table>

## Estoque e entrega

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Ação</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Descrição do evento</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Detalhes do evento</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Carrier Create
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Criação de transportadora.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID da transportadora.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Carrier Update
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Atualização de transportadora.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID da transportadora.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Carrier Delete
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Exclusão de transportadora.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID da transportadora.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Dock Create
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Criação de doca.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID da doca.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Dock Update
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Atualização de doca.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID da doca.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Dock Delete
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Exclusão de doca.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID da doca.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Warehouse Create
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Criação de estoque.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do estoque.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Warehouse Update
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Atualização de estoque.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do estoque.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Warehouse Delete
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Exclusão de estoque.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do estoque.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Pickup Point Save
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Criação ou alteração de ponto de retirada.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do ponto de retirada.
   </td>
  </tr>
</table>

## Catálogo (Admin)

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Ação</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Descrição do evento</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Detalhes do evento</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Product Activation
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Ativação de produto.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do produto.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Product Commercial Condition Change
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Mudanças em condições comerciais de um produto.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do produto e lista de condições alteradas.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">SKU Attachment Association    
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Associação de anexo a SKU.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do SKU, nome e ID do anexo.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Archive Upload    
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Envio de arquivo.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Nome do arquivo.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Field Activation    
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Ativação de campo de catálogo.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Nome, ID e status do campo.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">SKU Seller Binding    
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Ligação de um SKU a um seller.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do seller, ID do SKU no catálogo do seller e ID do SKU no catálogo do marketplace.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">SKU Seller Unbinding
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Remoção de ligação de um SKU a um seller.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do seller, ID do SKU no catálogo do seller e ID do SKU no catálogo do marketplace.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">SKU Seller Removal
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Remoção de SKU de seller.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do SKU no catálogo do seller.
   </td>
  </tr>
</table>

## Catálogo (API)

| Ação | Descrição | Detalhes do evento |
|---|---|---|
| SKU Seller Binding Removal | Remoção de vínculo de SKU. | ID do SKU no seller e ID do seller. |
| Seller Update | Atualização de seller. | ID do seller. |
| Seller Creation | Criação de seller. | ID do seller. |
| SKU Seller Binding Activation | Ativação de vínculo de SKU. | ID do SKU no seller e ID do seller. |
| SKU Seller Binding Inactivation | Inativação de vínculo de SKU. | ID do SKU no seller e ID do seller. |

## Preços

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Ação</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Descrição</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Detalhes do evento</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Put Price
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Criação ou alteração de preço para um dado SKU.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do SKU.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Save Price Table
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Criação ou alteração de tabela de preços.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Identificação da tabela criada ou alterada.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Save Price Tables
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Criação ou alteração de múltiplas tabelas de preços.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Identificação das tabelas criadas ou alteradas.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Price Deleted
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Exclusão de preço para um dado SKU.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do SKU.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Save Config
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Criação ou alteração de configuração de preço.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Identificação da configuração criada  ou alterada.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Fixed Price Modified
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Alteração de preço fixo.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Identificação do preço fixo alterado.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Put Catalog Step
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Criação ou alteração de uma regra de preço
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Regra de preço criada ou alterada.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Deleted Fixed Prices From Table
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Exclusão de preço fixo da respectiva tabela de preços.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Identificação da tabela e do preço excluído.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Compatibility Post Prices
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Alteração de preço utilizando a API de compatibilidade com o contrato do PricingV1
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Identificação do preço alterado.
   </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Change Rnb Config
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Alteração de configuração de preços em novas contas.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Nome da conta que fez a alteração.
    </td>
   </tr>
</table>

## Promoções

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Ação</strong>
    </td>
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Descrição do evento</strong>
    </td>
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Detalhes do evento</strong>
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Archive Coupon
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Arquivamento de cupom.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Código do cupom.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Unarchive Coupon
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Desarquivamento de cupom.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Código do cupom.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Change Rate Configuration
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Alteração de configuração de taxa.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID da configuração da taxa.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Change Promotion Configuration
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Alteração de configuração de promoção.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID da configuração da promoção.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Change Coupon Configuration
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Alteração em coupom.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Código do cupom.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Unarchived Calculator
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Desarquivamento de promoção ou taxa.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID da configuração da promoção ou taxa.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Archived Calculator
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Arquivamento de promoção ou taxa.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID da configuração da promoção ou taxa.
    </td>
  </tr>
</table>

## Carteiras

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Ação</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Descrição do evento</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Detalhes do evento</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">TOGGLE_WALLET
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Ativar ou desativar uma carteira digital.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">toggle-wallet-action
   </td>
  </tr>
</table>

## Checkout

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Ação</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Descrição do evento</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Detalhes do evento</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">SaveOrderFormConfiguration
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Alteração de configurações do OrderForm, objeto que rege o funcionamento do checkout da loja.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Descrição da ação (”configurated OrderForm”)
   </td>
  </tr>
</table>

## Portal CMS

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Ação</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Descrição do evento</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Detalhes do evento</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">File Update
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Alteração de arquivo do portal.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Nome e ID do arquivo alterado.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">File Upload
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Upload de arquivo do portal.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Nome do arquivo alterado.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">File Deleted
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Exclusão de arquivo.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Nome e ID do arquivo alterado.
   </td>
  </tr>
</table>

## License Manager

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Ação</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Descrição do evento</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Detalhes do evento</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Block AppToken
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Bloqueio de chave de aplicação.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Chave de aplicação bloqueada.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Accept Sponsor Invite
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Aceite de convite para se tornar usuário titular.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do usuário que aceitou o convite.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Save User
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Criação de usuário ou alteração de informações de usuário.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do usuário.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Save Account
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Criação de conta ou edição de informações de conta.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Conta criada ou alterada.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Change Role
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Edição de perfil de acesso.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Perfil de acesso editado.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Delete Role
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Exclusão perfil de acesso.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Perfil de acesso excluído.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Unblock AppToken
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Desbloqueio de chave de aplicação.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Chave de aplicação desbloqueada.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Resource Access Allowed
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Acesso a recurso permitido.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Chave do recurso e ID do usuário ao qual foi permitido.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Cancel Sponsor Invite
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Cancelamento de convite para usuário titular.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do usuário convidado.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Delete User
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Exclusão de usuário.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do usuário excluído.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Update Binding
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Atualização de binding.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Binding atualizado.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Resource Access Denied
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Acesso a recurso negado.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Chave do recurso e ID do usuário ao qual foi negado.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Create New AppToken
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Criação de chave de aplicação.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Chave de aplicação criada.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Create Sponsor Invite
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Criação de convite para usuário titular.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do usuário convidado.
   </td>
  </tr>
</table>

## VTEX ID

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Ação</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Descrição do evento</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Detalhes do evento</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">PasswordCreated
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Usuário registra uma senha pela primeira vez na loja ou no Admin VTEX.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do usuário.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">PasswordUpdated
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Usuário altera sua senha da loja ou do Admin VTEX.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do usuário.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">IdentityProviderChanged
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Mudança de configurações de provedor de identidade. Por exemplo: criação de integração OAuth customizada, alteração de informações em configuração de OAuth existente, entre outros.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Provedor de identidade.
   </td>
  </tr>
</table>

## Master Data

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Ação</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Descrição do evento</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Detalhes do evento</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">DeleteDocument
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Exclusão de documento.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID do documento.
   </td>
  </tr>
</table>

## Headless CMS

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Ação</strong>
    </td>
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Descrição</strong>
    </td>
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Detalhes do evento</strong>
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">TRY_PUBLISHING
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Tentativa de publicar uma página.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID do evento.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">TRY_PUBLISH_IN_RELEASE
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Tentativa de publicar um lançamento.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID do evento.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">TRY_UNPUBLISHING
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Tentativa de publicar uma página.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID do evento.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">RESTORE_CONTENT
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Restauração de conteúdo.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID do evento.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">TRY_UPDATING_DRAFT
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Tentativa de atualizar um rascunho.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID do evento.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">TRY_UNPUBLISHING_AND_OVERWRITING
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Tentativa de despublicar e sobrescrever uma página.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID do evento.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">done.invoke.deleteContent</td>
    <td class="t-body pa5" style="min-width: 15rem;">Exclusão de conteúdo.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID do evento.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">done.invoke.deleteContentVariant
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Exclusão de uma versão do conteúdo.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">ID do evento.
    </td>
  </tr>
</table>

Na coluna **Ação**, todos os eventos do Headless CMS também apresentam as seguintes informações:

* **CONTENT_ID:** código identificador único do conteúdo.
* **VARIANT_ID:** código identificador único da versão do conteúdo.
* **WORKSPACE:** workspace em que a alteração foi realizada.

