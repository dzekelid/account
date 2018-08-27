---
swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 0
info:
  title: CoinFabrik Set account as primary
  description: Promote an account as primary account.
  contact:
    name: CoinFabrik
    url: http://www.coinfabrik.com/
  version: 1.0.0
host: api.coinbase.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{account_id}/primary:
    get:
      summary: Set account as primary
      description: Promote an account as primary account.
      operationId: promote-an-account-as-primary-account
      x-api-path-slug: accountsaccount-idprimary-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Set
      - Account
      - As
      - Primary
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