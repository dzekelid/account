swagger: "2.0"
x-collection-name: Google Analytics
x-complete: 1
info:
  title: Google Analytics
  description: views-and-manages-your-google-analytics-data-
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