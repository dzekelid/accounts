swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
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
    put:
      summary: Put Accounts
      description: |-
        You can update an account using the following parameters.
        Use this method to set the accounts payment method, credit card token (when applicable), bill to contact and custom fields.
      operationId: putV1AccountsAccount
      x-api-path-slug: v1accountsaccount-id-put
      parameters:
      - in: body
        name: body
        description: Body Parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Accounts