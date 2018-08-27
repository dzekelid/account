---
swagger: "2.0"
x-collection-name: Vzaar
x-complete: 0
info:
  title: Vzaar API Get Api Accounts Account
  description: 'nnThis API call returns the details and rights for each vzaar subscription
    account type along with its relevant metadata. This will show the details of the
    packages available here: http://vzaar.com/pricingnn'
  termsOfService: http://vzaar.com/policies
  version: v1
host: vzaar.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accounts/{account}.{format}:
    get:
      summary: Get Api Accounts Account
      description: 'nnThis API call returns the details and rights for each vzaar
        subscription account type along with its relevant metadata. This will show
        the details of the packages available here: http://vzaar.com/pricingnn'
      operationId: getApiAccountsAccount.Format
      x-api-path-slug: apiaccountsaccount-format-get
      parameters:
      - in: query
        name: account is the vzaar account type. This is an integer.
      responses:
        "":
          description: ""
        400:
          description: Bad input parameter
        401:
          description: Bad or expired token
        403:
          description: Bad OAuth request (wrong consumer key, bad nonce, expired timestamp
        404:
          description: File or folder not found at the specified path
        405:
          description: Request method not expected (generally should be GET or POST)
        429:
          description: Your app is making too many requests and is being rate limited
        503:
          description: If the response includes the Retry-After header, this means
            your OAuth 1
        507:
          description: User is over Dropbox storage quota
        5xx:
          description: Server error
        200:
          description: OK
      tags:
      - Api
      - Accounts
      - Account
      - Format
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