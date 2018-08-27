---
swagger: "2.0"
x-collection-name: RipaEx
x-complete: 0
info:
  title: RipaEx Delegates Forging Get Forged By Account
  description: Get the amount of ripas forged by an account.
  version: 1.0.0
host: api.ripaex.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/delegates/forging/getForgedByAccount:
    get:
      summary: Delegates Forging Get Forged By Account
      description: Get the amount of ripas forged by an account.
      operationId: delegates.getForgedByAccount
      x-api-path-slug: apidelegatesforginggetforgedbyaccount-get
      parameters:
      - in: query
        name: generatorPublicKey
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Delegates
      - Forging
      - ""
      - Forged
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