swagger: "2.0"
x-collection-name: Browshot
x-complete: 1
info:
  title: Browshot
  description: take-screenshots-of-any-website-in-real-time
  termsOfService: https://browshot.com/terms
  contact:
    name: API Support
    url: https://browshot.com/contact
    email: support@browshot.com
  version: 1.17.0
host: api.browshot.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/info:
    get:
      summary: Get information about your account
      description: Get information about your account.
      operationId: GetAccountInfo
      x-api-path-slug: accountinfo-get
      parameters:
      - in: query
        name: details
        description: level of information returned
      responses:
        200:
          description: OK
      tags:
      - Account
      - Info