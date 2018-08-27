swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/account:
    get:
      summary: Find account details
      description: Searches for the user account details. Details include name, email,
        and basic account permissions
      operationId: getAccount
      x-api-path-slug: meaccount-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Account