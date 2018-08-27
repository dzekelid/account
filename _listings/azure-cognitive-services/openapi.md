swagger: "2.0"
x-collection-name: Azure Cognitive Services
x-complete: 1
info:
  title: CognitiveServicesManagementClient
  description: cognitive-services-management-client
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