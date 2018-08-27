---
swagger: "2.0"
x-collection-name: Google Tag Manager
x-complete: 0
info:
  title: Google Tag Manager API Get Account
  description: Gets a GTM Account.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tagmanager/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}:
    put:
      summary: Update Account
      description: Updates a GTM Account.
      operationId: tagmanager.accounts.update
      x-api-path-slug: accountsaccountid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the account in storage
      responses:
        200:
          description: OK
      tags:
      - Account
    get:
      summary: Get Account
      description: Gets a GTM Account.
      operationId: tagmanager.accounts.get
      x-api-path-slug: accountsaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
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