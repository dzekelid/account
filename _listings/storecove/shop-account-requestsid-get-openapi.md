---
swagger: "2.0"
x-collection-name: Storecove
x-complete: 0
info:
  title: Storecove Get ShopAccountRequest
  description: |-
    Show a specific ShopAccountRequest
    include::examples/shop_account_requests/get_shop_account_request/tabs.adoc[]
  version: 2.0.1
host: api.storecove.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shop_account_requests/{id}:
    patch:
      summary: Update ShopAccountRequest
      description: |-
        Update a specific ShopAccountRequest
        include::examples/shop_account_requests/update_shop_account_request/tabs.adoc[]
      operationId: update_shop_account_request
      x-api-path-slug: shop-account-requestsid-patch
      parameters:
      - in: path
        name: id
        description: shop_account_request id
      - in: body
        name: shop_account_request
        description: ShopAccountRequest updates
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Account
      - Requests
    get:
      summary: Get ShopAccountRequest
      description: |-
        Show a specific ShopAccountRequest
        include::examples/shop_account_requests/get_shop_account_request/tabs.adoc[]
      operationId: get_shop_account_request
      x-api-path-slug: shop-account-requestsid-get
      parameters:
      - in: path
        name: id
        description: shop_account_request id
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Account
      - Requests
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---