---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Billing API Invoice List by Account
  description: Invoice list by account.
  termsOfService: http://www.3scale.net/terms-and-conditions/
  contact:
    name: 3Scale
    url: https://support.3scale.net/
  version: "1"
host: su1.3scale.net
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/api/users/{id}/unsuspend.xml:
    put:
      summary: User Unsuspend (of provider account)
      description: User unsuspend (of provider account).
      operationId: user_provider_account
      x-api-path-slug: adminapiusersidunsuspend-xml-put
      parameters:
      - in: path
        name: id
        description: id of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - User
      - Unsuspend
      - (of
      - Provider
      - Account)
  /admin/api/users/{id}/suspend.xml:
    put:
      summary: User Suspend (provider account)
      description: User suspend (provider account).
      operationId: user_provider_account
      x-api-path-slug: adminapiusersidsuspend-xml-put
      parameters:
      - in: path
        name: id
        description: id of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - User
      - Suspend
      - (provider
      - Account)
  /admin/api/users/{id}/member.xml:
    put:
      summary: User change Role to Member (provider account)
      description: User change role to member (provider account).
      operationId: user_provider_account
      x-api-path-slug: adminapiusersidmember-xml-put
      parameters:
      - in: path
        name: id
        description: id of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - User
      - Change
      - Role
      - To
      - Member
      - (provider
      - Account)
  /admin/api/users/{id}/admin.xml:
    put:
      summary: User change Role to Admin (provider account)
      description: User change role to admin (provider account).
      operationId: user_provider_account
      x-api-path-slug: adminapiusersidadmin-xml-put
      parameters:
      - in: path
        name: id
        description: id of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - User
      - Change
      - Role
      - To
      - Admin
      - (provider
      - Account)
  /admin/api/users/{id}/activate.xml:
    put:
      summary: User Activate (provider account)
      description: User activate (provider account).
      operationId: user_provider_account
      x-api-path-slug: adminapiusersidactivate-xml-put
      parameters:
      - in: path
        name: id
        description: id of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - User
      - Activate
      - (provider
      - Account)
  /admin/api/users/{id}.xml:
    put:
      summary: User Update (provider account)
      description: User update (provider account).
      operationId: user_provider_account
      x-api-path-slug: adminapiusersid-xml-put
      parameters:
      - in: query
        name: additional_fields
        description: Additional fields have to be name and value i
      - in: query
        name: email
        description: Email of the user
      - in: path
        name: id
        description: id of the user
      - in: query
        name: password
        description: Password of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: username
        description: Username of the user
      responses:
        200:
          description: OK
      tags:
      - User
      - ""
      - (provider
      - Account)
    get:
      summary: User Read (provider account)
      description: User read (provider account).
      operationId: user_provider_account
      x-api-path-slug: adminapiusersid-xml-get
      parameters:
      - in: path
        name: id
        description: id of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - User
      - Read
      - (provider
      - Account)
    delete:
      summary: User Delete (provider account)
      description: User delete (provider account).
      operationId: user_provider_account
      x-api-path-slug: adminapiusersid-xml-delete
      parameters:
      - in: path
        name: id
        description: id of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - User
      - ""
      - (provider
      - Account)
  /admin/api/users.xml:
    post:
      summary: User Create (provider account)
      description: User create (provider account).
      operationId: user_provider_account
      x-api-path-slug: adminapiusers-xml-post
      parameters:
      - in: query
        name: additional_fields
        description: Additional fields have to be name and value i
      - in: query
        name: email
        description: Email of the user
      - in: query
        name: password
        description: Password of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: username
        description: Username of the user
      responses:
        200:
          description: OK
      tags:
      - User
      - (provider
      - Account)
    get:
      summary: User List (provider account)
      description: User list (provider account).
      operationId: user_provider_account
      x-api-path-slug: adminapiusers-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: role
        description: Filter users by Role
      - in: query
        name: state
        description: Filter users by State
      responses:
        200:
          description: OK
      tags:
      - User
      - List
      - (provider
      - Account)
  /admin/api/provider.xml:
    get:
      summary: Account Read
      description: Account read.
      operationId: account
      x-api-path-slug: adminapiprovider-xml-get
      responses:
        200:
          description: OK
      tags:
      - Account
      - Read
  /admin/api/features/{id}.xml:
    put:
      summary: Account Feature Update
      description: Account feature update.
      operationId: account_feature
      x-api-path-slug: adminapifeaturesid-xml-put
      parameters:
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: name
        description: Name of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Feature
    get:
      summary: Account Feature Read
      description: Account feature read.
      operationId: account_feature
      x-api-path-slug: adminapifeaturesid-xml-get
      parameters:
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Feature
      - Read
    delete:
      summary: Account Feature Delete
      description: Account feature delete.
      operationId: account_feature
      x-api-path-slug: adminapifeaturesid-xml-delete
      parameters:
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Feature
  /admin/api/features.xml:
    post:
      summary: Account Feature Create
      description: Account feature create.
      operationId: account_feature
      x-api-path-slug: adminapifeatures-xml-post
      parameters:
      - in: query
        name: name
        description: Name of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: system_name
        description: System Name of the object to be created
      responses:
        200:
          description: OK
      tags:
      - Account
      - Feature
      - Create
    get:
      summary: Account Feature List
      description: Account feature list.
      operationId: account_feature
      x-api-path-slug: adminapifeatures-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Feature
      - List
  /admin/api/account_plans/{id}/default.xml:
    put:
      summary: Account Plan set to Default
      description: Account plan set to default.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plansiddefault-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Set
      - To
      - Default
  /admin/api/account_plans/{id}.xml:
    put:
      summary: Account Plan Update
      description: Account plan update.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plansid-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account plan
      - in: query
        name: name
        description: Name of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
    get:
      summary: Account Plan Read
      description: Account plan read.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plansid-xml-get
      parameters:
      - in: path
        name: id
        description: id of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Read
    delete:
      summary: Account Plan Delete
      description: Account plan delete.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plansid-xml-delete
      parameters:
      - in: path
        name: id
        description: id of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
  /admin/api/account_plans/{account_plan_id}/features/{id}.xml:
    post:
      summary: Account Plan Features Create
      description: Account plan features create.
      operationId: account_plan_feature
      x-api-path-slug: adminapiaccount-plansaccount-plan-idfeaturesid-xml-post
      parameters:
      - in: path
        name: account_plan_id
        description: id of the account plan
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Features
      - Create
    delete:
      summary: Account Plan Features Delete
      description: Account plan features delete.
      operationId: account_plan_feature
      x-api-path-slug: adminapiaccount-plansaccount-plan-idfeaturesid-xml-delete
      parameters:
      - in: path
        name: account_plan_id
        description: id of the account plan
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Features
  /admin/api/account_plans/{account_plan_id}/features.xml:
    get:
      summary: Account Plan Feature List
      description: Account plan feature list.
      operationId: account_plan_feature
      x-api-path-slug: adminapiaccount-plansaccount-plan-idfeatures-xml-get
      parameters:
      - in: path
        name: account_plan_id
        description: id of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Feature
      - List
  /admin/api/account_plans.xml:
    post:
      summary: Account Plan Create
      description: Account plan create.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plans-xml-post
      parameters:
      - in: query
        name: name
        description: Name of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: system_name
        description: System Name of the object to be created
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Create
    get:
      summary: Account Plan List
      description: Account plan list.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - List
  /admin/api/accounts/{id}/reject.xml:
    put:
      summary: Account Reject
      description: Account reject.
      operationId: account
      x-api-path-slug: adminapiaccountsidreject-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Reject
  /admin/api/accounts/{id}/make_pending.xml:
    put:
      summary: Account Reset to Pending
      description: Account reset to pending.
      operationId: account
      x-api-path-slug: adminapiaccountsidmake-pending-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Reset
      - To
      - Pending
  /admin/api/accounts/{id}/credit_card.xml:
    put:
      summary: Account Set Credit Card
      description: Account set credit card.
      operationId: account
      x-api-path-slug: adminapiaccountsidcredit-card-xml-put
      parameters:
      - in: query
        name: billing_address_address
        description: Address associated to the credit card
      - in: query
        name: billing_address_city
        description: Billing address city
      - in: query
        name: billing_address_country
        description: Billing address country
      - in: query
        name: billing_address_name
        description: Name of the person/company to bill
      - in: query
        name: billing_address_phone
        description: Billing address phone
      - in: query
        name: billing_address_state
        description: Billing address state
      - in: query
        name: billing_address_zip
        description: Billing address ZIP code
      - in: query
        name: credit_card_authorize_net_payment_profile_token
        description: Authorize
      - in: query
        name: credit_card_expiration_month
        description: Month of expiration of credit card
      - in: query
        name: credit_card_expiration_year
        description: Year of expiration of credit card
      - in: query
        name: credit_card_partial_number
        description: 4 last numbers of the credit card
      - in: query
        name: credit_card_token
        description: The token returned by the payment gateway
      - in: path
        name: id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Set
      - Credit
      - Card
    delete:
      summary: Account Delete Credit Card
      description: Account delete credit card.
      operationId: account
      x-api-path-slug: adminapiaccountsidcredit-card-xml-delete
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - ""
      - Credit
      - Card
  /admin/api/accounts/{id}/change_plan.xml:
    put:
      summary: Account Change Plan
      description: Account change plan.
      operationId: account
      x-api-path-slug: adminapiaccountsidchange-plan-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: plan_id
        description: id of the target account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Change
      - Plan
  /admin/api/accounts/{id}/approve.xml:
    put:
      summary: Account Approve
      description: Account approve.
      operationId: account
      x-api-path-slug: adminapiaccountsidapprove-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Approve
  /admin/api/accounts/{id}.xml:
    put:
      summary: Account Update
      description: Account update.
      operationId: account
      x-api-path-slug: adminapiaccountsid-xml-put
      parameters:
      - in: query
        name: additional_fields
        description: Additional fields have to be name and value i
      - in: path
        name: id
        description: id of the account
      - in: query
        name: org_name
        description: Organization name of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
    get:
      summary: Account Read
      description: Account read.
      operationId: account
      x-api-path-slug: adminapiaccountsid-xml-get
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Read
    delete:
      summary: Account Delete
      description: Account delete .
      operationId: account
      x-api-path-slug: adminapiaccountsid-xml-delete
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
  /admin/api/accounts/{account_id}/plan.xml:
    get:
      summary: Account Fetch Account Plan
      description: Account fetch account plan.
      operationId: account
      x-api-path-slug: adminapiaccountsaccount-idplan-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Fetch
      - Account
      - Plan
  /admin/api/accounts/{account_id}/messages.xml:
    post:
      summary: Account Message
      description: Account message.
      operationId: account
      x-api-path-slug: adminapiaccountsaccount-idmessages-xml-post
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: query
        name: body
        description: Text to send
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Message
  /admin/api/accounts/find.xml:
    get:
      summary: Account Find
      description: Account find.
      operationId: account
      x-api-path-slug: adminapiaccountsfind-xml-get
      parameters:
      - in: query
        name: email
        description: email of the user of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: username
        description: username of the user of the account
      - in: query
        name: user_id
        description: id of the user of the account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Find
  /admin/api/accounts.xml:
    get:
      summary: Account List
      description: Account list.
      operationId: account
      x-api-path-slug: adminapiaccounts-xml-get
      parameters:
      - in: query
        name: page
        description: Page in the paginated list
      - in: query
        name: per_page
        description: Number of results per page
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: state
        description: Account state
      responses:
        200:
          description: OK
      tags:
      - Account
      - List
  /api/accounts/{account_id}/invoices/{id}.xml:
    get:
      summary: Invoice by Account
      description: Invoice by account.
      operationId: finance
      x-api-path-slug: apiaccountsaccount-idinvoicesid-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the invoice
      - in: query
        name: provider_key
        description: Your api key with 3scale
      responses:
        200:
          description: OK
      tags:
      - Invoice
      - By
      - Account
  /api/accounts/{account_id}/invoices.xml:
    get:
      summary: Invoice List by Account
      description: Invoice list by account.
      operationId: finance
      x-api-path-slug: apiaccountsaccount-idinvoices-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: query
        name: month
        description: Filter the invoice by month
      - in: query
        name: page
        description: Page in the paginated list
      - in: query
        name: per_page
        description: Number of results per page
      - in: query
        name: provider_key
        description: Your api key with 3scale
      - in: query
        name: state
        description: Filter the invoice by state
      responses:
        200:
          description: OK
      tags:
      - Invoice
      - List
      - By
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