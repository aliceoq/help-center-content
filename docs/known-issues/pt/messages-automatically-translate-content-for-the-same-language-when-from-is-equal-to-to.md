---
title: 'As mensagens traduzem automaticamente o conteúdo para o mesmo idioma (quando "de" é igual a "para")'
id: 7OIKmmhO3Pa2z0pIU33kY
status: PUBLISHED
createdAt: 2023-07-20T15:28:57.078Z
updatedAt: 2023-07-20T15:28:57.934Z
publishedAt: 2023-07-20T15:28:57.934Z
firstPublishedAt: 2023-07-20T15:28:57.934Z
contentType: knownIssue
productTeam: Store Framework
author: 2mXZkbi0oi061KicTExNjo
tag: Store Framework
slug: as-mensagens-traduzem-automaticamente-o-conteudo-para-o-mesmo-idioma-quando-de-e-igual-a-para
locale: pt
kiStatus: Backlog
internalReference: 865918
---

## Sumário

<div class="alert alert-info">
  <p>Este problema conhecido foi traduzido automaticamente do inglês.</p>
</div>


O aplicativo Mensagens traduz automaticamente o conteúdo quando o idioma "de" é igual a "para".

Ao implementar lojas multilíngues e o conteúdo tiver uma palavra em idioma estrangeiro, por exemplo, se o nome de um produto for traduzido do inglês para o espanhol, mas ainda tiver palavras em inglês, será exibida uma tradução indesejada.

## Simulação



- Traduza qualquer conteúdo da loja para qualquer outro idioma diferente do padrão;
- Certifique-se de que ainda haja pelo menos uma palavra em um idioma diferente do traduzido;
- Verifique a vitrine da loja; ela não corresponderá à tradução

## Workaround



- Desative a tradução automática;
- Traduza o conteúdo em que o idioma "de" é igual a "para", por exemplo, de "es-ES" para "es-ES".



