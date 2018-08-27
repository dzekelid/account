---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Makes payment to supplied account.
  version: 1.0.0
  description: Makes payment to supplied account..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/transfer/unsuspend:
    post:
      summary: Move funds from suspense account to another ledger
      description: Move funds from suspense account to another ledger.
      operationId: Transfer_ProcessUnsuspendFundsBysuspendDataContract
      x-api-path-slug: apitransferunsuspend-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: suspendDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Move
      - Funds
      - From
      - Suspense
      - Account
      - To
      - Another
      - Ledger
  /api/transfer/suspend:
    post:
      summary: Move funds to suspense account to another ledger
      description: Move funds to suspense account to another ledger.
      operationId: Transfer_ProcessSuspendFundsBysuspendDataContract
      x-api-path-slug: apitransfersuspend-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: suspendDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Move
      - Funds
      - To
      - Suspense
      - Account
      - To
      - Another
      - Ledger
  /api/tax/pay/hmrc:
    post:
      summary: Pay tax out of tax held account
      description: Pay tax out of tax held account.
      operationId: Tax_PayTaxHmrcBypayTaxDataContract
      x-api-path-slug: apitaxpayhmrc-post
      parameters:
      - in: body
        name: payTaxDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Tax
      - Out
      - Of
      - Tax
      - Held
      - Account
  /api/reconcile/account/{id}/statements:
    get:
      summary: Get reconcile statements for bank account
      description: Get reconcile statements for bank account.
      operationId: Reconcile_GetStatementsByid
      x-api-path-slug: apireconcileaccountidstatements-get
      parameters:
      - in: path
        name: id
        description: Bank Account Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Reconcile
      - Statementsbank
      - Account
  /api/receipt/fundsshortfall:
    post:
      summary: Records funds from office account into client account and then to client
        if necessary.
      description: Records funds from office account into client account and then
        to client if necessary..
      operationId: Receipt_ReceiptFundsShortfallBydataContract
      x-api-path-slug: apireceiptfundsshortfall-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Funds
      - From
      - Office
      - Account
      - Into
      - Client
      - Account
      - Then
      - To
      - Client
      - If
      - Necessary
  /api/receipt/recordpayment:
    post:
      summary: Makes payment to supplied account.
      description: Makes payment to supplied account..
      operationId: Receipt_RecordPaymentByrecordPaymentDataContract
      x-api-path-slug: apireceiptrecordpayment-post
      parameters:
      - in: body
        name: recordPaymentDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Makes
      - Payment
      - To
      - Supplied
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