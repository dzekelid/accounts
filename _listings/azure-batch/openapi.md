swagger: "2.0"
x-collection-name: Azure Batch
x-complete: 1
info:
  title: BatchManagement
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/listKeys
  : post:
      summary: Gets the account keys for the specified Batch account.
      description: This operation applies only to Batch accounts created with a poolAllocationMode
        of 'BatchService'. If the Batch account was created with a poolAllocationMode
        of 'UserSubscription', clients cannot use access to keys to authenticate,
        and must use Azure Active Directory instead. In this case, getting the keys
        will fail.
      operationId: BatchAccount_GetKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-batchbatchaccountsaccountnamelistkeys-post
      parameters:
      - in: path
        name: accountName
        description: The name of the account
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group that contains the Batch account
      responses:
        200:
          description: OK
      tags:
      - Account Key