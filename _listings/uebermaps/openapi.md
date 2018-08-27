swagger: "2.0"
x-collection-name: uebermaps
x-complete: 1
info:
  title: uebermaps
  description: enable-people-to-store-spots-on-public-and-private-maps
  termsOfService: https://uebermaps.com/terms/
  contact:
    name: uebermaps API Team
  version: "2.0"
host: uebermaps.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    patch:
      summary: Update account
      description: Update account. Wrap map parameters in [user].
      operationId: account.patch
      x-api-path-slug: account-patch
      parameters:
      - in: body
        name: user
        description: user attributes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Account