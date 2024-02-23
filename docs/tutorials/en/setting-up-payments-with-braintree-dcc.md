---
title: 'Setting up payments with Braintree-DCC'
id: 3Is3N2MmTldXPa2FtiV8xy
status: PUBLISHED
createdAt: 2022-08-11T12:01:04.231Z
updatedAt: 2024-01-23T18:20:50.864Z
publishedAt: 2024-01-23T18:20:50.864Z
firstPublishedAt: 2022-08-11T12:27:01.656Z
contentType: tutorial
productTeam: Financial
author: 6DODK49lJPk3yvcoe6GB6g
slug: setting-up-payments-with-braintree-dcc
locale: en
legacySlug: setting-up-payments-with-braintree-dcc
subcategory: 3tDGibM2tqMyqIyukqmmMw
---

At VTEX, it is possible to integrate with the Braintree-DCC payment provider. With this provider, your store can make sales through a credit and debit cards.

To configure Braintree-DCC, follow the steps below:

1. In the VTEX Admin, go to __Store Settings > Payment > Providers__, or type __Providers__ in the search bar at the top of the page.
2. On the providers screen, click the `New Provider` button.
3. Type the name __Braintree-DCC__ in the search bar and click on the name of the provider.
4. Fill in the fields below your Braintree-DCC account information:
   - __Application Key__
   - __Application Token__
   - __Merchand Id (Braintree)__
   - __Forward (optional)__
   - __DelayToAutoSettle__
   - __PayPal Client ID (optional)__
   - __PayPal Secret (optional)__
   - __PayPal Payer ID (optional)__
   - __Merchant Account Id (optional)__
   - __Sandbox__
   - __Webhook (optional)__
   - __PayPal Merchant ID (optional)__
5. Click on `Save`.

To set up payment conditions, access [Configure special payment conditions](https://help.vtex.com/en/tutorial/condicoes-de-pagamento).

After following the indicated steps, Braintree-DCC connector may take up to 10 minutes to appear at your store's checkout as a payment option.
