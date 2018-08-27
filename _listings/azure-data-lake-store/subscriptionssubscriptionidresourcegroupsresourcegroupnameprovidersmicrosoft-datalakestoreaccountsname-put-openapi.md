---
swagger: "2.0"
x-collection-name: Azure Data Lake Store
x-complete: 0
info:
  title: Azure Data Lake Store API Account Create
  description: Creates the specified Data Lake Store account.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/Microsoft.DataLakeStore/accounts:
    get:
      summary: Account List
      description: Lists the Data Lake Store accounts within the subscription. The
        response includes a link to the next page of results, if any.
      operationId: Account_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-datalakestoreaccounts-get
      parameters:
      - in: query
        name: $count
        description: The Boolean value of true or false to request a count of the
          matching resources included with the resources in the response, e
      - in: query
        name: $filter
        description: OData filter
      - in: query
        name: $orderby
        description: OrderBy clause
      - in: query
        name: $select
        description: OData Select statement
      - in: query
        name: $skip
        description: The number of items to skip over before returning elements
      - in: query
        name: $top
        description: The number of items to return
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Account
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataLakeStore/accounts:
    get:
      summary: Account List By Resource Group
      description: Lists the Data Lake Store accounts within a specific resource group.
        The response includes a link to the next page of results, if any.
      operationId: Account_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakestoreaccounts-get
      parameters:
      - in: query
        name: $count
        description: A Boolean value of true or false to request a count of the matching
          resources included with the resources in the response, e
      - in: query
        name: $filter
        description: OData filter
      - in: query
        name: $orderby
        description: OrderBy clause
      - in: query
        name: $select
        description: OData Select statement
      - in: query
        name: $skip
        description: The number of items to skip over before returning elements
      - in: query
        name: $top
        description: The number of items to return
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Store account(s)
      responses:
        200:
          description: OK
      tags:
      - Account
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataLakeStore/accounts/{accountName}/enableKeyVault
  : post:
      summary: Account Enable Key Vault
      description: Attempts to enable a user managed key vault for encryption of the
        specified Data Lake Store account.
      operationId: Account_EnableKeyVault
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakestoreaccountsaccountnameenablekeyvault-post
      parameters:
      - in: path
        name: accountName
        description: The name of the Data Lake Store account to attempt to enable
          the Key Vault for
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Store account
      responses:
        200:
          description: OK
      tags:
      - Account
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataLakeStore/accounts/{name}:
    get:
      summary: Account Get
      description: Gets the specified Data Lake Store account.
      operationId: Account_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakestoreaccountsname-get
      parameters:
      - in: path
        name: name
        description: The name of the Data Lake Store account to retrieve
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Store account
      responses:
        200:
          description: OK
      tags:
      - Account
    delete:
      summary: Account Delete
      description: Deletes the specified Data Lake Store account.
      operationId: Account_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakestoreaccountsname-delete
      parameters:
      - in: path
        name: name
        description: The name of the Data Lake Store account to delete
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Store account
      responses:
        200:
          description: OK
      tags:
      - Account
    patch:
      summary: Account Update
      description: Updates the specified Data Lake Store account information.
      operationId: Account_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakestoreaccountsname-patch
      parameters:
      - in: path
        name: name
        description: The name of the Data Lake Store account to update
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to update the Data Lake Store account
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Store account
      responses:
        200:
          description: OK
      tags:
      - Account
    put:
      summary: Account Create
      description: Creates the specified Data Lake Store account.
      operationId: Account_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakestoreaccountsname-put
      parameters:
      - in: path
        name: name
        description: The name of the Data Lake Store account to create
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to create the Data Lake Store account
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Store account
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