---
title: 'Setting up payments with CieloEcommerce'
id: 6zuELBqEo0QzApbU4l7L4
status: PUBLISHED
createdAt: 2023-09-18T14:07:22.540Z
updatedAt: 2023-09-18T15:29:57.321Z
publishedAt: 2023-09-18T15:29:57.321Z
firstPublishedAt: 2023-09-18T15:29:57.321Z
contentType: tutorial
productTeam: Financial
author: 6DODK49lJPk3yvcoe6GB6g
slug: setting-up-payments-with-cieloecommerce
locale: en
legacySlug: setting-up-payments-with-cieloecommerce
subcategory: 3tDGibM2tqMyqIyukqmmMw
---

At VTEX, it is possible to integrate with the CieloEcommerce. With this connector, your store can make sales through credit, debit, private labels and cobranded cards, bank invoices, PIX, among others. To configure CieloEcommerce, follow the steps below:

1. In the VTEX Admin, go to __Store Settings__ > __Payment__ > __Settings__, or type __Settings__ in the search bar at the top of the page.
2. In the __Gateway affiliations__ tab, click on the __+__ button.
3. Click on the __CieloEcommerce__ connector.
4. Fill in the __Application Key__ and __Application Token__ fields with data provided by CieloEcommerce.
5. In __Integration__, select whether the connector will be used as __Adquirencia__ or __Gateway__.
6. In __Provider__, select the acquirer to be used with the CieloEcommerce connector.
7. In __IsSplit__, choose whether the split option will be available.
8. In __UseMpi__, choose whether transactions will be authenticated. If you select “Yes”, go to Step 9. If you select “No”, go to Step 10.
9. Fill in the __MpiClientId__, __MpiClientSecret__, __MpiMerchantName__, __MpiMCC__, and __MpiEstablishmentCode__ fields with you Mpi access data.
10. In __SoftDescriptor__, indicate the information to be displayed to identify the transaction carried out in your store.
11. In __Captura__, select the period in which payment capture should be requested. Standard time will be held four days after authorization.
12. In __Enable payout split and send payment recipients?__, select whether split payments will be available for the marketplace and sellers.
13. Click on `Save`.

To configure the payment methods to be processed by CieloEcommerce, access [Configuring Payment Conditions](https://help.vtex.com/en/tutorial/how-to-configure-payment-conditions--tutorials_455#).

To set special conditions on payment methods, go to [Configuring payment special conditions](https://help.vtex.com/en/tutorial/special-conditions--tutorials_456#).

After following the indicated steps, CieloEcommerce connector may take up to 10 minutes to appear at your store's checkout as a payment option.
