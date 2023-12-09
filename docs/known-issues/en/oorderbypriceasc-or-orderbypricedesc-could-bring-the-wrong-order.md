---
title: 'O=OrderByPriceASC (or OrderByPriceDESC) could bring the wrong order'
id: 2XCplZQutilKeD2bNnjYDx
status: PUBLISHED
createdAt: 2022-05-20T15:48:15.215Z
updatedAt: 2023-10-19T12:52:38.615Z
publishedAt: 2023-10-19T12:52:38.615Z
firstPublishedAt: 2022-05-20T15:48:16.089Z
contentType: knownIssue
productTeam: Portal
author: 2mXZkbi0oi061KicTExNjo
tag: Portal
slug: oorderbypriceasc-or-orderbypricedesc-could-bring-the-wrong-order
locale: en
kiStatus: Backlog
internalReference: 582861
---

## Summary


O=OrderByPriceASC (or OrderByPriceDESC) can use wrong policy to order prices.


##

## Simulation



- Enter more than one price on the product. Ex: two different list prices on different sellers
- Put page sorting by price (ex: O=OrderByPriceASC)
- See that the sorting is not in the order of the prices being displayed


##

## Workaround


None on the Portal. However, the account can switch to Inteligente Search.





