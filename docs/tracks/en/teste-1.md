---
title: 'Teste (1)'
id: 2Oq3MriB8hJ5YmFq3QIlPD
status: DRAFT
createdAt: 2021-04-14T14:58:44.451Z
updatedAt: 2023-11-27T23:47:43.098Z
publishedAt: 
firstPublishedAt: 2021-04-14T15:01:28.601Z
contentType: trackArticle
productTeam: Channels
slug: teste-1
locale: en
trackId: 5Yx5IrNa7Y48c6aSC8wu2Y
trackSlugEN: magazine-luiza-integration-set-up
---

<div class="alert alert-info">
<p>Essa funcionalidade está em fase beta, o que significa que estamos trabalhando para aprimorá-la. Em caso de dúvidas, entre em contato com <a href= "https://support.vtex.com/hc/pt-br/requests">nosso Suporte</a>.</p>
</div>

A funcionalidade **Alterar pedido (beta)** permite que você mude um pedido de diversas maneiras, seja a mudança motivada pela vontade do cliente, pela indisponibilidade de produtos ou outros motivos. Os principais tipos de alteração de pedidos são: 

* **Adicionar:** uma quantidade de itens ou novos produtos.
* **Remover:** uma quantidade parcial ou total de itens.
* **Alterar peso:** os itens podem passar a ter um peso maior ou menor.
* **Substituir itens:** trocar itens por outros, incluindo itens precificados por peso.
* **Alterar preço:** mudar valor total do pedido.

Para ver o passo a passo completo de como realizar cada ação, veja a documentação [Como alterar pedidos (Beta)](link). O artigo atual aborda outros aspectos da **Alterar pedido (Beta)** e está organizado da seguinte forma:

* [Alterações pelo Admin VTEX e API](#alteracoes-pelo-admin-vtex-e-api)
* [Características gerais](#caracteristicas-gerais)
* [Mudanças de preço](#mudanças-de-preco)

## Alterações pelo Admin VTEX e API

Existem duas vias pelas quais um pedido pode ser alterado, veja os detalhes na tabela a seguir:

| **Como alterar** | **Descrição** | **Status que admite alteração** |
|:---:|:--- |:--- |
| Via Admin VTEX | <p>A alteração é feita pela <a href="https://help.vtex.com/pt/tutorial/pagina-de-detalhes-do-pedido--2Y75n54Cc9VizrlG1N6ZNl">página de detalhes do pedido</a>, que pode ser acessada em <b>Pedidos > Todos os pedidos</b>, selecionando o pedido desejado.</p><p>Também é possível acessar o pedido usando a barra de busca no topo do Admin VTEX. Para isso, clique sobre a barra, selecione a opção <b>Pedidos</b> e utilize algum dos seguintes critérios:</p><p><ul><li>ID do pedido</li><li>Nome do cliente</li><li>Email do cliente</li><li>Documento do cliente</li></ul></p><p><b>Artigo no Help Center:</b> <a href="https://help.vtex.com/pt/tutorial/--531cHtUCUi3puRXNDmKziw">Como alterar pedidos (Beta)</a></p> | <p><ul><li><code>preparando entrega</code></li></ul></p> |
| Via API | Altera pelos endpoints:<p><ul><li><a href="https://developers.vtex.com/docs/api-reference/orders-api#patch-/api/order-system/orders/-changeOrderId-/changes">Create order change</a></li><li><a href="https://developers.vtex.com/docs/api-reference/orders-api#post-/api/order-system/orders/-changeOrderId-/changes/preview">Preview order change</a></li><li><a href="https://developers.vtex.com/docs/api-reference/orders-api#get-/api/order-system/orders/-changeOrderId-/changes/-changeRequestId-">Get order change detail</a></li><li><a href="https://developers.vtex.com/docs/api-reference/orders-api#get-/api/order-system/orders/-changeOrderId-/changes">Get order change history</a></li><li><a href="https://developers.vtex.com/docs/api-reference/orders-api#post-/api/order-system/orders/-changeOrderId-/changes/-changeRequestId-/retry">Retry order change</a></li><li><a href="https://developers.vtex.com/docs/api-reference/orders-api#post-/api/order-system/orders/-changeOrderId-/changes/-changeRequestId-/cancel">Cancel order change</a></li></ul></p>| <p><ul><li><code>ready-for-handling</code></li><li><code>handling</code></li><li><code>waiting-for-fulfillment</code></li><li><code>ready for invoicing</code></li></ul></p> |

O histórico de alterações do pedido fica registrado na sua [página de detalhes](https://help.vtex.com/pt/tutorial/pagina-de-detalhes-do-pedido--2Y75n54Cc9VizrlG1N6ZNl), na seção **Histórico de itens alterados**. Para consultar essa informação por API, utilize o endpoint [Get order change history](https://developers.vtex.com/docs/api-reference/orders-api#get-/api/order-system/orders/-changeOrderId-/changes).
