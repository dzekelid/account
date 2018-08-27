---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Delete Account Attribute
  description: Remove attribute from an account. Attribute name is used as a quary
    parameter. For this API request account/owner, system/admin or system/manager
    role is required
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