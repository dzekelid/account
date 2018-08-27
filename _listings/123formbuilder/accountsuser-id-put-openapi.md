---
swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 0
info:
  title: 123FormBuilder Update account
  version: 1.0.0
  description: Updates an account. You can only update the users that you have created
    using your account token.
host: api.123contactform.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{user_id}:
    put:
      summary: Update account
      description: Updates an account. You can only update the users that you have
        created using your account token.
      operationId: updates-an-account-you-can-only-update-the-users-that-you-have-created-using-your-account-token
      x-api-path-slug: accountsuser-id-put
      parameters:
      - in: formData
        name: company_name
        description: The company name associated with the account
      - in: formData
        name: email
        description: The email address associated with the account
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: password
        description: The password associated with the account
      - in: formData
        name: password_repeat
        description: Password repeat
      - in: formData
        name: plan
        description: 'The service plan of the account: 0 - Free (default value), 1
          - Gold, 2 - Platinum, 3 - Diamond'
      - in: path
        name: user_id
        description: The ID of the account that you want to update
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