---
title: 'Configurar pagamento com CieloEcommerce'
id: 6zuELBqEo0QzApbU4l7L4
status: PUBLISHED
createdAt: 2023-09-18T14:07:22.540Z
updatedAt: 2023-09-18T15:29:57.321Z
publishedAt: 2023-09-18T15:29:57.321Z
firstPublishedAt: 2023-09-18T15:29:57.321Z
contentType: tutorial
productTeam: Financial
author: 6DODK49lJPk3yvcoe6GB6g
slug: configurar-pagamento-com-cieloecommerce
locale: pt
legacySlug: configurar-pagamento-com-cieloecommerce
subcategory: 3tDGibM2tqMyqIyukqmmMw
---

Na VTEX, é possível realizar a integração com o CieloEcommerce. Com este conector, sua loja pode realizar vendas com cartões de crédito, débito, private labels, cobranded, boletos bancário, PIX, entre outros. Para configurar a CieloEcommerce, siga os passos abaixo:

1. No Admin VTEX, acesse __Configurações da loja__ > __Pagamentos__ > __Configurações__, ou digite __Configurações__ na barra de busca no topo da página.
2. Na aba __Afiliações de Gateway__, clique no botão __+__.
3. Clique no conector __CieloEcommerce__.
4. Preencha os campos __Application Key__ e __Application Token__ com as informações da sua conta CieloEcommerce.
5. Em __Integration__, selecione se o conector será utilizado como __Adquirencia__ ou __Gateway__.
6. Em __Provider__, selecione o adquirente a ser utilizado com o conector CieloEcommerce.
7. Em __IsSplit__, escolha se a opção de split estará disponível.
8. Em __UseMPi__, escolha se as transações serão autenticadas. Caso selecione “Yes”, siga para o Passo 9. Caso selecione “No”, siga para o Passo 10.
9. Preencha os campos __MpiClientId__, __MpiClientSecret__, __MpiMerchantName__, __MpiMCC__ e __MpiEstablishmentCode__ com os seus dados de acesso Mpi.
10. Em __SoftDescriptor__, indique a informação a ser exibida para identificar a transação realizada na sua loja.
11. Em __Captura__, selecione o período em que a captura do pagamento deve ser solicitada. O tempo padrão será realizado quatro dias após a autorização.
12. Em __Ativar split e enviar recebedores?__, selecione se o split de pagamentos estará disponível para o marketplace e os sellers.
13. Clique em `Salvar`.

Para configurar os métodos de pagamento a serem processados pela CieloEcommerce, acesse [Condições de Pagamento](https://help.vtex.com/pt/tutorial/condicoes-de-pagamento). 

Para definir condições especiais sobre os métodos de pagamento, acesse [Configurar condições especiais de Pagamento](https://help.vtex.com/pt/tutorial/condicoes-especiais--tutorials_456#).

Depois de seguir os passos indicados, o conector CieloEcommerce pode demorar até 10 minutos para aparecer no checkout da sua loja como uma opção de pagamento. 
