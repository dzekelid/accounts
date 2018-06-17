---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting Get Accounts
  description: Get accounts account.
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts:
    get:
      summary: Get Accounts
      description: Retrieve the chart of accounts
      operationId: getAccounts
      x-api-path-slug: accounts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Accounts
    post:
      summary: Post Accounts
      description: Post accounts.
      operationId: postAccounts
      x-api-path-slug: accounts-post
      parameters:
      - in: body
        name: Accounts
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Accounts
    put:
      summary: Put Accounts
      description: Put accounts.
      operationId: putAccounts
      x-api-path-slug: accounts-put
      parameters:
      - in: body
        name: Accounts
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Accounts
    x-related-model:
      summary: X-related-model Accounts
      description: X-related-model accounts.
      operationId: x-related-modelAccounts
      x-api-path-slug: accounts-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /Accounts/{AccountID}:
    delete:
      summary: Delete Accounts
      description: Delete accounts account.
      operationId: deleteAccountsAccount
      x-api-path-slug: accountsaccountid-delete
      parameters:
      - in: path
        name: AccountID
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
    get:
      summary: Get Accounts
      description: Get accounts account.
      operationId: getAccountsAccount
      x-api-path-slug: accountsaccountid-get
      parameters:
      - in: path
        name: AccountID
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
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