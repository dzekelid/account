---
swagger: "2.0"
x-collection-name: Google Adsense
x-complete: 0
info:
  title: Google Adsense API Get Accounts
  version: 1.0.0
  description: List hosted accounts associated with this AdSense account by ad client
    id.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}:
    get:
      summary: Get Account
      description: Get information about the selected associated AdSense account.
      operationId: adsensehost.accounts.get
      x-api-path-slug: accountsaccountid-get
      parameters:
      - in: path
        name: accountId
        description: Account to get information about
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
  /accounts:
    get:
      summary: Get Accounts
      description: List hosted accounts associated with this AdSense account by ad
        client id.
      operationId: adsensehost.accounts.list
      x-api-path-slug: accounts-get
      parameters:
      - in: query
        name: filterAdClientId
        description: Ad clients to list accounts for
      responses:
        200:
          description: OK
      tags:
      - Advertising
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