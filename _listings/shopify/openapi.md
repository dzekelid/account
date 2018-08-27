swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/shop.json:
    get:
      summary: Get the configuration of the shop account
      description: Get the configuration of the shop account.
      operationId: getAdminShop.json
      x-api-path-slug: adminshop-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Configuration
      - Shop
      - Account