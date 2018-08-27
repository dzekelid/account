---
swagger: "2.0"
x-collection-name: TradeStation
x-complete: 0
info:
  title: TradeStation Get Account Orders
  description: |-
    Returns the Orders for the given accounts sorted descending, most recent order first.

    #### Stateless Connection
    Since the web-API provides a stateless connection, it only supports fetching the current state of Orders. If it is needed to display the intermediate state changes, it should be executed at client level.
  termsOfService: http://elasticbeanstalk-us-east-1-525856068889.s3.amazonaws.com/wp-content/uploads/2014/03/Guidelines_For_Acceptance.pdf
  contact:
    name: TradeStation API Team
    url: https://developer.tradestation.com/webapi
    email: webapi@tradestation.com
  version: 1.0.0
host: api.tradestation.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{account_keys}/orders:
    get:
      summary: Get Account Orders
      description: |-
        Returns the Orders for the given accounts sorted descending, most recent order first.

        #### Stateless Connection
        Since the web-API provides a stateless connection, it only supports fetching the current state of Orders. If it is needed to display the intermediate state changes, it should be executed at client level.
      operationId: getOrdersByAccounts
      x-api-path-slug: accountsaccount-keysorders-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: account_keys
        description: 1 or more Account Keys
      - in: query
        name: pageNum
        description: Conveys the page number to return, given a set of orders and
          a page size
      - in: query
        name: pageSize
        description: Conveys the number of order items to return in the request
      - in: query
        name: since
        description: Start Date from which to pull older orders
      responses:
        200:
          description: Successful response
      tags:
      - Account
      - Orders
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