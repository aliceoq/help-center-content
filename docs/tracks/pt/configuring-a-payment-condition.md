---
title: 'Configurar uma condição de pagamento'
id: 6bzGxlz4inf8sKmvZ1c7i3
status: PUBLISHED
createdAt: 2019-11-26T17:47:27.426Z
updatedAt: 2023-03-21T20:02:36.184Z
publishedAt: 2023-03-21T20:02:36.184Z
firstPublishedAt: 2019-11-26T20:43:48.321Z
contentType: trackArticle
productTeam: Financial
slug: configurar-uma-condicao-de-pagamento
locale: pt
trackId: 6GAS7ZzGAm7AGoEAwDbwJG
trackSlugPT: pagamentos
---

O próximo passo é configurar as condições de pagamento.

Mas antes é preciso esclarecer a diferença entre meios de pagamento e condições de pagamento. Como esses conceitos são parecidos, costumam gerar confusão na hora de configurar as condições de pagamento. 

## Meios de pagamento
Os meios de pagamento são as formas que podem ser usadas para o dinheiro trocar de mãos e, assim, viabilizar relações de compra e venda. A VTEX dá suporte a vários meios de pagamento, como cartões de crédito e de débito, boletos bancários, carteiras digitais e vales, entre outros.

## Condições de pagamento
Já as condições de pagamentos são as regras que deverão ser seguidas por uma pessoa que deseja comprar na sua loja. Na prática, as condições de pagamento são as opções que aparecem na tela do usuário no momento da finalização da compra.

Dito isso, podemos partir para a configuração das condições de pagamento em si.

## Configurações gerais
Para configurar uma condição de pagamento, primeiro você precisa cadastrar uma afiliação, conforme explicado no documento [Afiliações de Gateway](https://help.vtex.com/pt/tutorial/afiliacoes-de-gateway/).

O que não muda de uma condição de pagamento para outra é a necessidade de:
- Definir o nome da regra de acordo com o que ela representa, para ajudar a identificá-la;
- Ativá-la;
- Definir por qual afiliação de gateway essa condição será processada;
- Definir se você vai ou não usar [antifraude](https://help.vtex.com/pt/tutorial/como-configurar-antifraude?locale=pt).

Além disso, existe a possibilidade de definir se o pagamento será à vista ou em parcelas, com ou sem juros e [condições especiais](https://help.vtex.com/pt/tutorial/condicoes-especiais--tutorials_456?locale=pt "condições especiais").

Como o meio de pagamento que permite todas essas configurações é o **Cartão de Crédito**, siga as etapas abaixo para cada uma dessas configurações.

## À vista
Aqui, antes de ativar a condição de pagamento, você deve verificar com o gateway ou adquirente se a bandeira ou o meio de pagamento estão disponíveis no sistema deles.

Feito isso, siga as instruções:

1. No Admin VTEX, acesse **Configurações da loja** > **Pagamentos** > **Configurações**, ou digite **Configurações** na barra de busca no topo da página.
2. Clique em **Condições de pagamento**.
3. Clique no botão **+**.
4. Escolha um dos cartões de crédito como meio de pagamento.
5. Nomeie a regra no campo **Nome da regra**.
6. Ative a condição no campo **Status**.
7. No campo **Processar com a afiliação**, escolha a afiliação que configurou.
8. No campo **À vista ou parcelado?**, selecione a opção **À vista**.
9. Clique no botão **Salvar**.

## Parcelado

A configuração dos pagamentos parcelados é bem parecida com a dos feitos à vista. Entretanto, para esta opção, é possível definir se os pagamentos ocorrerão: sem juros, com juros ou via parcelamento automático.

### Sem juros

Vale ressaltar que o campo **Cobrança** só será levado em consideração para parcelamentos com juros. Logo, qualquer opção é válida.

1. No Admin VTEX, acesse **Configurações da loja** > **Pagamentos** > **Configurações**, ou digite **Configurações** na barra de busca no topo da página.
2. Clique em **Condições de pagamento**.
3. Clique no botão **+**.
4. Escolha um dos cartões de crédito como meio de pagamento.
5. Nomeie a regra no campo **Nome da regra**.
6. Ative a condição no campo **Status**.
7. No campo **Processar com a afiliação**, escolha a afiliação que configurou. 
8. No campo **À vista ou parcelado?**, selecione **parcelado**.
9. Configure o número de parcelas sequenciais ou individuais no campo **Total de parcelas**.
10. Defina uma parcela mínima para ser aplicada conforme o valor de cada produto.
11. Clique no botão **Salvar**.

### Com juros
Caso você decida configurar um meio de pagamento que aceite parcelas com juros, esse campo aceita valores com até duas casas decimais. Por exemplo, 1,25 ou 10,89 são valores possíveis.

1. No Admin VTEX, acesse **Configurações da loja** > **Pagamentos** > **Configurações**, ou digite **Configurações** na barra de busca no topo da página.
2. Clique em **Condições de pagamento**.
3. Clique no botão **+**.
4. Escolha um dos cartões de crédito como meio de pagamento.
5. Nomeie a regra no campo **Nome da regra**.
6. Ative a condição no campo **Status**.
7. No campo **Processar com a afiliação**, escolha a afiliação que configurou.
8. No campo **À vista ou parcelado?**, selecione **parcelado**.
9. Configure o número de parcelas sequenciais ou individuais no campo **Total de parcelas**.
10. Defina uma parcela mínima para ser aplicada conforme o valor de cada produto.
11. Selecione a data da cobrança (início ou fim do período).
12. Clique no botão **Adicionar juros**.
13. Digite o valor do juros que deseja aplicar a cada uma das parcelas.
14. Clique em **Juros composto aplicado. Alterar** para escolher entre juros composto ou simples.
15. Clique no botão **Salvar**.

### Parcelamento Automático
A opção de Parcelamento Automático permite que você configure os detalhes dos parcelamentos diretamente no provedor de pagamento (externamente ao ambiente VTEX).
Para habilitar esta opção, selecione “Sim” no campo **Usar parcelamento externo** durante a etapa de [configuração de afiliação](https://help.vtex.com/pt/tutorial/afiliacoes-de-gateway--tutorials_444).

![parcelamentoautomatico](//images.ctfassets.net/alneenqid6w5/3ErHSFlSGyUwbLzJWaUlXw/f05aa9a6c8ed312d82a5aa2e51b5fa03/parcelamentoautomaticobr.JPG)

<div class="alert alert-warning">
  Atualmente, somente a afiliação do MercadoPagoV1 permite a função de parcelamento automático.
</div>

Após habilitar o parcelamento automático na afiliação, siga os seguintes passos:

1. No Admin VTEX, acesse **Configurações da loja** > **Pagamentos** > **Configurações**, ou digite **Configurações** na barra de busca no topo da página.
2. Clique em **Condições de pagamento**.
3. Clique no botão **+**.
4. Escolha um dos cartões de crédito como meio de pagamento.
5. Nomeie a regra no campo **Nome da regra**.
6. Ative a condição no campo **Status**.
7. No campo **Processar com a afiliação**, escolha a afiliação que configurou.
8. Se desejar utilizar um sistema antifraude, selecione a opção **Usar antifraude**.
9. Selecione uma opção de antifraude. 
10. No campo **À vista ou parcelado?**, selecione **Automático**.
11. Clique no botão **Salvar**.

