swagger: "2.0"
x-collection-name: Google Cloud Billing
x-complete: 1
info:
  title: Google Cloud Billing
  description: allows-developers-to-manage-billing-for-their-google-cloud-platform-projects----programmatically-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: cloudbilling.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:
    get:
      summary: Get Billing Account
      description: |-
        Gets information about a billing account. The current authenticated user
        must be an [owner of the billing
        account](https://support.google.com/cloud/answer/4430947).
      operationId: cloudbilling.billingAccounts.get
      x-api-path-slug: v1name-get
      parameters:
      - in: path
        name: name
        description: The resource name of the billing account to retrieve
      responses:
        200:
          description: OK
      tags:
      - Account
  /v1/billingAccounts:
    get:
      summary: Get Billing Accounts
      description: |-
        Lists the billing accounts that the current authenticated user
        [owns](https://support.google.com/cloud/answer/4430947).
      operationId: cloudbilling.billingAccounts.list
      x-api-path-slug: v1billingaccounts-get
      parameters:
      - in: query
        name: pageSize
        description: Requested page size
      - in: query
        name: pageToken
        description: A token identifying a page of results to return
      responses:
        200:
          description: OK
      tags:
      - Account