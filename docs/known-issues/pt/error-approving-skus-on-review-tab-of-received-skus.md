---
title: 'Erro ao aprovar skus na guia Revisão de skus recebidos'
id: 7fRMTxq7CFRkyZeK08AGIg
status: PUBLISHED
createdAt: 2023-11-23T13:46:30.453Z
updatedAt: 2023-11-23T13:46:31.370Z
publishedAt: 2023-11-23T13:46:31.370Z
firstPublishedAt: 2023-11-23T13:46:31.370Z
contentType: knownIssue
productTeam: Marketplace
author: 2mXZkbi0oi061KicTExNjo
tag: Marketplace
slug: erro-ao-aprovar-skus-na-guia-revisao-de-skus-recebidos
locale: pt
kiStatus: Backlog
internalReference: 940998
---

## Sumário

<div class="alert alert-info">
  <p>Este problema conhecido foi traduzido automaticamente do inglês.</p>
</div>


Quando um sku é reprovado nas regras opcionais de Qualidade da Oferta criadas pelo Marketplace, ele vai diretamente para a "Guia Revisão" de Skus Recebidos.

No entanto, ao tentar aprovar o sku, uma mensagem de erro é retornada: "Sorry, something went wrong in the Catalog. Tente novamente ou entre em contato com a VTEX se o problema persistir."

Isso acontece porque o módulo Matcher não foi capaz de preencher as informações do produto e do sku depois de enviar o sku para a guia Review (você pode verificar isso usando as APIs):
 ![](https://vtexhelp.zendesk.com/attachments/token/0Dti3ak7twOpuVzvzntmPCGit/?name=image.png)

## Simulação



1. Crie uma regra opcional sobre a qualidade da oferta;
2. Aguarde até que um sku falhe na regra e vá para a guia Review (Revisão);
3. Tente aprovar o sku e receba uma mensagem de erro;
4. Verificar via API se o objeto de correspondência está preenchido como na imagem acima

## Workaround


Aprovar o sku via API passando manualmente as informações corretas do produto e do sku.





