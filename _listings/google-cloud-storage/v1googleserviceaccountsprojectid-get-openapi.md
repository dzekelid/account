---
swagger: "2.0"
x-collection-name: Google Cloud Storage
x-complete: 0
info:
  title: Google Cloud Storage Get Account
  version: 1.0.0
  description: Returns the Google service account that is used by Storage Transfer
    Service to access buckets in the project where transfers run or in other projects.
    Each Google service account is associated with one Google Developers Console project.
    Users should add this service account to the Google Cloud Storage bucket ACLs
    to grant access to Storage Transfer Service. This service account is created and
    owned by Storage Transfer Service and can only be used by Storage Transfer Service.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1:getGoogleServiceAccount:
    get:
      summary: Get Service Account
      description: Returns the Google service account that is used by Storage Transfer
        Service to access buckets in the project where transfers run or in other projects.
        Each Google service account is associated with one Google Developers Console
        project. Users should add this service account to the Google Cloud Storage
        bucket ACLs to grant access to Storage Transfer Service. This service account
        is created and owned by Storage Transfer Service and can only be used by Storage
        Transfer Service.
      operationId: storagetransfer.getGoogleServiceAccount
      x-api-path-slug: v1getgoogleserviceaccount-get
      parameters:
      - in: query
        name: projectId
        description: The ID of the Google Developers Console project that the Google
          service account is associated with
      responses:
        200:
          description: OK
      tags:
      - Account
  /v1/googleServiceAccounts/{projectId}:
    get:
      summary: Get Account
      description: Returns the Google service account that is used by Storage Transfer
        Service to access buckets in the project where transfers run or in other projects.
        Each Google service account is associated with one Google Developers Console
        project. Users should add this service account to the Google Cloud Storage
        bucket ACLs to grant access to Storage Transfer Service. This service account
        is created and owned by Storage Transfer Service and can only be used by Storage
        Transfer Service.
      operationId: storagetransfer.googleServiceAccounts.get
      x-api-path-slug: v1googleserviceaccountsprojectid-get
      parameters:
      - in: path
        name: projectId
        description: The ID of the Google Developers Console project that the Google
          service account is associated with
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