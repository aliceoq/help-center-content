---
title: 'Orders with asterisks in the address for invoice'
id: 6AaZ4p042LZwvfeKIqavjw
status: PUBLISHED
createdAt: 2023-08-25T17:03:49.755Z
updatedAt: 2023-11-10T20:11:14.163Z
publishedAt: 2023-11-10T20:11:14.163Z
firstPublishedAt: 2023-08-25T17:03:50.594Z
contentType: knownIssue
productTeam: Checkout
author: 2mXZkbi0oi061KicTExNjo
tag: Checkout
slug: orders-with-asterisks-in-the-address-for-invoice
locale: en
kiStatus: Backlog
internalReference: 360783
---

## Summary


There are orders where the `invoiceAddress` or `shippingAddress` is being sent as 'masked' instead of the actual address. This behavior occurs when a user completes the purchase with an order form containing masked data that is 'stringified'. Since these are string fields, the order data is filled with the '***' mask.

So, the bug lies in the fact that our API to place orders allows objects with special characters in these fields.


##

## Simulation



1. Add some products to your cart;
2. During the checkout process, enter a valid billing address and log into your account;
3. Abandon the cart or leave the website without completing the purchase;
4. Use our API to insert an attachment and put an address with "***" in some fields, such as the neighborhood one;
5. Place an order using this same cart;
6. Note that the order will have the shipping data with these special characters.


##

## Workaround


N/A





