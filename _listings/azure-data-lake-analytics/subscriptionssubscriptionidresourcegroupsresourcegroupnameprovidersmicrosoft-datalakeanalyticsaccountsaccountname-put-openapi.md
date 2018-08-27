---
swagger: "2.0"
x-collection-name: Azure Data Lake Analytics
x-complete: 0
info:
  title: Azure Data Lake Analytics API Account Create
  description: Creates the specified Data Lake Analytics account. This supplies the
    user with computation services for Data Lake Analytics workloads
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataLakeAnalytics/accounts/{accountName}:
    patch:
      summary: Account Update
      description: Updates the Data Lake Analytics account object specified by the
        accountName with the contents of the account object.
      operationId: Account_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountname-patch
      parameters:
      - in: path
        name: accountName
        description: The name of the Data Lake Analytics account to update
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to the update Data Lake Analytics account
          operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Analytics account
      responses:
        200:
          description: OK
      tags:
      - Account
    put:
      summary: Account Create
      description: Creates the specified Data Lake Analytics account. This supplies
        the user with computation services for Data Lake Analytics workloads
      operationId: Account_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountname-put
      parameters:
      - in: path
        name: accountName
        description: The name of the Data Lake Analytics account to create
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to the create Data Lake Analytics account
          operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Analytics account
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