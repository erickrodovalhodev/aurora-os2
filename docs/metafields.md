# Metafields and metaobjects

| Namespace | Key | Type | Used by |
| --- | --- | --- | --- |
| `custom` | `size_guide` | metaobject reference | `sections/main-product.liquid` |
| `custom` | `care_notes` | multi-line text | `sections/main-product.liquid` |
| `reviews` | `rating` | number_decimal | `snippets/rating.liquid` |

`size_guide` is a metaobject definition with `title` and `body`. One entry per
category; the PDP renders the entry referenced by the product, and falls back
to nothing when the metafield is empty.
