---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Post Account Resources
  description: 'Redistributes resources between workspaces. Roles: account/owner,
    system/manager, system/admin.'
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