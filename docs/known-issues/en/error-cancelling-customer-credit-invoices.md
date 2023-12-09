---
title: 'Error cancelling Customer Credit invoices'
id: 75nZNOHGYGBlAoTOjG6gs
status: PUBLISHED
createdAt: 2023-10-26T21:09:54.255Z
updatedAt: 2023-10-26T21:09:54.992Z
publishedAt: 2023-10-26T21:09:54.992Z
firstPublishedAt: 2023-10-26T21:09:54.992Z
contentType: knownIssue
productTeam: Payments
author: 2mXZkbi0oi061KicTExNjo
tag: Payments
slug: error-cancelling-customer-credit-invoices
locale: en
kiStatus: Backlog
internalReference: 926563
---

## Summary


We found cases where an invoice can't be cancelled, when running the DEL API we get an error 500 with the below response:

`"message": "An error has occurred."`


##

## Simulation


We were not able to replicate this bug, seems related to old invoices (dated before 2023)


##

## Workaround


NA




