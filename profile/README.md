# Opoha

**The Laravel of Commerce** — an open-source, API-first commerce engine you own and extend with plugins.

Opoha is not a Shopify clone or a turnkey storefront. It is a modular GraphQL commerce framework: core stays small and universal; everything that varies by business, country, or provider lives in plugins.

## Start here

```bash
npx @opoha/create-opoha@latest my-store
cd my-store && pnpm install && pnpm docker:up && pnpm dev
```

| | |
|---|---|
| **Engine** | [opoha-core](https://github.com/Opoha/opoha-core) |
| **Admin** | [opoha-admin](https://github.com/Opoha/opoha-admin) |
| **SDK** | [opoha-sdk](https://github.com/Opoha/opoha-sdk) |
| **Plugin SDK** | [opoha-plugin-sdk](https://github.com/Opoha/opoha-plugin-sdk) |
| **CLI / scaffold** | [opoha-cli](https://github.com/Opoha/opoha-cli) · [create-opoha](https://github.com/Opoha/create-opoha) (`@opoha/create-opoha`) |
| **Docs** | [opoha-docs](https://github.com/Opoha/opoha-docs) |

## Why Opoha

- **API-first** — GraphQL is the contract; Admin and storefronts consume it
- **Plugin-extensible** — payments, shipping, tax, search, storage without forking core
- **You own the stack** — modular monolith you deploy; no core source patches for customization
- **DX-first** — CLI, typed SDK, plugin contracts, shared toolkit

## Official plugins

| Category | Repos |
|----------|--------|
| Payments | [`plugin-manual-payment`](https://github.com/Opoha/plugin-manual-payment), [`plugin-stripe`](https://github.com/Opoha/plugin-stripe), [`plugin-omise`](https://github.com/Opoha/plugin-omise), [`plugin-paypal`](https://github.com/Opoha/plugin-paypal) |
| Shipping | [`plugin-shipping-flat-rate`](https://github.com/Opoha/plugin-shipping-flat-rate), [`plugin-dhl`](https://github.com/Opoha/plugin-dhl) |
| Storage | [`plugin-storage-localfs`](https://github.com/Opoha/plugin-storage-localfs), [`plugin-storage-s3`](https://github.com/Opoha/plugin-storage-s3) |
| Search | [`plugin-search-meilisearch`](https://github.com/Opoha/plugin-search-meilisearch) |
| Commerce | [`plugin-tax-standard`](https://github.com/Opoha/plugin-tax-standard), [`plugin-coupon`](https://github.com/Opoha/plugin-coupon), [`plugin-discount`](https://github.com/Opoha/plugin-discount), [`plugin-rma`](https://github.com/Opoha/plugin-rma), [`plugin-mail-smtp`](https://github.com/Opoha/plugin-mail-smtp) |
| Growth | [`plugin-cms`](https://github.com/Opoha/plugin-cms), [`plugin-product-review`](https://github.com/Opoha/plugin-product-review), [`plugin-wishlist`](https://github.com/Opoha/plugin-wishlist), [`plugin-marketplace`](https://github.com/Opoha/plugin-marketplace), [`plugin-pos`](https://github.com/Opoha/plugin-pos), [`plugin-subscription`](https://github.com/Opoha/plugin-subscription), [`plugin-workflow`](https://github.com/Opoha/plugin-workflow) |

Author plugins against [opoha-plugin-sdk](https://github.com/Opoha/opoha-plugin-sdk). Start from [plugin-sample](https://github.com/Opoha/plugin-sample).

## Principles

1. Core never depends on `@opoha/plugin-*`
2. Variable / provider behavior lives in plugins
3. Admin and SDK talk GraphQL only
4. Developers customize without modifying core source

---

Built for platform engineers, plugin authors, and teams who need commerce that fits their domain — not the other way around.
