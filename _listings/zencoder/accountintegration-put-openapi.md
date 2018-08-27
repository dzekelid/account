---
swagger: "2.0"
x-collection-name: Zencoder
x-complete: 0
info:
  title: Zencoder API Integration Mode
  version: v2
  description: Integration Mode
host: app.zencoder.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/live:
    put:
      summary: Integration Mode - Live
      description: Integration Mode - Live
      operationId: putAccountLive
      x-api-path-slug: accountlive-put
      responses:
        200:
          description: OK
      tags:
      - Account
      - Live
  /account/integration:
    put:
      summary: Integration Mode
      description: Integration Mode
      operationId: putAccountIntegration
      x-api-path-slug: accountintegration-put
      parameters:
      - in: query
        name: api_key
        description: The API key
      responses:
        200:
          description: OK
      tags:
      - Account
      - Integration
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