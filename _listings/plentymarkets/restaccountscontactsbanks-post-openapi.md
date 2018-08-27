---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Create a bank account
  description: Create a bank account.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
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
  /rest/payments/methods/ebics:
    post:
      summary: Create an EBICS Account
      description: Create an ebics account.
      operationId: postRestPaymentsMethodsEbics
      x-api-path-slug: restpaymentsmethodsebics-post
      parameters:
      - in: query
        name: name
        description: The name of the EBICS Account
      responses:
        200:
          description: OK
      tags:
      - EBICS
      - Account
  /rest/items/sales_prices/{id}/accounts/{accountType}/{accountId}:
    delete:
      summary: Deactivate a referrer account
      description: Deactivates a referrer account for a sales price.
      operationId: deleteRestItemsSalesPricesAccountsAccounttypeAccount
      x-api-path-slug: restitemssales-pricesidaccountsaccounttypeaccountid-delete
      parameters:
      - in: path
        name: accountId
      - in: path
        name: accountType
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Referrer
      - Account
  /rest/items/sales_prices/{id}/accounts:
    post:
      summary: Activate a referrer account
      description: Activates a referrer account for a sales price.
      operationId: postRestItemsSalesPricesAccounts
      x-api-path-slug: restitemssales-pricesidaccounts-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/accounts
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Referrer
      - Account
  /rest/accounts/{accountId}:
    put:
      summary: Update an account
      description: Updates an account. The ID of the account must be specified.
      operationId: putRestAccountsAccount
      x-api-path-slug: restaccountsaccountid-put
      parameters:
      - in: body
        name: /rest/accounts/{accountId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: accountId
      responses:
        200:
          description: OK
      tags:
      - Account
    get:
      summary: Get an account
      description: Gets an account. The ID of the account must be specified.
      operationId: getRestAccountsAccount
      x-api-path-slug: restaccountsaccountid-get
      parameters:
      - in: path
        name: accountId
      responses:
        200:
          description: OK
      tags:
      - Account
    delete:
      summary: Delete an account
      description: Deletes an account. The ID of the account must be specified.
      operationId: deleteRestAccountsAccount
      x-api-path-slug: restaccountsaccountid-delete
      parameters:
      - in: path
        name: accountId
      responses:
        200:
          description: OK
      tags:
      - Account
  /rest/accounts/contacts/{contactId}/accounts/{accountId}:
    put:
      summary: Update an account
      description: Updates an account. The ID of the contact and the ID of the account
        must be specified.
      operationId: putRestAccountsContactsContactAccountsAccount
      x-api-path-slug: restaccountscontactscontactidaccountsaccountid-put
      parameters:
      - in: path
        name: accountId
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Account
    get:
      summary: Get an account of the contact
      description: Gets an account of the contact. The ID of the contact and the ID
        of the account must be specified.
      operationId: getRestAccountsContactsContactAccountsAccount
      x-api-path-slug: restaccountscontactscontactidaccountsaccountid-get
      parameters:
      - in: path
        name: accountId
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Account
      - Of
      - Contact
    delete:
      summary: Delete an account of the contact
      description: Deletes an account of the contact. The ID of the contact and the
        ID of the account must be specified.
      operationId: deleteRestAccountsContactsContactAccountsAccount
      x-api-path-slug: restaccountscontactscontactidaccountsaccountid-delete
      parameters:
      - in: path
        name: accountId
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Account
      - Of
      - Contact
  /rest/accounts/contacts/banks/{contactBankId}:
    put:
      summary: Update a bank account
      description: Updates a bank account. The ID of the bank account must be specified.
      operationId: putRestAccountsContactsBanksContactbank
      x-api-path-slug: restaccountscontactsbankscontactbankid-put
      parameters:
      - in: body
        name: /rest/accounts/contacts/banks/{contactBankId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contactBankId
      responses:
        200:
          description: OK
      tags:
      - Bank
      - Account
    get:
      summary: Get a bank account
      description: Gets a bank account of the contact. The ID of the bank account
        must be specified.
      operationId: getRestAccountsContactsBanksContactbank
      x-api-path-slug: restaccountscontactsbankscontactbankid-get
      parameters:
      - in: path
        name: contactBankId
      responses:
        200:
          description: OK
      tags:
      - Bank
      - Account
    delete:
      summary: Delete a bank account
      description: Deletes a bank account. The ID of the bank account must be specified.
      operationId: deleteRestAccountsContactsBanksContactbank
      x-api-path-slug: restaccountscontactsbankscontactbankid-delete
      parameters:
      - in: path
        name: contactBankId
      responses:
        200:
          description: OK
      tags:
      - Bank
      - Account
  /rest/accounts/contacts/banks:
    post:
      summary: Create a bank account
      description: Create a bank account.
      operationId: postRestAccountsContactsBanks
      x-api-path-slug: restaccountscontactsbanks-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/banks
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bank
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