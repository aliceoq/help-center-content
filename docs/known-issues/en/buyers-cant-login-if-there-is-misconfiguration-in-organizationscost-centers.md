---
title: "Buyers can't login if there is misconfiguration in organizations/cost centers"
id: r5p7K15FkbZUDSOUQ6hGz
status: PUBLISHED
createdAt: 2023-11-30T22:21:39.852Z
updatedAt: 2023-12-01T20:19:35.375Z
publishedAt: 2023-12-01T20:19:35.375Z
firstPublishedAt: 2023-11-30T22:21:40.638Z
contentType: knownIssue
productTeam: B2B
author: 2mXZkbi0oi061KicTExNjo
tag: B2B
slug: buyers-cant-login-if-there-is-misconfiguration-in-organizationscost-centers
locale: en
kiStatus: Backlog
internalReference: 945609
---

## Summary


When a user has the first organization assigned to them is invalid with the wrong cost center id login fails with no message.

There will be the message `"App storefront-permissions failed, resulting in an error building the session"` in the session response.


##

## Simulation



- Create an organization with the wrong cost center id;
- Login in the site.


##

## Workaround


Fix the cost center id associated with the organization or delete the organization.



