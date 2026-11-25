# Commerce Index Insight

A plugin for Claude. It reviews your own Shopify store's catalog with the Commerce Index connector.
It finds variants priced below unit cost, margins under your margin floor, compare-at prices below the selling price, variants with no sellable stock, and missing prices or costs.
It can also work out what a price or cost change would do. That is arithmetic, not a forecast.

## What it brings

- The Commerce Index connector: https://commerceindex.com/api/connector/mcp
- One skill, `catalog-review`, that tells Claude how to run a review and how to present it.

## What data goes where

- The review of your own store's catalog goes from Commerce Index to the assistant you use.
- The connector only reads. Nothing is changed in your store.
- From there, the terms of your assistant's provider apply.
- Commerce Index keeps the list of connections: the store, a coded form of the staff member's Shopify id, the assistant's name and host, whether costs are included, and dates. It keeps its own sign-in tokens and access keys only as hashes. It also keeps one Shopify token per store, encrypted.
- Commerce Index keeps no products, prices, costs, stock figures, questions or answers.

## How to connect

1. Add the connector. A sign-in window opens and shows a code.
2. In Shopify admin, open the Commerce Index app and choose "Connect an assistant".
3. Type the code there and approve.

You never type your store address. Do not paste the code into the chat.

## Requirements

- The Commerce Index app installed on your Shopify store.
- A staff account that can open the app. To see margins, it must be able to view product costs.

## Support and privacy

- Support: mithun.kadur@sagisu.com
- Privacy policy: https://commerceindex.com/privacy
