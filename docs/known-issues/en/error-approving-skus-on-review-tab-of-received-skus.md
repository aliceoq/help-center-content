---
title: 'Error approving skus on Review Tab of Received Skus'
id: 7fRMTxq7CFRkyZeK08AGIg
status: PUBLISHED
createdAt: 2023-11-23T13:46:30.453Z
updatedAt: 2023-11-23T13:46:31.370Z
publishedAt: 2023-11-23T13:46:31.370Z
firstPublishedAt: 2023-11-23T13:46:31.370Z
contentType: knownIssue
productTeam: Marketplace
author: 2mXZkbi0oi061KicTExNjo
tag: Marketplace
slug: error-approving-skus-on-review-tab-of-received-skus
locale: en
kiStatus: Backlog
internalReference: 940998
---

## Summary


When a sku fails the Offer Quality optional rules created by the Marketplace, it goes directly to the "Review Tab" of Received Skus.

However, when trying to approve the sku, an error message is returned: "Sorry, something went wrong in the Catalog. Please try again or contact VTEX if the problem persists."

This happens because the Matcher module was not able to fill the product and sku information after sending the sku to the Review Tab (you can check this using the APIs):
 ![](https://vtexhelp.zendesk.com/attachments/token/0Dti3ak7twOpuVzvzntmPCGit/?name=image.png)


##

## Simulation



1. Create a optional rule on Offer Quality;
2. Wait for a sku to fail the rule and go to the Review Tab;
3. Try to approve the sku and get an error message;
4. Check via API if the matches object is filled like the image above.


##

## Workaround


Approve the sku via API passing the correct product and sku information manually.





