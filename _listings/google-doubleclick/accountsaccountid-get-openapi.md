---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Get Account
  version: 1.0.0
  description: Get information about the selected Ad Exchange account.
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
    get:
      summary: Get Accounts
      description: Retrieves the list of accounts, possibly filtered. This method
        supports paging.
      operationId: dfareporting.accounts.list
      x-api-path-slug: userprofilesprofileidaccounts-get
      parameters:
      - in: query
        name: active
        description: Select only active accounts
      - in: query
        name: ids
        description: Select only accounts with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
  /accounts/{accountId}:
    get:
      summary: Get Account
      description: Get information about the selected Ad Exchange account.
      operationId: adexchangeseller.accounts.get
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