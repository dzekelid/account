swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /audit/authentication/accounts/{account_id}:
    get:
      summary: Query by account.
      description: Query by account..
      operationId: query-by-account
      x-api-path-slug: auditauthenticationaccountsaccount-id-get
      parameters:
      - in: query
        name: end_time
        description: The end of the time range from which you want events
      - in: query
        name: start_time
        description: The beginning of the time range from which you want events
      responses:
        200:
          description: OK
      tags:
      - Audit
      - Authentication
      - Accounts
      - Account
      - Id
  /users/{id}/merge_into/accounts/destination_account_id/users/{destination_user_id}:
    put:
      summary: Merge user into another user
      description: Merge user into another user.
      operationId: merge-user-into-another-user
      x-api-path-slug: usersidmerge-intoaccountsdestination-account-idusersdestination-user-id-put
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
      - Merge
      - Into
      - Accounts
      - Destination
      - Account
      - Id
      - Users
      - Destination
      - User
      - Id
  /api/sis/accounts/{account_id}/assignments:
    get:
      summary: Retrieve assignments enabled for grade export to SIS
      description: Retrieve assignments enabled for grade export to sis.
      operationId: retrieve-assignments-enabled-for-grade-export-to-sis
      x-api-path-slug: apisisaccountsaccount-idassignments-get
      parameters:
      - in: query
        name: account_id
        description: The ID of the account to query
      - in: query
        name: course_id
        description: The ID of the course to query
      - in: query
        name: ends_after
        description: When searching on an account, restricts to courses that end after
          this daten(if they have an end date)
      - in: query
        name: starts_before
        description: When searching on an account, restricts to courses that start
          before thisndate (if they have a start date)
      responses:
        200:
          description: OK
      tags:
      - Api
      - Sis
      - Accounts
      - Account
      - Id
      - Assignments