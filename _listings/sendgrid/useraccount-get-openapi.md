---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get User Account
  description: |-
    **This endpoint allows you to retrieve your user account details.**

    Your user's account information includes the user's account type and reputation.

    Keeping your user profile up to date is important. This will help SendGrid to verify who you are as well as contact you should we need to.

    For more information about your user profile:

    * [SendGrid Account Settings](https://sendgrid.com/docs/User_Guide/Settings/account.html)
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/account:
    get:
      summary: Get User Account
      description: |-
        **This endpoint allows you to retrieve your user account details.**

        Your user's account information includes the user's account type and reputation.

        Keeping your user profile up to date is important. This will help SendGrid to verify who you are as well as contact you should we need to.

        For more information about your user profile:

        * [SendGrid Account Settings](https://sendgrid.com/docs/User_Guide/Settings/account.html)
      operationId: user.account.get
      x-api-path-slug: useraccount-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - User
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