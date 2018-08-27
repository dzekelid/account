---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Get API Account Exist
  version: 1.0.0
  description: Get api account exist.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/MarginTrading/account/reset/{accountId}:
    delete:
      summary: Delete API Margintrading Account Reset Account
      description: Delete api margintrading account reset account.
      operationId: ApiMarginTradingAccountResetByAccountIdDelete
      x-api-path-slug: apimargintradingaccountresetaccountid-delete
      parameters:
      - in: path
        name: accountId
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Margintrading
      - Account
      - Reset
      - Account
  /api/MarginTrading/account/balance:
    post:
      summary: Add API Margintrading Account Balance
      description: Add api margintrading account balance.
      operationId: ApiMarginTradingAccountBalancePost
      x-api-path-slug: apimargintradingaccountbalance-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Margintrading
      - Account
      - Balance
  /api/AccountExist:
    get:
      summary: Get API Account Exist
      description: Get api account exist.
      operationId: ApiAccountExistGet
      x-api-path-slug: apiaccountexist-get
      parameters:
      - in: query
        name: email
      - in: query
        name: partnerId
      responses:
        200:
          description: OK
      tags:
      - Account
      - Exist
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