---
title: 'Pontos de coleta não indexados nos dados mestre'
id: 6OHjbM6GXBEvgepaod3AyT
status: PUBLISHED
createdAt: 2023-12-14T22:29:26.240Z
updatedAt: 2023-12-15T20:04:00.518Z
publishedAt: 2023-12-15T20:04:00.518Z
firstPublishedAt: 2023-12-14T22:29:26.972Z
contentType: knownIssue
productTeam: Storage
author: 2mXZkbi0oi061KicTExNjo
tag: Storage
slug: pontos-de-coleta-nao-indexados-nos-dados-mestre
locale: pt
kiStatus: Backlog
internalReference: 530824
---

## Sumário

<div class="alert alert-info">
  <p>Este problema conhecido foi traduzido automaticamente do inglês.</p>
</div>


Atualmente, o sistema de logística usa o MasterData para armazenar informações de pontos de coleta. Como resultado, podemos ter problemas para indexar essa entidade interna ao usar a rota de pesquisa. Isso pode levar a informações desatualizadas, como:

- Exclusão feita em Logística que não é refletida na lista;
- Ponto de coleta sendo ativado/inativado em Logística, mas ainda retornando com o status anterior;
- Alterações de coordenadas que não estão sendo refletidas;
- E outros.

## Simulação


Não há uma maneira confiável de reproduzir esse problema.



## Workaround


A equipe da VTEX deve verificar os dados e, eventualmente, reindexá-los, para que os dados sejam atualizados.




