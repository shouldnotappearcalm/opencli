# coupang

Total commands: **2**

## Commands


### add-to-cart
- Description: Add a Coupang product to cart using logged-in browser session
- Args:
  - `product-id` (optional) — Coupang product ID
  - `url` (optional) — Canonical product URL
- Example: `opencli coupang add-to-cart -f json`

### search
- Description: Search Coupang products with logged-in browser session
- Args:
  - `query` (required) — Search keyword
  - `page` (optional) — type=int; default=1; Search result page number
  - `limit` (optional) — type=int; default=20; Max results (max 50)
  - `filter` (optional) — Optional search filter (currently supports: rocket)
- Example: `opencli coupang search -f json`
