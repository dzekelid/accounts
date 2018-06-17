---
swagger: "2.0"
x-collection-name: Azure Logic Apps
x-complete: 0
info:
  title: Azure Logic Apps API Sessions List By Integration Accounts
  description: Gets a list of integration account sessions.
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
    patch:
      summary: Integration Accounts Update
      description: Updates an integration account.
      operationId: IntegrationAccounts_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountname-patch
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
    delete:
      summary: Integration Accounts Delete
      description: Deletes an integration account.
      operationId: IntegrationAccounts_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountname-delete
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/listCallbackUrl
  : post:
      summary: Integration Accounts Get Callback Url
      description: Gets the integration account callback URL.
      operationId: IntegrationAccounts_GetCallbackUrl
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamelistcallbackurl-post
      parameters:
      - in: path
        name: integrationAccountName
        description: The integration account name
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The callback URL parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Integration Accounts Callback Url
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/schemas
  : get:
      summary: Schemas List By Integration Accounts
      description: Gets a list of integration account schemas.
      operationId: Schemas_ListByIntegrationAccounts
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnameschemas-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
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
      - Schemas Integration Accounts
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/maps
  : get:
      summary: Maps List By Integration Accounts
      description: Gets a list of integration account maps.
      operationId: Maps_ListByIntegrationAccounts
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamemaps-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
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
      - Maps Integration Accounts
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/partners
  : get:
      summary: Partners List By Integration Accounts
      description: Gets a list of integration account partners.
      operationId: Partners_ListByIntegrationAccounts
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamepartners-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
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
      - Partners Integration Accounts
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/agreements
  : get:
      summary: Agreements List By Integration Accounts
      description: Gets a list of integration account agreements.
      operationId: Agreements_ListByIntegrationAccounts
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnameagreements-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
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
      - Agreements Integration Accounts
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/certificates
  : get:
      summary: Certificates List By Integration Accounts
      description: Gets a list of integration account certificates.
      operationId: Certificates_ListByIntegrationAccounts
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamecertificates-get
      parameters:
      - in: query
        name: $top
        description: The number of items to be included in the result
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
      - Certificates Integration Accounts
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/sessions
  : get:
      summary: Sessions List By Integration Accounts
      description: Gets a list of integration account sessions.
      operationId: Sessions_ListByIntegrationAccounts
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamesessions-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
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
      - Sessions Integration Accounts
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