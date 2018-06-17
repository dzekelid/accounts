---
swagger: "2.0"
x-collection-name: Azure Logic Apps
x-complete: 0
info:
  title: Azure Logic Apps API Integration Accounts Create Or Update
  description: Creates or updates an integration account.
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
  /subscriptions/{subscriptionId}/providers/Microsoft.Logic/integrationAccounts:
    get:
      summary: Integration Accounts List By Subscription
      description: Gets a list of integration accounts by subscription.
      operationId: IntegrationAccounts_ListBySubscription
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-logicintegrationaccounts-get
      parameters:
      - in: query
        name: $top
        description: The number of items to be included in the result
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Integration Accounts Subscription
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts:
    get:
      summary: Integration Accounts List By Resource Group
      description: Gets a list of integration accounts by resource group.
      operationId: IntegrationAccounts_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccounts-get
      parameters:
      - in: query
        name: $top
        description: The number of items to be included in the result
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Integration Accounts Resource Group
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}
  : get:
      summary: Integration Accounts Get
      description: Gets an integration account.
      operationId: IntegrationAccounts_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountname-get
      parameters:
      - in: path
        name: integrationAccountName
        description: The integration account name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Integration Accounts
    put:
      summary: Integration Accounts Create Or Update
      description: Creates or updates an integration account.
      operationId: IntegrationAccounts_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountname-put
      parameters:
      - in: body
        name: integrationAccount
        description: The integration account
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: integrationAccountName
        description: The integration account name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Integration Accounts
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