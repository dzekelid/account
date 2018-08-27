---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API Account Plan Delete
  description: Account plan delete.
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