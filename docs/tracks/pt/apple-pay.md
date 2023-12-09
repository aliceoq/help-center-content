---
title: 'Apple Pay'
id: STKWiXJSR9ImPt5EEC2aL
status: PUBLISHED
createdAt: 2023-06-28T14:04:58.979Z
updatedAt: 2023-06-28T14:13:24.803Z
publishedAt: 2023-06-28T14:13:24.803Z
firstPublishedAt: 2023-06-28T14:13:24.803Z
contentType: trackArticle
productTeam: Shopping
slug: apple-pay
locale: pt
trackId: 6X8YyZBoVJpz5R8oXciTyu
trackSlugPT: carteira-digital-e-wallet
---

Seus clientes podem fazer compras usando o Apple Pay, a [carteira digital](https://help.vtex.com/pt/tracks/digital-wallet-e-wallet--6X8YyZBoVJpz5R8oXciTyu/7jLbdfch9Oe2yYbQa9zwE1) da Apple. Para isso, você precisa cumprir alguns requisitos:

- Ter conta em `developer.apple.com`.
- Ter contrato com um gateway que processe pagamentos com Apple Pay.

<div class="alert alert-warning">
  O Apple Pay funciona atualmente somente nos sistemas operacionais MacOs e IOS, e no navegador Safari. Para maiores informações, acesse <a href="https://support.apple.com/pt-br/HT208531">Dispositivos compatíveis com o Apple Pay</a>.
</div>

Com os requisitos cumpridos, basta seguir os passos abaixo para oferecer essa condição de pagamento na sua loja.

## Configurar afiliação de gateway

Oferecer condições de pagamento aos clientes da sua loja depende de afiliações de gateway capazes de processá-las. Na plataforma VTEX, as afiliações compatíveis atualmente com o __Apple Pay__ são: __ERedeREST__ (integração da adquirente Rede), __Adyen__ e __Stripe__.

Nestes artigos, você tem o passo a passo para configurar o [ERedeREST](/pt/tutorial/configurar-adquirente-rede-com-o-erederest), [Adyen](/pt/tutorial/como-configurar-o-gateway-adyen-na-vtex) e [Stripe](https://help.vtex.com/pt/tutorial/configuring-stripe-gateway-affiliation--fwF2wk2FQKrODrWWkvSLO). 

Mas lembre-se: é fundamental [registrar o Merchant ID no Apple Pay](https://developers.vtex.com/vtex-rest-api/docs/setting-up-merchant-id-in-apple-pay) antes de fazer a configuração da afiliação de gateway.

## Baixar e instalar aplicativo da VTEX App Store

1. No menu lateral do admin, clique em __Apps__.
2. Acesse o link __VTEX App Store__ ou use a URL `https://apps.vtex.com/?an={{AccountName}}` direto no navegador, trocando `{{AccountName}}` pelo store name em que deseja oferecer o Apple Pay.
3. Procure pelo app __Apple Pay__ e clique em `Get`.
4. Você será direcionado para uma tela de revisão de pedido. Confira os dados e clique no botão `Confirm order and begin installation`.
5. Com tudo certo, você vai para a tela de instalação. Lá, você pode rever as permissões do aplicativo e iniciar o download (clicando em `Instalar`).
6. O app vai ser instalado no seu workspace, mas precisará que você preencha o __Merchant ID__ (no campo __Merchant Identifier__) para ser aplicado na sua loja.
7. Clique em `Salvar`. 

## Configurar condição de pagamento Apple Pay

1. No Admin VTEX, acesse **Configurações da loja** > **Pagamentos** > **Configurações**, ou digite **Configurações** na barra de busca no topo da página.
2. Clique na aba __Condições de pagamento__ e, em seguida, no botão `+`.
3. Selecione o meio de pagamento __Apple Pay__.
4. Clique no botão `Status` para ativar essa condição de pagamento.
5. No campo __Processar com a afiliação__, selecione a opção que vai ser usada para processar os pagamentos.
6. Se houver um antifraude configurado na sua loja, você pode ativá-lo para essa condição de pagamento marcando a caixa __Usar Antifraude__.
7. Escolha se deseja que os pagamentos sejam feitos à vista ou parcelados.
8. Se quiser, você também pode optar por uma [condição especial de pagamento](/pt/tutorial/condicoes-especiais).
9. Clique em `Salvar`.

Depois de seguir os passos indicados, o __Apple Pay__ vai aparecer no checkout da sua loja como uma opção de pagamento para seus clientes utilizarem.

### Artigos relacionados

- [Configurar adquirente Rede com o ERedeREST](/pt/tutorial/configurar-adquirente-rede-com-o-erederest)
- [Configurar o gateway Adyen na VTEX](/pt/tutorial/como-configurar-o-gateway-adyen-na-vtex)
- [Configurando Merchant ID no Apple Pay](https://developers.vtex.com/vtex-rest-api/docs/setting-up-merchant-id-in-apple-pay)
- [Configurar condições especiais de pagamento](/pt/tutorial/condicoes-especiais)
