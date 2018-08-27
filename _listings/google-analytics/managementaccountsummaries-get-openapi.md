---
swagger: "2.0"
x-collection-name: Google Analytics
x-complete: 0
info:
  title: Google Analytics Get Account Summary
  description: Lists account summaries (lightweight tree comprised of accounts/properties/profiles)
    to which the user has access.
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /analytics/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /management/accounts:
    get:
      summary: Get Accounts
      description: Lists all accounts to which the user has access.
      operationId: analytics.management.accounts.list
      x-api-path-slug: managementaccounts-get
      parameters:
      - in: query
        name: max-results
        description: The maximum number of accounts to include in this response
      - in: query
        name: start-index
        description: An index of the first account to retrieve
      responses:
        200:
          description: OK
      tags:
      - Account
  /management/accountSummaries:
    get:
      summary: Get Account Summary
      description: Lists account summaries (lightweight tree comprised of accounts/properties/profiles)
        to which the user has access.
      operationId: analytics.management.accountSummaries.list
      x-api-path-slug: managementaccountsummaries-get
      parameters:
      - in: query
        name: max-results
        description: The maximum number of account summaries to include in this response,
          where the largest acceptable value is 1000
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      responses:
        200:
          description: OK
      tags:
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