swagger: "2.0"
x-collection-name: Rebilly
x-complete: 1
info:
  title: Rebilly
  description: -introductionthe-rebilly-api-is-built-on-http---our-api-is-restful---it-has-predictableresource-urls---it-returns-http-response-codes-to-indicate-errors---it-alsoaccepts-and-returns-json-in-the-http-body---you-can-use-your-favoritehttprest-library-for-your-programming-language-to-use-rebillys-api-oryou-can-use-one-of-our-sdks-currently-available-in-phphttpsgithub-comrebillyrebillyphpand-chttpsgithub-comrebillyrebillydotnetclient--authenticationwhen-you-sign-up-for-an-account-you-are-given-your-first-api-key-you-can-generate-additional-api-keys-and-delete-api-keys-as-you-mayneed-to-rotate-your-keys-in-the-future--you-authenticate-to-therebilly-api-by-providing-your-secret-key-in-the-request-header-rebilly-offers-three-forms-of-authentication--private-key-json-web-tokens-andpublic-key--private-key-authenticates-each-request-by-searching-for-the-presenceof-an-http-header-rebapikey--jwt-authenticates-each-request-by-the-http-header-authorization--public-key-authenticates-by-the-http-header-rebauth-read-more-on-this-below-rebilly-also-offers-json-web-tokens-jwt-authentication-where-you-can-controlthe-specific-granular-permissions-and-expiration-for-that-jwt---we-call-our-resourcefor-generating-jwt-sessionstagsessions-rebilly-also-has-a-clientside-authentication-scheme-that-uses-anapiuser-and-hmacsha1-signature-only-for-the-tokens-resource-sothat-you-may-safely-create-tokens-from-the-clientside-without-compromisingyour-secret-keys-never-share-your-secret-keys--keep-them-guarded-and-secure-the-clientside-authentication-scheme-uses-one-http-header-named-rebauth--redocinject-securitydefinitions--php-sdkfor-all-php-sdk-examples-provided-in-this-spec-you-will-need-to-configure-client-you-may-do-it-like-thisphpclient--new-rebillyclient----apikey--yourapikeyhere----baseurl--httpsapi-rebilly-com
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
    get:
      summary: Retrieve a PayPal Account
      description: Retrieve a PayPal Account with specified identifier string
      operationId: paypal_accounts.id.get
      x-api-path-slug: paypalaccountsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - PayPal
      - Account
  /paypal-accounts:
    post:
      summary: Create a PayPal Account
      description: Create a PayPal Account
      operationId: paypal_accounts.post
      x-api-path-slug: paypalaccounts-post
      parameters:
      - in: body
        name: body
        description: PayPalAccount resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - PayPal
      - Account
  /bank-accounts/{id}/deactivation:
    post:
      summary: Deactivate a Bank Account
      description: Deactivate a Bank Account
      operationId: bank_accounts.id.deactivation.post
      x-api-path-slug: bankaccountsiddeactivation-post
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Bank
      - Account
  /bank-accounts/{id}:
    get:
      summary: Retrieve a Bank Account
      description: Retrieve a Bank Account with specified identifier string
      operationId: bank_accounts.id.get
      x-api-path-slug: bankaccountsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Bank
      - Account
  /bank-accounts:
    post:
      summary: Create a Bank Account
      description: Create a Bank Account
      operationId: bank_accounts.post
      x-api-path-slug: bankaccounts-post
      parameters:
      - in: body
        name: body
        description: BankAccount resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bank
      - Account