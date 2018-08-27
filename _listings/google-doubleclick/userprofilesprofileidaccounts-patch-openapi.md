---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Update Account
  version: 1.0.0
  description: Updates an existing account. This method supports patch semantics.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /userprofiles/{profileId}/accounts/{id}:
    get:
      summary: Get Account
      description: Gets one account by ID.
      operationId: dfareporting.accounts.get
      x-api-path-slug: userprofilesprofileidaccountsid-get
      parameters:
      - in: path
        name: id
        description: Account ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
  /userprofiles/{profileId}/accounts:
    put:
      summary: Update Account
      description: Updates an existing account.
      operationId: dfareporting.accounts.update
      x-api-path-slug: userprofilesprofileidaccounts-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
    patch:
      summary: Update Account
      description: Updates an existing account. This method supports patch semantics.
      operationId: dfareporting.accounts.patch
      x-api-path-slug: userprofilesprofileidaccounts-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Account ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
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