---
title: 'How does the Score field work?'
id: 1BUZC0mBYEEIUgeQYAKcae
status: PUBLISHED
createdAt: 2018-02-16T16:17:51.610Z
updatedAt: 2023-07-14T11:54:54.135Z
publishedAt: 2023-07-14T11:54:54.135Z
firstPublishedAt: 2018-02-16T18:09:11.291Z
contentType: tutorial
productTeam: Marketing & Merchandising
author: 7FpKZ0rc6k4WqeymES80cw
slug: how-does-the-score-field-work
locale: en
legacySlug: how-does-the-score-field-work
subcategory: 2g6LxtasS4iSeGEqeYUuGW
---

The __Score__ field, available for __Product__, __Category__ and __Brand__, is the value used to ensure the ordering of products in your store, and is also used as a tie-breaking criterion for other ordering options, such as lower price, better discount etc. By filling in this field, you can define the priority of some products over others, both on the storefront and on the search results page.

The field enumeration criterion follows a simple numeric order (1, 2, 3, 4...) to display the sequence in the storefront or on the search results page. 

By default, products without a registered score behave as if they had a score of 0.

The score of a product is the __sum of its own score plus those of category and brand__. That is: `Product score + category score + brand score`.

You can use the following parameters to implement the ordering:

- __Ascending order:__ `?O=OrderByScoreASC`
- __Descending order:__ `?O=OrderByScoreDESC`

It is best to enter the product score one by one, as your storefront probably changes constantly.

An example for the use of the score field is in specific events, like when your store needs to position certain products before others to ensure they are seen.

To add or change a score related to a product, please follow these steps:

1. In VTEX Admin, go to **Catalog > Products & SKUs**.
2. Click on `Add Product` to create a new product or click on `Update` on the product you want to edit.
3. Enter the desired score value in the **Score field**.

