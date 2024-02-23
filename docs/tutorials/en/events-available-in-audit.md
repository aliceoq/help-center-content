---
title: 'Events available in Audit'
id: 6r1Mzcu5NmkmmDLJlz9CCZ
status: PUBLISHED
createdAt: 2022-06-22T16:05:16.214Z
updatedAt: 2024-01-18T20:46:19.490Z
publishedAt: 2024-01-18T20:46:19.490Z
firstPublishedAt: 2022-06-22T16:28:52.801Z
contentType: tutorial
productTeam: Master Data
author: 2Gy429C47ie3tL9XUEjeFL
slug: events-available-in-audit
locale: en
legacySlug: events-available-in-audit
subcategory: 2TNXiKzLZOPxjMTyGiEeJu
---

Below, you will find a list of the potential events available in [Audit](https://help.vtex.com/pt/tutorial/searching-for-events-on-audit--5RXf9WJ5YLFBcS8q8KcxTA#) for each app.

* [OMS](#oms)
* [Orders](#orders)
* [Inventory & Shipping](#inventory-shipping)
* [Catalog (Admin)](#catalog-admin)
* [Catalog (API)](#catalog-api)
* [Prices](#prices)
* [Promotions](#promotions)
* [Wallets](#wallets)
* [Checkout](#checkout)
* [Portal CMS](#portal-cms)
* [License Manager](#license-manager)
* [VTEX ID](#vtex-id)
* [Headless CMS](#headless-cms)

<div class = "alert alert-info">
In case you encounter an event in Audit which has not been included in this list, please inform us through the <a href="https://docs.google.com/forms/d/e/1FAIpQLSfmnotPvPjw-SjiE7lt2Nt3RQgNUe10ixXZmuO2v9enOJReoQ/viewform">documentation feedback page</a>.
</div>

<div class="alert alert-warning">
<p>In the Audit filter options, you can find <strong>Shipping Options</strong>, <strong>Profile System</strong>, and <strong>Billing</strong> options besides the applications listed in this guide. Since these options refer to internal resources or features in closed beta, most accounts will not have events associated with them.</p>
</div>

## OMS

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Action</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event description</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event details</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Start Handling
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Informs VTEX that the store has started handling an order. This helps order workflow.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Order ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Change Status
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Change in order status.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Order ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Shipping Notification
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Shipping notification of a certain order.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Order ID.
    </td>
   </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Payment Notification
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Payment notification of a certain order.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Order ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Save Configuration
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Change in price module settings.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Short description of the change.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Resend Last Email
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Resending the last email related to the order in the Message Center.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Order ID.
   </td>
  </tr>
</table>

## Orders

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Action</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event description</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event details</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Change State
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Change in order status.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Order ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Order Cancellation
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Cancellation of an order.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Order ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Start Handling
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Action that signals to VTEX that the store has started handling a given order. This triggers the continuation of the flow of this order.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Order ID.
    </td>
   </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Notify Payment
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Payment notification for a given order.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Order ID.
   </td>
  </tr>
</table>

## Inventory & Shipping

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Action</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event description</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event details</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Carrier Create
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Carrier creation.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Carrier ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Carrier Update
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Carrier update.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Carrier ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Carrier Delete
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Carrier deletion.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Carrier ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Dock Create
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Loading dock creation.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Loading dock ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Dock Update
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Loading dock update.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Loading dock ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Dock Delete
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Loading dock deletion.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Loading dock ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Warehouse Create
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Warehouse creation.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Warehouse ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Warehouse Update
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Warehouse update.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Warehouse ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Warehouse Delete
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Warehouse deletion.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Warehouse ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Pickup Point Save
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Pickup point creation or change.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Pickup point ID.
   </td>
  </tr>
</table>

## Catalog (Admin)

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Action</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event description</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event details</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Product Activation
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Product activation.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Product ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Product Commercial Condition Change
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Change in product commercial condition.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Product ID and changed list of conditions.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">SKU Attachment Association    
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">SKU Attachment Association.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">SKU ID, name and attachment ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Archive Upload    
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">File delivery.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">File name.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Field Activation    
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Catalog field activation.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Field name, ID and status.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">SKU Seller Binding    
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">SKU and seller binding.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Seller’s ID, SKU ID in seller’s catalog and SKU ID in the marketplace catalog.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">SKU Seller Unbinding
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Removal of SKU and seller binding.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Seller’s ID, SKU ID in seller’s catalog and SKU ID in the marketplace catalog.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">SKU Seller Removal
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Removal of seller SKU.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">SKU ID in seller’s catalog.
   </td>
  </tr>
</table>

## Catalog (API)

| Action | Description | Event details |
|---|---|---|
| SKU Seller Binding Removal | SKU Binding Removal. | SKU ID in seller and seller ID. |
| Seller Update | Seller update. | Seller ID. |
| Seller Creation | Seller creation. | Seller ID. |
| SKU Seller Binding Activation | SKU binding activation. | SKU ID in seller and seller ID. |
| SKU Seller Binding Inactivation | SKU binding inactivation. | SKU ID in seller and seller ID. |

## Prices

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Action</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Description</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event details</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Put Price
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Creation or change of a SKU price.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">SKU ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Save Price Table
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Creation or change of a price table.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Identifies the created or changed table.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Save Price Tables
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Creation or change of multiple price tables.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Identifies the created or changed tables.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Price Deleted
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Deletion of a SKU price.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">SKU ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Save Config
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Creation or change of price settings.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Identifies the created or changed configuration.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Fixed Price Modified
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Change of fixed price.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Identification of the fixed price changed.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Put Catalog Step
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Creation or change of a price rule.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Price rule created or changed.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Deleted Fixed Prices From Table
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Deletion of fixed price from the related price table.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Identification of the table and the deleted price.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Compatibility Post Prices
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Change of price using the compatibility API with the PricingV1 contract
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Identification of the changed price.
   </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Change Rnb Config
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Change in price settings for new accounts.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Name of the account that made the change.
    </td>
   </tr>
</table>

## Promotions

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Action</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event description</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event details</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Archive Coupon
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Archived a coupon.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Coupon code.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Unarchive Coupon
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Unarchived a coupon.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Coupon code.
    </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Change Rate Configuration
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Change in fee settings.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Fee configuration ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Change Promotion Configuration
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Change in promotion settings.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Promotion configuration ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Change Coupon Configuration
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Coupon change.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Coupon code.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Unarchived Calculator
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Unarchived promotion or fee.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Promotion or fee configuration ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">Archived Calculator
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Archived promotion or fee.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Promotion or fee configuration ID.
    </td>
  </tr>
</table>

## Wallets

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Action</strong>
    </td>
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Event description</strong>
    </td>
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Event details</strong>
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">TOGGLE_WALLET
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Activate or deactivate a digital wallet.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">toggle-wallet-action
    </td>
  </tr>
</table>

## Checkout

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Action</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event description</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event details</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">SaveOrderFormConfiguration
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Change in OrderForm settings, which is in charge of running the store checkout.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Action description (“configurated OrderForm”)
   </td>
  </tr>
</table>

## Portal CMS

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Action</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event description</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event details</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">File Update
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Change in portal file.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">File name and ID changed.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">File Upload
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Portal file upload.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">File name changed.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">File Deleted
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">File removal.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">File name and ID changed.
   </td>
  </tr>
</table>

## License Manager

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Action</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event description</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event details</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Block AppToken
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Application key blocking.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Application key blocked.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Accept Sponsor Invite
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Accept the invitation to become the sponsor user.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID of the user who accepted the invitation.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Save User
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Create a user or change user information.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">User ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Save Account
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Create an account or edit account information.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Created or changed account.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Change Role
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Access role editing.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Role edited.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Delete Role
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Deletion of a role.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Role deleted.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Unblock AppToken
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Application key unlocking.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Unblocked application key.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Resource Access Allowed
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Resource access allowed.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Resource key and user ID to which access has been allowed.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Cancel Sponsor Invite
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Cancellation of sponsor user invitation.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID of invited user.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Delete User
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Deletion of a user.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID of deleted user.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Update Binding
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Binding update.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Binding updated.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Resource Access Denied
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Resource access denied.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Resource key and user ID to which access was denied.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Create New AppToken
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Creation of application key.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Application key created.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">Create Sponsor Invite
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Creation of a sponsor user invitation.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">ID of invited user.
   </td>
  </tr>
</table>

## VTEX ID

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Action</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event description</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event details</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">PasswordCreated
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Creation of a first-time password in the store or the VTEX Admin
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">User ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">PasswordUpdated
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Change of store or VTEX Admin password by the user.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">User ID.
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">IdentityProviderChanged
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Identity provider configuration change. For example: Creating a customized OAuth integration and changing information in an existing OAuth configuration.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Identity provider.
   </td>
  </tr>
</table>

## Master Data

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;"><strong>ACtion</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event description</strong>
   </td>
   <td class="t-body pa5" style="min-width: 15rem;"><strong>Event details</strong>
   </td>
  </tr>
  <tr class="bb b--muted-3">
   <td class="t-body pa5" style="min-width: 15rem;">DeleteDocument
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Deleted document.
   </td>
   <td class="t-body pa5" style="min-width: 15rem;">Document ID.
   </td>
  </tr>
</table>

## Headless CMS

<table class="w-100 center mv7 bb b--gray" style="border-spacing: 0px; border-collapse: collapse;">
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Action</strong>
    </td>
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Event description</strong>
    </td>
    <td class="t-body pa5" style="min-width: 15rem;"><strong>Event details</strong>
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">TRY_PUBLISHING
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Attempt to publish a page.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Event ID.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">TRY_PUBLISH_IN_RELEASE
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Attempt to publish a release.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Event ID.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">TRY_UNPUBLISHING
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Attempt to unpublish a page.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Event ID.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">RESTORE_CONTENT
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Content restore.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Event ID.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">TRY_UPDATING_DRAFT
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Attempt to update a draft.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Event ID.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">TRY_UNPUBLISHING_AND_OVERWRITING
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Attempt to unpublish and overwrite a page.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Event ID.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">done.invoke.deleteContent</td>
    <td class="t-body pa5" style="min-width: 15rem;">Delete content.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Event ID.
    </td>
  </tr>
  <tr class="bb b--muted-3">
    <td class="t-body pa5" style="min-width: 15rem;">done.invoke.deleteContentVariant
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Delete content version.
    </td>
    <td class="t-body pa5" style="min-width: 15rem;">Event ID.
    </td>
  </tr>
</table>

In the **Action** column, all Headless CMS events also display the following information:

* **CONTENT_ID:** unique identifier of the content.
* **VARIANT_ID:** unique identifier of the content version.
* **WORKSPACE**: workspace where the action occurred.
