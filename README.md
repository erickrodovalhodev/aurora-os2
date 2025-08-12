# Aurora OS 2.0

Shopify theme on Online Store 2.0 — JSON templates, sections with blocks,
metafields and metaobjects. Rebuild of the 2020 `aurora` theme for the 2.0
layout.

## install

    shopify theme dev --store sua-loja
    shopify theme push --unpublished

## what it covers

- `templates/*.json` with `sections/*.liquid` and schema blocks
- PDP price read from the variant, so PDP and checkout never drift
- size guide as a metaobject, one entry shared by every PDP
- cart drawer with focus trap
- section-level settings for copy, no hardcoded text

## decisions

- no jQuery, no external bundle
- price formatting only through the `money` filter
- every section validates against `shopify theme check`

## limits

Headless was not the goal here; `storefront-next` is where that lives.
