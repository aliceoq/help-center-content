---
title: 'How does VTEX Intelligent Search work?'
id: 23mytRDsEduqLO0Lo7yufy
status: PUBLISHED
createdAt: 2020-03-05T14:57:22.014Z
updatedAt: 2024-02-07T13:18:52.194Z
publishedAt: 2024-02-07T13:18:52.194Z
firstPublishedAt: 2020-03-05T19:54:00.932Z
contentType: trackArticle
productTeam: Marketing & Merchandising
slug: how-does-vtex-intelligent-search-work
locale: en
trackId: 19wrbB7nEQcmwzDPl1l4Cb
trackSlugEN: vtex-intelligent-search
---

The Search Engine is the core of VTEX Intelligent Search's intelligence. It interprets the search term and displays a filtered and ordered list of products. This tool allows a more objective search through indexing and treatment of the catalog data.

This feature is included by default in VTEX Intelligent Search and covers the vast majority of scenarios. However, you can also adjust the Search Engine to improve search results. This guide covers the following:

* [Search behavior configuration](#search-behavior-configuration)
* [Alternative ways to search](#alternative-ways-to-search)
* [Indexing](#indexing)

## Search behavior configuration

There is a set of settings that change the products that are displayed in search results and their order. In the following sections, you will see the main definitions that affect search behavior.

### Defining searchable fields

Determines which product information is searchable. From this configuration, every search in the search bar checks the content of these fields to generate search results. Check the following table to understand which information is searchable by default and the other configuration options:

| Information | Configuration |
| - | - |
| Product name, brand, product ID (`ProductID`), product reference code (`ProductRefID`), SKU ID (`SKUID`), SKU reference code (`SKURefID`), and EAN  | This information is searchable by default in VTEX Intelligent Search. To remove any of this information, please contact our [Support](https://help.vtex.com/support?/cultureInfo=en-us). |
| Product and SKU specifications | Please contact our [Support](https://help.vtex.com/support?/cultureInfo=en-us) to add the desired specifications as searchable fields.<br /><br /> For example, if a shirt does not have the color in the product name or SKU, by default, Intelligent Search does not identify this attribute in a search for "blue shirt", bringing up shirts of different colors. However, if the color specification is configured as searchable, the search will likely return blue shirts at the top of search results.<br /><br /> Learn more about specifications in [Product and SKU specifications](https://help.vtex.com/en/tracks/catalogo-101--5AF0XfnjfWeopIFBgs3LIQ/2NQoBv8m4Yz3oQaLgDRagP). |
| Manufacturer code (`ManufactureID`) | Please contact our [Support](https://help.vtex.com/support?/cultureInfo=en-us) to set this field as searchable. |

For example: the "color" specification is set as searchable and the product was added with the name "Nike Total 90 Sneakers" and the color "black". If a customer searches for "Black Sneakers", the tool will return products that have the term "sneakers" and the color "black" at the top of search results.

You can include special characters ( `-` and `/`) when searching for a product.

<div class="alert alert-warning">
	<p>Choosing the search fields affects the <a href="https://help.vtex.com/en/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/5tBSYXb9EIdePa0MWTnFd0">merchandising rule</a> options, as only searchable fields can be used to set up the rules. For example, if you set only the <strong><code>SKUID</code></strong> field as searchable, you cannot promote a<strong><code> ProductID</code></strong> or a <strong><code>ProductRefID</code></strong> using merchandising rules. </p>
</div>

### Defining and sorting filter fields

In all search results, users can select filters. Some filters are pre-defined by default, but it is also possible to create more filters to meet  store needs. The display order is also customizable. Example: In a search results list, there can be filters for Price, Categories, and Brand.

### Configuring autocorrect

The user may make spelling mistakes when performing a search. The tool interprets these misspellings and shows similar products.

The Search Engine performs an automatic correction in each search. For each search term, a specific number of wrong characters is allowed. The number of accepted misspellings is called fuzzy.

The fuzzy varies according to the length of the search term. By default, if the term is 3 to 5 characters long, the fuzzy applied will be 1, which means that 1 misspelled character is allowed. For terms with 6 or more characters, the fuzzy used will be 2.

The predicted misspellings considering fuzzy = 1 are:

* Insert 1 extra character.
* Remove 1 character.
* Change 1 character.
* Swap 2 characters that are next to each other.

_For example_: Suppose a customer wants to search for the term `case`. Using the default configuration (fuzzy = 1 for terms of 3 to 5 characters), the Search Engine will show results for `case` in any search that contains accepted errors, such as:

* `chase` (insert 1 extra character)
* `cae` (remove 1 character)
* `cast` (change 1 character)
* `csae` (swap 2 characters that are next to each other)

<div class="alert alert-info">
	<p>Blanks are not considered in the fuzzy, so "base ball" will not be changed to "baseball". We recommend using <a href="https://help.vtex.com/en/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/1pxAWPEglBey1UFdvcetZV">synonyms</a> for such cases. </p>
</div>

### Configuring relevance

Relevance is the ordering principle of search results. In this section, you can assign weights and prioritize certain criteria in the Search Engine, such as popularity, release date, and promotions. The relevance of a product is composed by the combination of weights and priorities defined by each merchant.

_For example_: a merchant configured that "promotion" has greater relevance than other criteria. When a customer searches for "t-shirt", the tool might display the t-shirts on sale at the top of search results, depending on the weights assigned to other criteria.

For more information on how to customize the order of results to meet your store's needs, read the article [Relevance settings](https://help.vtex.com/en/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/1qlObWIib6KqgrfX1FCOXS).

<div class="alert alert-info">
	<p>When using Intelligent Search, two options define the sorting order of your collections. By using the <code>map=productClusterIds</code> command, you are setting the order of your collections to be the one pre-defined by the merchant, with its relevance criteria. If you choose to use <code>productClusterNames</code>, you are setting that you want your collections to follow Intelligent Search's own relevance standards.</p>
</div>

### Minimum result configuration

The search engine allows you to set the minimum number of products for multi-term queries. If this number is not reached, the search returns more comprehensive results, considering only one of the searched terms.

_For example_: the minimum result for multi-term queries was configured as **three**. The user searched for "nike sneakers", but there are only **four** products in the catalog with that name. The platform will first display products with the terms "nike sneakers", then products with the term "sneakers", and after that, those with the term "nike".

### Page limit

VTEX Intelligent Search limits search results to 50 pages. This feature encourages the customer to use filters, creating a more relevant and focused experience.

## Alternative ways to search

It is possible to search by the ID of one or more items in the search bar or by adding search parameters (*query*) in the store URL.

### Partial match

By entering the exact first digits of the product ID (`ProductID`), product reference code (`ProductRefID`), SKU ID (`SKUID`), SKU reference code (`SKURefID`), or EAN in the search bar, Intelligent Search will partially match products and SKUs active in the store, adding them to the search results.

For example, if the product ID is `123456789` and you search for `123`, it will be listed in the search results. However, the product will not be displayed if the search is `234` and does not include any of the first ID numbers.

### URL

To search from your store URL, add search parameters (*query*) at the end of the store URL, respecting one of the following structures:

- Example for searching an item: `[account address]/[id type]:[id_1]?q=[id type]&map=ft`
- Example for searching a list: `[account address]/[id type]:[id_1];[id_2];[id_3]?q=[id type]:[id_1];[id_2];[id_3]&map=ft`

The possible value types for the ID type field are `product.id`, `sku.id`,`sku.ean`, `sku.reference`, or `id` (ProductID, ProductRefID, SKUID, SKURefID, and EAN). All searched IDs should be of the same type.   

- **Search by SKU ID:**  `?q=sku.id:<id>` or `?q=sku:<id>`
- **Search by EAN:**  `?q=sku.ean:<id>`
- **Search by reference ID:**  `?q=sku.reference:<id>`
- **Search by slug:**  `?q=product.link:<link>`
- **Search by product ID:**  `?q=product:<id>` or `?q=product.id:<id>`

## Indexing

Indexing is the syncing process between store and search catalogs. This feature allows you to keep your content up to date with continuous updates of the product index. It also performs data processing to be used in the search.

Initially, it syncs all the products from your VTEX catalog. After that, data changes — such as product name and status — are updated in real time by the search indexer.

In this sync process, the system queues up the information that has been updated to add it to the search catalog. Once all changes have been indexed, they will be available on the website.

The indexing process is safe and has a retry mechanism — if an item is not indexed on the first attempt, the system makes subsequent attempts until it is successfully completed.

Indexing is fundamental to analyze, process, and organize data as best as possible to improve your search results.

Check [Indexing History](https://help.vtex.com/en/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/4flMwTaQL8FRKl1YT58ezH) for more information on how to monitor the indexing process.
