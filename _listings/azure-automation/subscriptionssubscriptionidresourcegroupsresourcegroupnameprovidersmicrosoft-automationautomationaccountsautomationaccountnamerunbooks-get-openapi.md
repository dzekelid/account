---
swagger: "2.0"
x-collection-name: Azure Automation
x-complete: 0
info:
  title: Azure Automation API Runbook List By Automation Account
  version: 1.0.0
  description: Retrieve a list of runbooks.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/webhooks
  : get:
      summary: Webhook List By Automation Account
      description: Retrieve a list of webhooks.
      operationId: Webhook_ListByAutomationAccount
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamewebhooks-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Webhook
      - List
      - Automation
      - Account
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/variables
  : get:
      summary: Variable List By Automation Account
      description: Retrieve a list of variables.
      operationId: Variable_ListByAutomationAccount
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamevariables-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Variable
      - List
      - Automation
      - Account
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/schedules
  : get:
      summary: Schedule List By Automation Account
      description: Retrieve a list of schedules.
      operationId: Schedule_ListByAutomationAccount
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnameschedules-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Schedule
      - List
      - Automation
      - Account
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/runbooks
  : get:
      summary: Runbook List By Automation Account
      description: Retrieve a list of runbooks.
      operationId: Runbook_ListByAutomationAccount
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamerunbooks-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Runbook
      - List
      - Automation
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