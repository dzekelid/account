---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Create a PayPal account with predefined ID
  description: ""
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /payment-cards-migrations/migrate:
    post:
      summary: Migrate payment cards to another gateway account
      description: Migrate payment cards to another gateway account
      operationId: migrate-payment-cards-to-another-gateway-account
      x-api-path-slug: paymentcardsmigrationsmigrate-post
      parameters:
      - in: body
        name: body
        description: Payment card migration attributes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Migrate
      - Payment
      - Cards
      - To
      - Another
      - Gateway
      - Account
  /gateway-accounts/{id}:
    put:
      summary: Create or update a Gateway Account with predefined ID
      description: Create or update a GatewayAccount with predefined identifier string
      operationId: create-or-update-a-gatewayaccount-with-predefined-identifier-string
      x-api-path-slug: gatewayaccountsid-put
      parameters:
      - in: body
        name: body
        description: Gateway Account resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Gateway
      - Account
      - Predefined
      - ID
    patch:
      summary: Update a Gateway Account with predefined ID
      description: Update a GatewayAccount with predefined identifier string
      operationId: update-a-gatewayaccount-with-predefined-identifier-string
      x-api-path-slug: gatewayaccountsid-patch
      parameters:
      - in: body
        name: body
        description: Gateway Account resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gateway
      - Account
      - Predefined
      - ID
    get:
      summary: Retrieve a Gateway Account
      description: Retrieve a Gateway Account with specified identifier string
      operationId: retrieve-a-gateway-account-with-specified-identifier-string
      x-api-path-slug: gatewayaccountsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Gateway
      - Account
    delete:
      summary: Delete a Gateway Account
      description: Delete a Gateway Account with predefined identifier string
      operationId: delete-a-gateway-account-with-predefined-identifier-string
      x-api-path-slug: gatewayaccountsid-delete
      responses:
        200:
          description: OK
      tags:
      - Gateway
      - Account
  /gateway-accounts:
    post:
      summary: Create a Gateway Account
      description: Create a Gateway Account
      operationId: create-a-gateway-account
      x-api-path-slug: gatewayaccounts-post
      parameters:
      - in: body
        name: body
        description: Gateway Account resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gateway
      - Account
  /activation/{token}:
    post:
      summary: Sends a token to activate user account
      description: Sends a token to activate user account
      operationId: sends-a-token-to-activate-user-account
      x-api-path-slug: activationtoken-post
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Token
      - To
      - Activate
      - User
      - Account
  /paypal-accounts/{id}/deactivation:
    post:
      summary: Deactivate a PayPal Account
      description: Deactivate a PayPal Account
      operationId: paypal_accounts.id.deactivation.post
      x-api-path-slug: paypalaccountsiddeactivation-post
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - PayPal
      - Account
  /paypal-accounts/{id}/activation:
    post:
      summary: Activate a PayPal Account
      description: Activate a PayPal Account
      operationId: paypal_accounts.id.activation.post
      x-api-path-slug: paypalaccountsidactivation-post
      parameters:
      - in: body
        name: body
        description: PayPal Account resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Activate
      - PayPal
      - Account
  /paypal-accounts/{id}:
    put:
      summary: Create a PayPal account with predefined ID
      description: ""
      operationId: paypal_accounts.id.put
      x-api-path-slug: paypalaccountsid-put
      parameters:
      - in: body
        name: body
        description: PayPal Account
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - PayPal
      - Account
      - Predefined
      - ID
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