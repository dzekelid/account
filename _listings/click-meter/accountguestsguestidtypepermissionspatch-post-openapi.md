---
swagger: "2.0"
x-collection-name: Click Meter
x-complete: 0
info:
  title: Click Meter Change the permission on a shared object
  description: Change the permission on a shared object.
  contact:
    name: Api Support
    url: http://www.clickmeter.com/api
    email: api@clickmeter.com
  version: v2
host: apiv2.clickmeter.com:80
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/plan:
    get:
      summary: Retrieve current account plan
      description: Retrieve current account plan.
      operationId: getAccountPlan
      x-api-path-slug: accountplan-get
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
  /account/ipblacklist/{blacklistId}:
    delete:
      summary: Delete an ip blacklist entry
      description: Delete an ip blacklist entry.
      operationId: deleteAccountIpblacklistBlacklist
      x-api-path-slug: accountipblacklistblacklistid-delete
      parameters:
      - in: path
        name: blacklistId
        description: The id of the ip to delete
      responses:
        200:
          description: OK
      tags:
      - Account
      - Ipblacklist
      - BlacklistId
  /account/ipblacklist:
    post:
      summary: Create an ip blacklist entry
      description: Create an ip blacklist entry.
      operationId: postAccountIpblacklist
      x-api-path-slug: accountipblacklist-post
      parameters:
      - in: body
        name: value
        description: The entry to add
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Ipblacklist
    get:
      summary: Retrieve list of a ip to exclude from event tracking
      description: Retrieve list of a ip to exclude from event tracking.
      operationId: getAccountIpblacklist
      x-api-path-slug: accountipblacklist-get
      parameters:
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      responses:
        200:
          description: OK
      tags:
      - Account
      - Ipblacklist
  /account/guests/{guestId}/{type}/permissions/patch:
    put:
      summary: Change the permission on a shared object
      description: Change the permission on a shared object.
      operationId: putAccountGuestsGuestTypePermissionsPatch
      x-api-path-slug: accountguestsguestidtypepermissionspatch-put
      parameters:
      - in: body
        name: body
        description: The patch permission request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: guestId
        description: Id of the guest
      - in: path
        name: type
        description: Can be datapoint or group
      responses:
        200:
          description: OK
      tags:
      - Account
      - Guests
      - GuestId
      - Type
      - Permissions
      - Patch
    post:
      summary: Change the permission on a shared object
      description: Change the permission on a shared object.
      operationId: postAccountGuestsGuestTypePermissionsPatch
      x-api-path-slug: accountguestsguestidtypepermissionspatch-post
      parameters:
      - in: body
        name: body
        description: The patch permission request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: guestId
        description: Id of the guest
      - in: path
        name: type
        description: Can be datapoint or group
      responses:
        200:
          description: OK
      tags:
      - Account
      - Guests
      - GuestId
      - Type
      - Permissions
      - Patch
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