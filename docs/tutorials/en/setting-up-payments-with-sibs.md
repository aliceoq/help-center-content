---
title: 'Setting up payments with SIBS'
id: sNLPtJlAMnDpq40CCPKNo
status: PUBLISHED
createdAt: 2023-04-06T18:57:27.591Z
updatedAt: 2023-10-18T16:57:05.576Z
publishedAt: 2023-10-18T16:57:05.576Z
firstPublishedAt: 2023-04-06T19:07:28.327Z
contentType: tutorial
productTeam: Financial
author: 6DODK49lJPk3yvcoe6GB6g
slug: setting-up-payments-with-sibs
locale: en
legacySlug: setting-up-payments-with-sibs
subcategory: 3tDGibM2tqMyqIyukqmmMw
---

At VTEX, it is possible to integrate with the SIBS payment provider. With this connector, your store can make sales through SIBS credit card, Notes Payable, MBWay and MultiBanco.

To configure SIBS affiliation, follow the steps below:

1. In the VTEX Admin, go to __Store Settings > Payments > Settings__, or type __Settings__ in the search bar at the top of the page.
2. In the __Gateway affiliations__ tab, click on the `+` button.
3. Click on the __SIBS__ connector.
4. Fill in the __Application Key__ and __Application Token__ fields with data provided by SIBS.
5. In the __Payment settlement__ field, select one of the available options:

    - __Use Behavior Recommended By The Payment Processor__: capture is not automatic; it is scheduled according to the period specified by the acquirer. The acquirer indicates whether the payment has been authorized and can determine or recommend a number of days for the capture upon payment authorization.
    - __Immediate: Automatic Settlement After Payment Authorization__: capture is automatically performed right after payment authorization, even if the transaction includes an anti-fraud analysis.
    - __Immediate: Automatic Settlement After Anti-Fraud Analysis__:  Capture is automatically performed right after payment authorization and anti-fraud analysis. If you select this behavior and do not have anti-fraud analysis, the system will perform the payment capture as in __Immediate: Automatic Settlement After Payment Authorization__.
    - __Deactivated: Not Automatically Captured__: capture takes place only when the order is invoiced. If you select this behavior, it is important to pay attention to the invoicing time, as invoicing can exceed the capture time agreed with the payment provider and lead to the cancellation of the transaction.

<ui>  6. If an alert message appears indicating the need to install the app, click on the <b>Install app</b> button and follow the installation instructions.</ui>

<ui>  7. Click on <b>Save.</b></ui>

To configure the payment methods to be processed by SIBS, access [Configuring Payment Conditions](https://help.vtex.com/en/tutorial/how-to-configure-payment-conditions--tutorials_455#).

To set special conditions on payment methods, go to [Configuring payment special conditions](https://help.vtex.com/en/tutorial/special-conditions--tutorials_456#).

After following the indicated steps, SIBS connector may take up to 10 minutes to appear at your store's checkout as a payment option.
