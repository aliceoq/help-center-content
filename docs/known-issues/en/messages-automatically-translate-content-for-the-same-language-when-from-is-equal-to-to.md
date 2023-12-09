---
title: "Messages automatically translate content for the same language (when 'from' is equal to 'to')"
id: 7OIKmmhO3Pa2z0pIU33kY
status: PUBLISHED
createdAt: 2023-07-20T15:28:57.078Z
updatedAt: 2023-07-20T15:28:57.934Z
publishedAt: 2023-07-20T15:28:57.934Z
firstPublishedAt: 2023-07-20T15:28:57.934Z
contentType: knownIssue
productTeam: Store Framework
author: 2mXZkbi0oi061KicTExNjo
tag: Store Framework
slug: messages-automatically-translate-content-for-the-same-language-when-from-is-equal-to-to
locale: en
kiStatus: Backlog
internalReference: 865918
---

## Summary


The Messages app automatically translates content when the language 'from' is equal to 'to'.

When implementing multi-language stores and the content has a foreign language word, for example, if a product name is translated from English to Spanish but still has English words, it will show an undesired translation.


##

## Simulation



- Translate any content from the store to any other language different from the default;
- Make sure there is still at least one word in a different language than the translated one;
- Check the storefront; it won't match the translation.


##

## Workaround



- Disable the automatic translation;
- Translate the content where the language 'from' is equal to 'to', for example, from 'es-ES' to 'es-ES'.



