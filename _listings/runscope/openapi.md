swagger: "2.0"
x-collection-name: Runscope
x-complete: 1
info:
  title: Runscope
  description: manage-runscope-programmatically-
  version: 1.0.0
host: api.runscope.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    get:
      summary: Get Account
      description: Account Resource
      operationId: account.get
      x-api-path-slug: account-get
      responses:
        200:
          description: OK
      tags:
      - Account