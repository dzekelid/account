---
swagger: "2.0"
x-collection-name: Intuit
x-complete: 0
info:
  title: QuickBooks Online V3 API Get Account
  description: Get the Account which has accountId as 1
  version: 1.0.0
host: DefaultParameterValue
basePath: /v3/company/DefaultParameterValue
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/AccountList:
    get:
      summary: Get Reports Account List
      description: |-
        Report - Account list detail
        Method : GET

        The information below provides a reference on how to access the account list detail report from the QuickBooks Online Report Service.
      operationId: getReportsAccountlist
      x-api-path-slug: reportsaccountlist-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Account
      - List
  /account:
    post:
      summary: Post Account
      description: Create a new Account
      operationId: postAccount
      x-api-path-slug: account-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Account
  /account/1:
    get:
      summary: Get Account
      description: Get the Account which has accountId as 1
      operationId: getAccount1
      x-api-path-slug: account1-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Account
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