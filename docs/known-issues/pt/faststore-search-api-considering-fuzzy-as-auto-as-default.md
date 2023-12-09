---
title: 'A API de pesquisa da Faststore considera o fuzzy como automático por padrão'
id: 2zedXBMhlD8pu4gZMXsrSp
status: PUBLISHED
createdAt: 2023-08-28T23:35:04.009Z
updatedAt: 2023-08-28T23:35:04.608Z
publishedAt: 2023-08-28T23:35:04.608Z
firstPublishedAt: 2023-08-28T23:35:04.608Z
contentType: knownIssue
productTeam: FastStore
author: 2mXZkbi0oi061KicTExNjo
tag: FastStore
slug: a-api-de-pesquisa-da-faststore-considera-o-fuzzy-como-automatico-por-padrao
locale: pt
kiStatus: Backlog
internalReference: 889321
---

## Sumário

<div class="alert alert-info">
  <p>Este problema conhecido foi traduzido automaticamente do inglês.</p>
</div>


No pacote @fatstore/api, para o resolvedor da Pesquisa Inteligente, estamos considerando o fuzzy como automático por padrão quando deveria ser 0. Isso está fazendo com que o comportamento do fuzzy seja aplicado, causando uma "falsa correspondência incorreta" nos resultados da pesquisa quando realmente temos uma correspondência exata com o termo pesquisado, mas exibimos mais resultados independentemente disso

## Simulação



## Workaround



