---
swagger: "2.0"
x-collection-name: Azure Cognitive Services
x-complete: 0
info:
  title: Azure Cognitive Services Accounts List By Resource Group
  description: Returns all the resources of a particular type belonging to a resource
    group
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/Microsoft.CognitiveServices/accounts:
    get:
      summary: Accounts List
      description: Returns all the resources of a particular type belonging to a subscription.
      operationId: Accounts_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-cognitiveservicesaccounts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Account
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.CognitiveServices/accounts:
    get:
      summary: Accounts List By Resource Group
      description: Returns all the resources of a particular type belonging to a resource
        group
      operationId: Accounts_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-cognitiveservicesaccounts-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group within the users subscription
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
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