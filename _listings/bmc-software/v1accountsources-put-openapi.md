---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 0
info:
  title: BMC Software API Set source metadata
  version: 1.0.0
  description: Sets one or more source metadata
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/account/sources:
    put:
      summary: Set source metadata
      description: Sets one or more source metadata
      operationId: set-source-metadata
      x-api-path-slug: v1accountsources-put
      responses:
        200:
          description: OK
      tags:
      - Account
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