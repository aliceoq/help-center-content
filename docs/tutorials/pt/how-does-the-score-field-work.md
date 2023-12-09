---
title: 'Como funciona o campo Score?'
id: 1BUZC0mBYEEIUgeQYAKcae
status: PUBLISHED
createdAt: 2018-02-16T16:17:51.610Z
updatedAt: 2023-07-14T11:54:54.135Z
publishedAt: 2023-07-14T11:54:54.135Z
firstPublishedAt: 2018-02-16T18:09:11.291Z
contentType: tutorial
productTeam: Marketing & Merchandising
author: 7FpKZ0rc6k4WqeymES80cw
slug: como-funciona-o-campo-score
locale: pt
legacySlug: como-funciona-o-campo-score
subcategory: 2g6LxtasS4iSeGEqeYUuGW
---

O campo __Score__, disponível nos cadastros de __Produto__, __Categoria__ e __Marca__, é o valor utilizado para garantir a ordenação de produtos na sua loja e, também, como critério de desempate para outras ordenações comuns, como menor preço, melhor desconto etc. Ao preencher esse campo, é possível definir a prioridade de alguns produtos em relação a outros, tanto na vitrine quanto na página de resultado de busca.

O critério para enumerar o campo segue uma ordenação numérica (1, 2, 3, 4…) para apresentar a sequência na vitrine da loja ou na página de resultado de busca. 

Por padrão, produtos sem um *score* cadastrado se comportam como se tivessem score igual a 0.

O *score* do produto é a soma do seu próprio *score* mais os de categoria e marca. Ou seja: `Score do produto + Score da Categoria + Score da Marca`.

Você pode utilizar os parâmetros abaixo para implementar a ordenação:

- __Ordem ascendente:__ `?O=OrderByScoreASC`
- __Ordem descendente:__ `?O=OrderByScoreDESC`

Recomendamos definir o Score a nível de produto, já que o mais comum é que sua vitrine esteja sempre em constante mudança.

Um exemplo para o uso do Score pode ser em eventos pontuais, quando sua loja precisa colocar produtos específicos na frente de outros para que a visualização seja garantida.

Para adicionar ou alterar um score relacionado a um produto, siga estes passos:

1. No Admin VTEX, acesse **Catálogo > Produtos e SKUs**.
2. Clique em `Adicionar Produto` para criar um novo produto ou clique em `Alterar` no produto que deseja editar.
3. Insira o valor desejado do score no campo **Score (usado para ordenação de busca)**.

![posicao-Score-PT](//images.ctfassets.net/alneenqid6w5/6SGu9GBtxou7sLg5rM59vl/f02f302fc3de0346b7ec9d794c413da3/Screenshot_6.png)
