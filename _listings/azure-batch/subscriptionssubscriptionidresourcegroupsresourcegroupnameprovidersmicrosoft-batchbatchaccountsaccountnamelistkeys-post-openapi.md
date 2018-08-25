---
swagger: "2.0"
x-collection-name: Azure Batch
x-complete: 0
info:
  title: Azure Batch API Gets the account keys for the specified Batch account.
  version: 1.0.0
  description: This operation applies only to Batch accounts created with a poolAllocationMode
    of 'BatchService'. If the Batch account was created with a poolAllocationMode
    of 'UserSubscription', clients cannot use access to keys to authenticate, and
    must use Azure Active Directory instead. In this case, getting the keys will fail.
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