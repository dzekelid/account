swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /my/account:
    put:
      summary: Put My Account
      description: Update account details
      operationId: putMyAccount
      x-api-path-slug: myaccount-put
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - My
      - Account
    get:
      summary: Get My Account
      description: Get account details
      operationId: getMyAccount
      x-api-path-slug: myaccount-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Account