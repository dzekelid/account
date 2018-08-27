---
swagger: "2.0"
x-collection-name: Google Content API for Shopping
x-complete: 0
info:
  title: Google Content API for Shopping API Update Account
  description: 'Updates a Merchant Center account. This method can only be called
    for accounts to which the managing account has access: either the managing account
    itself or sub-accounts if the managing account is a multi-client account. This
    method supports patch semantics.'
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /content/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{merchantId}/accounttax/{accountId}:
    put:
      summary: Update Account Tax
      description: 'Updates the tax settings of the account. This method can only
        be called for accounts to which the managing account has access: either the
        managing account itself or sub-accounts if the managing account is a multi-client
        account.'
      operationId: content.accounttax.update
      x-api-path-slug: merchantidaccounttaxaccountid-put
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account tax settings
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Tax
    patch:
      summary: Update Account Tax
      description: 'Updates the tax settings of the account. This method can only
        be called for accounts to which the managing account has access: either the
        managing account itself or sub-accounts if the managing account is a multi-client
        account. This method supports patch semantics.'
      operationId: content.accounttax.patch
      x-api-path-slug: merchantidaccounttaxaccountid-patch
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account tax settings
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Tax
    get:
      summary: Get Account Tax
      description: 'Retrieves the tax settings of the account. This method can only
        be called for accounts to which the managing account has access: either the
        managing account itself or sub-accounts if the managing account is a multi-client
        account.'
      operationId: content.accounttax.get
      x-api-path-slug: merchantidaccounttaxaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account tax settings
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Tax
  /{merchantId}/accounttax:
    get:
      summary: Get Account Taxes
      description: Lists the tax settings of the sub-accounts in your Merchant Center
        account. This method can only be called for multi-client accounts.
      operationId: content.accounttax.list
      x-api-path-slug: merchantidaccounttax-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of tax settings to return in the response,
          used for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Account
      - Taxes
  /{merchantId}/accountstatuses/{accountId}:
    get:
      summary: Get Account Status
      description: 'Retrieves the status of a Merchant Center account. This method
        can only be called for accounts to which the managing account has access:
        either the managing account itself or sub-accounts if the managing account
        is a multi-client account.'
      operationId: content.accountstatuses.get
      x-api-path-slug: merchantidaccountstatusesaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The ID of the account
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Status
  /{merchantId}/accountstatuses:
    get:
      summary: Get Account Status
      description: Lists the statuses of the sub-accounts in your Merchant Center
        account. This method can only be called for multi-client accounts.
      operationId: content.accountstatuses.list
      x-api-path-slug: merchantidaccountstatuses-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of account statuses to return in the response,
          used for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Account
      - Status
  /{merchantId}/accountshipping/{accountId}:
    put:
      summary: Updat Account Shipping
      description: 'Updates the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account.'
      operationId: content.accountshipping.update
      x-api-path-slug: merchantidaccountshippingaccountid-put
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account shipping
          settings
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Updat
      - Account
      - Shipping
    patch:
      summary: Updat Account Shipping
      description: 'Updates the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account. This method supports patch semantics.'
      operationId: content.accountshipping.patch
      x-api-path-slug: merchantidaccountshippingaccountid-patch
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account shipping
          settings
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Updat
      - Account
      - Shipping
    get:
      summary: Get Account Shipping
      description: 'Retrieves the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account.'
      operationId: content.accountshipping.get
      x-api-path-slug: merchantidaccountshippingaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account shipping
          settings
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Shipping
  /{merchantId}/accountshipping:
    get:
      summary: Get Account Shipping
      description: Lists the shipping settings of the sub-accounts in your Merchant
        Center account. This method can only be called for multi-client accounts.
      operationId: content.accountshipping.list
      x-api-path-slug: merchantidaccountshipping-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of shipping settings to return in the response,
          used for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Account
      - Shipping
  /{merchantId}/accounts/{accountId}:
    put:
      summary: Update Account
      description: 'Updates a Merchant Center account. This method can only be called
        for accounts to which the managing account has access: either the managing
        account itself or sub-accounts if the managing account is a multi-client account.'
      operationId: content.accounts.update
      x-api-path-slug: merchantidaccountsaccountid-put
      parameters:
      - in: path
        name: accountId
        description: The ID of the account
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
    patch:
      summary: Update Account
      description: 'Updates a Merchant Center account. This method can only be called
        for accounts to which the managing account has access: either the managing
        account itself or sub-accounts if the managing account is a multi-client account.
        This method supports patch semantics.'
      operationId: content.accounts.patch
      x-api-path-slug: merchantidaccountsaccountid-patch
      parameters:
      - in: path
        name: accountId
        description: The ID of the account
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
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