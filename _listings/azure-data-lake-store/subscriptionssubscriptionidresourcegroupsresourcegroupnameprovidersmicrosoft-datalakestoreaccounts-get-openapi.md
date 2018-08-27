---
swagger: "2.0"
x-collection-name: Azure Data Lake Store
x-complete: 0
info:
  title: Azure Data Lake Store API Account List By Resource Group
  description: Lists the Data Lake Store accounts within a specific resource group.
    The response includes a link to the next page of results, if any.
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