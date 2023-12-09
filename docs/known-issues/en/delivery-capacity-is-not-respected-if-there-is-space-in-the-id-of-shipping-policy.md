---
title: 'Delivery capacity is not respected if there is space in the Id of Shipping Policy'
id: 1OyY54G05o15EI2zAmW4Vq
status: PUBLISHED
createdAt: 2023-07-14T21:25:50.522Z
updatedAt: 2023-07-28T21:37:08.673Z
publishedAt: 2023-07-28T21:37:08.673Z
firstPublishedAt: 2023-07-14T21:25:51.117Z
contentType: knownIssue
productTeam: Logistics
author: 2mXZkbi0oi061KicTExNjo
tag: Logistics
slug: delivery-capacity-is-not-respected-if-there-is-space-in-the-id-of-shipping-policy
locale: en
kiStatus: Backlog
internalReference: 862830
---

## Summary


If the delivery schedule feature is in use and the delivery capacity is activated, if there is a space in the Id of the shipping policy in question, the window will always be visible and the quantity configured for the delivery capacity will not be respected.


##

## Simulation


Create a shipping policy and in its Id insert a space, configure the scheduled delivery as well as the delivery capacity.
Place orders by selecting the registered window, verify that it will be possible to create more orders than the maximum configured in the delivery capacity.
At checkout once the configured limit is reached the window should not be unavailable, however it remains visible and possible to be selected.


##

## Workaround


Do not register any Id with space in the shipping policy.





