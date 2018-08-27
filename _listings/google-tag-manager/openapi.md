swagger: "2.0"
x-collection-name: Google Tag Manager
x-complete: 1
info:
  title: Tag Manager
  description: accesses-tag-manager-accounts-and-containers-
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
  /accounts:
    get:
      summary: Get Accounts
      description: Lists all GTM Accounts that a user has access to.
      operationId: tagmanager.accounts.list
      x-api-path-slug: accounts-get
      responses:
        200:
          description: OK
      tags:
      - Account