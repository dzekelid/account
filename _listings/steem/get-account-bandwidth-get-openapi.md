---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem get_account_bandwidth
  description: get_account_bandwidth
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /verify_account_authority:
    get:
      summary: verify_account_authority
      description: verify_account_authority
      operationId: verify-account-authority
      x-api-path-slug: verify-account-authority-get
      parameters:
      - in: query
        name: nameOrId
        description: nameOrId
      - in: query
        name: signers
        description: signers
      responses:
        200:
          description: OK
      tags:
      - Verify
      - Account
      - Authority
  /get_account_bandwidth:
    get:
      summary: get_account_bandwidth
      description: get_account_bandwidth
      operationId: get-account-bandwidth
      x-api-path-slug: get-account-bandwidth-get
      parameters:
      - in: query
        name: account
        description: account name
      - in: query
        name: bandwidthType
        description: bandwidthType
      responses:
        200:
          description: OK
      tags:
      - Get
      - Account
      - Bandwidth
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