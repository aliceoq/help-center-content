---
title: 'Setting up PagSeguro V3'
id: 5Noi1mUbBQ6CyqdeDQtWfw
status: PUBLISHED
createdAt: 2021-12-02T12:14:58.698Z
updatedAt: 2024-01-23T20:57:44.838Z
publishedAt: 2024-01-23T20:57:44.838Z
firstPublishedAt: 2021-12-02T19:18:21.251Z
contentType: tutorial
productTeam: Financial
author: 6DODK49lJPk3yvcoe6GB6g
slug: setting-up-pagseguro-v3
locale: en
legacySlug: setting-up-pagseguro-v3
subcategory: 3tDGibM2tqMyqIyukqmmMw
---

If you have a PagSeguro account, you can configure PagseguroV3 on the VTEX gateway to receive payments by: boleto, PIX, debit and credit cards.

## Setting up PagseguroV3 gateway

1. In the VTEX Admin, go to __Store Settings > Payment > Providers__, or type __Providers__ in the search bar at the top of the page.
2. On the providers screen, click the `New Provider` button.
3. Type the name __PagSeguroV3__ in the search bar and click on the name of the provider.
4. In __Click to authorize VTEX to make payments__, click on __Authorize__. At this moment, you will be redirected to the PagSeguro webpage, where you will have to access your account, and authorize the connection of VTEX in your PagSeguro account.
5. After authorizing, you will automatically return to the VTEX Admin, and the __Application Key__, __Application Token__, __Application Id__ fields will already be filled in.
6. Click on __Save__.

## Setting up the payment condition

After following the steps indicated above, PagSeguroV3 will be configured in your store. Thus, while you're registering a payment condition, it will be available in the __Process with affiliation__ field (provided that the payment method is compatible with PagSeguroV3).

For more on how to set up payment conditions, access [configuring payment conditions](https://help.vtex.com/en/tutorial/condicoes-de-pagamento#).
