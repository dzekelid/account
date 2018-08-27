---
swagger: "2.0"
x-collection-name: Intuit
x-complete: 0
info:
  title: QuickBooks Online V3 API Get Reports Account List
  description: |-
    Report - Account list detail
    Method : GET

    The information below provides a reference on how to access the account list detail report from the QuickBooks Online Report Service.
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