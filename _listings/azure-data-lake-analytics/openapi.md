swagger: "2.0"
x-collection-name: Azure Data Lake Analytics
x-complete: 1
info:
  title: DataLakeAnalyticsJobManagementClient
  description: creates-an-azure-data-lake-analytics-job-client-
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
    delete:
      summary: Account Delete
      description: Begins the delete delete process for the Data Lake Analytics account
        object specified by the account name.
      operationId: Account_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountname-delete
      parameters:
      - in: path
        name: accountName
        description: The name of the Data Lake Analytics account to delete
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Analytics account
      responses:
        200:
          description: OK
      tags:
      - Account
    get:
      summary: Account Get
      description: Gets details of the specified Data Lake Analytics account.
      operationId: Account_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountname-get
      parameters:
      - in: path
        name: accountName
        description: The name of the Data Lake Analytics account to retrieve
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Analytics account
      responses:
        200:
          description: OK
      tags:
      - Account
  /subscriptions/{subscriptionId}/providers/Microsoft.DataLakeAnalytics/accounts:
    get:
      summary: Account List
      description: Gets the first page of Data Lake Analytics accounts, if any, within
        the current subscription. This includes a link to the next page, if any.
      operationId: Account_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-datalakeanalyticsaccounts-get
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