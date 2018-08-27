---
swagger: "2.0"
x-collection-name: Capital One DevExchange
x-complete: 0
info:
  title: Capital One DevExchange Get all purchases by account and merchant
  description: Returns the purchases that a merchant is involved in.
  version: 1.0.0
host: api.reimaginebanking.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /merchants/{id}/accounts/{accountId}/purchases:
    get:
      summary: Get all purchases by account and merchant
      description: Returns the purchases that a merchant is involved in.
      operationId: returns-the-purchases-that-a-merchant-is-involved-in
      x-api-path-slug: merchantsidaccountsaccountidpurchases-get
      parameters:
      - in: path
        name: accountId
        description: ID of the account associated with all the purchases
      - in: path
        name: id
        description: ID of the merchant associated with all the purchases
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Merchants
      - ""
      - Accounts
      - Account
      - Purchases
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