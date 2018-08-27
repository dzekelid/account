swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 1
info:
  title: ""
  version: 1.0.0
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
  /accounts:
    post:
      summary: Create new account
      description: Creates a new account (standalone user). This is available only
        upon request.
      operationId: creates-a-new-account-standalone-user-this-is-available-only-upon-request
      x-api-path-slug: accounts-post
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
        name: name
        description: The username associated with the account
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
      responses:
        200:
          description: OK
      tags:
      - New
      - Account