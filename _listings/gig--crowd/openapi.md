swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
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
  /api/v1/gigme/account/user:
    post:
      summary: Post Gigme Account User
      description: Post gigme account user.
      operationId: postApiV1GigmeAccountUser
      x-api-path-slug: apiv1gigmeaccountuser-post
      parameters:
      - in: header
        name: Authorization
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
      - User
    get:
      summary: Get Gigme Account User
      description: Get gigme account user.
      operationId: getApiV1GigmeAccountUser
      x-api-path-slug: apiv1gigmeaccountuser-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Account
      - User
  /api/v1/account/external/link/{provider}:
    get:
      summary: Get Account External Link Prover
      description: Get account external link prover.
      operationId: getApiV1AccountExternalLinkProver
      x-api-path-slug: apiv1accountexternallinkprovider-get
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: code
      - in: path
        name: provider
      - in: query
        name: redirectUri
      responses:
        200:
          description: OK
      tags:
      - Account
      - External
      - Link
      - Prover
  /api/v1/account/external/register/{userSocialId}:
    post:
      summary: Post Account External Register Usersocialid
      description: Post account external register usersocialid.
      operationId: postApiV1AccountExternalRegisterUsersocial
      x-api-path-slug: apiv1accountexternalregisterusersocialid-post
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
      - Account
      - External
      - Register
      - Usersocialid
  /api/v1/account/culture:
    post:
      summary: Post Account Culture
      description: Post account culture.
      operationId: postApiV1AccountCulture
      x-api-path-slug: apiv1accountculture-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: culture
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Culture
  /api/v1/account/devicetoken:
    post:
      summary: Post Account Devicetoken
      description: Post account devicetoken.
      operationId: postApiV1AccountDevicetoken
      x-api-path-slug: apiv1accountdevicetoken-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Devicetoken
  /api/v1/account/avatar:
    post:
      summary: Post Account Avatar
      description: Post account avatar.
      operationId: postApiV1AccountAvatar
      x-api-path-slug: apiv1accountavatar-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Account
      - Avatar
  /api/v1/account/logout:
    post:
      summary: Post Account Logout
      description: Post account logout.
      operationId: postApiV1AccountLogout
      x-api-path-slug: apiv1accountlogout-post
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Account
      - Logout
  /api/v1/account/register/invite:
    post:
      summary: Post Account Register Invite
      description: Post account register invite.
      operationId: postApiV1AccountRegisterInvite
      x-api-path-slug: apiv1accountregisterinvite-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Register
      - Invite
  /api/v1/account/register/art:
    post:
      summary: Post Account Register Art
      description: Post account register art.
      operationId: postApiV1AccountRegisterArt
      x-api-path-slug: apiv1accountregisterart-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Register
      - Art
  /api/v1/account/register/org:
    post:
      summary: Post Account Register Org
      description: Post account register org.
      operationId: postApiV1AccountRegisterOrg
      x-api-path-slug: apiv1accountregisterorg-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Register
      - Org
  /api/v1/account/user:
    get:
      summary: Get Account User
      description: Get account user.
      operationId: getApiV1AccountUser
      x-api-path-slug: apiv1accountuser-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Account
      - User