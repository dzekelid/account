---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Get Account Memberships
  description: ID of a user should be specified as a query parameter. JSON with membership
    details is returned. For this API call system/admin or system/manager role is
    required
  version: 1.0.0
host: /account
basePath: https://codenvy.com/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/{id}/resources:
    post:
      summary: Post Account Resources
      description: 'Redistributes resources between workspaces. Roles: account/owner,
        system/manager, system/admin.'
      operationId: redistributeResources
      x-api-path-slug: accountidresources-post
      parameters:
      - in: body
        name: body
        description: Resources description
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Resources
    get:
      summary: Get Account Resources
      description: 'Returns used resources, provided by subscriptions. Roles: account/owner,
        account/member, system/manager, system/admin.'
      operationId: getResources
      x-api-path-slug: accountidresources-get
      parameters:
      - in: path
        name: id
        description: Account ID
      - in: query
        name: serviceId
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Resources
  /account/{id}/members/{userid}:
    delete:
      summary: Delete Account Members User
      description: Remove user from a specific account. This API call requires account/owner,
        system/admin or system/manager role.
      operationId: removeMember
      x-api-path-slug: accountidmembersuserid-delete
      parameters:
      - in: path
        name: id
        description: Account ID
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Members
      - Userid
  /account/{id}/members:
    post:
      summary: Post Account Members
      description: Add a new user to an account. This user will have account/member
        role. This API call requires account/owner, system/admin or system/manager
        role.
      operationId: addMember
      x-api-path-slug: accountidmembers-post
      parameters:
      - in: body
        name: body
        description: New membership
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Members
    get:
      summary: Get Account Members
      description: Get all members for a specific account. This API call requires
        account/owner, system/admin or system/manager role.
      operationId: getMembers
      x-api-path-slug: accountidmembers-get
      parameters:
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Members
  /account/{id}/attribute:
    delete:
      summary: Delete Account Attribute
      description: Remove attribute from an account. Attribute name is used as a quary
        parameter. For this API request account/owner, system/admin or system/manager
        role is required
      operationId: removeAttribute
      x-api-path-slug: accountidattribute-delete
      parameters:
      - in: path
        name: id
        description: Account ID
      - in: query
        name: name
        description: Attribute name to be removed
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Attribute
  /account/{id}:
    post:
      summary: Post Account
      description: Update account. This API call requires account/owner role.
      operationId: update
      x-api-path-slug: accountid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
    get:
      summary: Get Account
      description: Get account information by its ID. JSON with account details is
        returned. This API call requires account/owner, system/admin or system/manager
        role.
      operationId: getById
      x-api-path-slug: accountid-get
      parameters:
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
    delete:
      summary: Delete Account
      description: Remove subscription from account. JSON with subscription details
        is sent. Can be performed only by system/admin.
      operationId: remove
      x-api-path-slug: accountid-delete
      parameters:
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
  /account/{accountId}/subscriptions:
    get:
      summary: Get Account Accountid Subscriptions
      description: Get information on account subscriptions. This API call requires
        account/owner, account/member, system/admin or system/manager role.
      operationId: getSubscriptions
      x-api-path-slug: accountaccountidsubscriptions-get
      parameters:
      - in: path
        name: accountId
        description: Account ID
      - in: query
        name: service
        description: Service ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - AccountId
      - Subscriptions
  /account/subscriptions/{subscriptionId}:
    get:
      summary: Get Account Subscriptions Subscriptionid
      description: Get information on a particular subscription by its unique ID.
      operationId: getSubscriptionById
      x-api-path-slug: accountsubscriptionssubscriptionid-get
      parameters:
      - in: path
        name: subscriptionId
        description: Subscription ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Subscriptions
      - SubscriptionId
    delete:
      summary: Delete Account Subscriptions Subscriptionid
      description: 'Remove subscription from account. Roles: account/owner, system/admin.'
      operationId: removeSubscription
      x-api-path-slug: accountsubscriptionssubscriptionid-delete
      parameters:
      - in: path
        name: subscriptionId
        description: Subscription ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Subscriptions
      - SubscriptionId
  /account/subscriptions:
    post:
      summary: Post Account Subscriptions
      description: 'Add a new subscription to an account. JSON with subscription details
        is sent. Roles: account/owner, system/admin.'
      operationId: addSubscription
      x-api-path-slug: accountsubscriptions-post
      parameters:
      - in: body
        name: body
        description: Subscription details
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Subscriptions
  /account/memberships:
    get:
      summary: Get Account Memberships
      description: ID of a user should be specified as a query parameter. JSON with
        membership details is returned. For this API call system/admin or system/manager
        role is required
      operationId: getMembershipsOfSpecificUser
      x-api-path-slug: accountmemberships-get
      parameters:
      - in: query
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Memberships
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