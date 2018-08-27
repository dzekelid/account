---
swagger: "2.0"
x-collection-name: Quovo
x-complete: 0
info:
  title: Quovo Delete a manual account
  description: Deletes a Manual Account.
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{account_id}:
    put:
      summary: Update an account
      description: Modifies an existing account.
      operationId: AccountsByAccountIdPut
      x-api-path-slug: accountsaccount-id-put
      parameters:
      - in: path
        name: account_id
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Account
    get:
      summary: Get a single account
      description: Provides information on a single account.
      operationId: AccountsByAccountIdGet
      x-api-path-slug: accountsaccount-id-get
      parameters:
      - in: path
        name: account_id
      responses:
        200:
          description: OK
      tags:
      - Single
      - Account
  /accounts/{account_id}/auth:
    get:
      summary: Get auth for an account
      description: Retrieves all authentication information associated with an account.
      operationId: AccountsAuthByAccountIdGet2
      x-api-path-slug: accountsaccount-idauth-get
      parameters:
      - in: path
        name: account_id
      responses:
        200:
          description: OK
      tags:
      - Authan
      - Account
  /users/{user_id}/manual_accounts:
    post:
      summary: Create a manual account
      description: Creates a Manual Account.
      operationId: UsersManualAccountsByUserIdPost
      x-api-path-slug: usersuser-idmanual-accounts-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Manual
      - Account
  /manual_accounts/{manual_account_id}:
    delete:
      summary: Delete a manual account
      description: Deletes a Manual Account.
      operationId: ManualAccountsByManualAccountIdDelete
      x-api-path-slug: manual-accountsmanual-account-id-delete
      parameters:
      - in: path
        name: manual_account_id
      responses:
        200:
          description: OK
      tags:
      - Manual
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