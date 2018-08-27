---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Nurego Get Accounts
  description: You can retrieve a specific account by using the account number.
  contact:
    name: support@nurego.com
  version: 1.0.0
host: api.nurego.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/accounts/{predix-zone-id}:
    post:
      summary: Create an EC system account
      description: Create a EC system account with the CF details
      operationId: create-a-ec-system-account-with-the-cf-details
      x-api-path-slug: adminaccountspredixzoneid-post
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: path
        name: predix-zone-id
        description: Cloud Foundry service instance details
      - in: body
        name: settings
        description: Cloud Foundry setting details
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - EC
      - System
      - Account
    get:
      summary: Get the EC system account
      description: Get an existing EC system account by predix zone id
      operationId: get-an-existing-ec-system-account-by-predix-zone-id
      x-api-path-slug: adminaccountspredixzoneid-get
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: path
        name: predix-zone-id
        description: pass the predix zone id
      responses:
        200:
          description: Successful response
      tags:
      - EC
      - System
      - Account
    delete:
      summary: Delete the EC system account
      description: Delete an existing EC system account by predix zone id
      operationId: delete-an-existing-ec-system-account-by-predix-zone-id
      x-api-path-slug: adminaccountspredixzoneid-delete
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: path
        name: predix-zone-id
        description: pass the predix zone id
      responses:
        200:
          description: Successful response
      tags:
      - EC
      - System
      - Account
    put:
      summary: Update the EC gateway setting in the account
      description: Update the EC gateway setting in the account with the CF details
      operationId: update-the-ec-gateway-setting-in-the-account-with-the-cf-details
      x-api-path-slug: adminaccountspredixzoneid-put
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: path
        name: predix-zone-id
        description: Predix Zone Id
      - in: body
        name: settings
        description: Cloud Foundry setting destails
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - EC
      - Gateway
      - Setting
      - In
      - Account
  /v1/accounts/{account_id}:
    parameters:
      summary: Parameters Accounts
      description: Parameters accounts.
      operationId: parametersV1AccountsAccount
      x-api-path-slug: v1accountsaccount-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Accounts
    get:
      summary: Get Accounts
      description: You can retrieve a specific account by using the account number.
      operationId: getV1AccountsAccount
      x-api-path-slug: v1accountsaccount-id-get
      responses:
        200:
          description: OK
      tags:
      - Accounts
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