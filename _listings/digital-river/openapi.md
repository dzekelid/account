swagger: "2.0"
x-collection-name: Digital River
x-complete: 1
info:
  title: Digital River Shopper API
  description: the-dr-connect-shopper-api-operates-on-a-store-and-products-that-are-set-up-in-global-commerce--
  version: v1
host: store.digitalriver.com
basePath: /store/{mysite}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/shoppers/me/account:
    get:
      summary: Get Shoppers Me Account
      description: Get shoppers me account.
      operationId: getV1ShoppersMeAccount
      x-api-path-slug: v1shoppersmeaccount-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Account