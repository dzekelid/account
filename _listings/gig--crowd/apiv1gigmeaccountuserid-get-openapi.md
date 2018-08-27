---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Gigme Account User
  version: 1.0.0
  description: Get gigme account user.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/gigme/account/external/register/{userSocialId}:
    post:
      summary: Post Gigme Account External Register Usersocialid
      description: Post gigme account external register usersocialid.
      operationId: postApiV1GigmeAccountExternalRegisterUsersocial
      x-api-path-slug: apiv1gigmeaccountexternalregisterusersocialid-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userSocialId
        description: id UserSocial
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Account
      - External
      - Register
      - Usersocialid
  /api/v1/gigme/account/register:
    post:
      summary: Post Gigme Account Register
      description: Post gigme account register.
      operationId: postApiV1GigmeAccountRegister
      x-api-path-slug: apiv1gigmeaccountregister-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Account
      - Register
  /api/v1/gigme/account/user/{id}:
    get:
      summary: Get Gigme Account User
      description: Get gigme account user.
      operationId: getApiV1GigmeAccountUser
      x-api-path-slug: apiv1gigmeaccountuserid-get
      parameters:
      - in: query
        name: hash
      - in: path
        name: id
      - in: query
        name: timestamp
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Account
      - User
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