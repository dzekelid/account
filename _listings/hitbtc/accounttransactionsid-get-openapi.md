---
swagger: "2.0"
x-collection-name: HitBTC
x-complete: 0
info:
  title: HitBTC Get Account Transaction By Id
  description: Get account transaction by id.
  version: 1.0.0
basePath: /api/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/transactions/{id}:
    get:
      summary: Get Account Transaction By Id
      description: Get account transaction by id.
      operationId: getAccountTransactions
      x-api-path-slug: accounttransactionsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Account
      - Transaction
      - By
      - Id
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