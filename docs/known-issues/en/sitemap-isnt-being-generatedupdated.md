---
title: "Sitemap isn't being generated/updated"
id: 1tJ4XHtbnFsfS30JWXwxb0
status: PUBLISHED
createdAt: 2023-05-17T13:58:46.443Z
updatedAt: 2024-02-16T18:17:17.707Z
publishedAt: 2024-02-16T18:17:17.707Z
firstPublishedAt: 2023-05-17T13:58:47.102Z
contentType: knownIssue
productTeam: Store Framework
author: 2mXZkbi0oi061KicTExNjo
tag: Store Framework
slug: sitemap-isnt-being-generatedupdated
locale: en
kiStatus: Backlog
internalReference: 827104
---

## Summary



There are three scenarios where the sitemap is not being generated/updated:



1. When we have a product not found or with some kind of problem on the catalog the sitemap is not generated. You can search for the logs on OpenSearch, in this case, to check which product has a problem;



2. When the account has the app `search.resolver@1.x`  the sitemap can have errors when:



- A category has its first product coming from a similar category (the merch rules can have an impact on this case depending on the product you're promoting);

- The search/brand/category page has no products, in this case, the page is not indexed on the sitemap, and its generation crashes


3. Products that don't have the trade policy set on the catalog won't be received by the sitemap



##

## Simulation



Try to generate the sitemap for an account that has one of the scenarios described above and it will crash


##

## Workaround




- Create a new workspace
- Install the search-resolver@0.x `(vtex install vtex.search-resolver@0.x)`
- Generate the new sitemap
- Now you can rollback search-resolver to 1.x (`vtex install vtex.search-resolver@1.x`)
- Promote the created workspace to master

Obs: This workaround may not work at all times. Sometimes the store can have so many invalid products that even the `search-resolver@0.x` will not update the sitemap.

But eventually, you will need to fix the scenario that prevents the sitemap from being generated

Stay in mind that updating the store to resolver@0.x and generate the sitemap in a workspace is the workaround because some invalid cases don't happen in our legacy search





