---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get list of accounts with sorting and searching and by type of group
    for the accounts
  version: 1.0.0
  description: Get list of accounts with sorting and searching and by type of group
    for the accounts.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/account/all:
    get:
      summary: Get all accounts paginated
      description: Get all accounts paginated.
      operationId: Account_GetAllBypageSizeBypageNumber
      x-api-path-slug: apiaccountall-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Paginated
  /api/account/setstatus:
    post:
      summary: Set an accounts status
      description: Set an accounts status.
      operationId: Account_SetStatusBydataContract
      x-api-path-slug: apiaccountsetstatus-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Accounts
      - Status
  /api/account/systemaccounts:
    get:
      summary: Get list of all system accounts
      description: Get list of all system accounts.
      operationId: Account_GetSystemAccounts
      x-api-path-slug: apiaccountsystemaccounts-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - System
      - Accounts
  /api/account/pm/list:
    post:
      summary: Get list of accounts with sorting and searching and by type of group
        for the accounts
      description: Get list of accounts with sorting and searching and by type of
        group for the accounts.
      operationId: Account_GetPMAccountsBydataContractBypageSizeBypageNumber
      x-api-path-slug: apiaccountpmlist-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Accounts
      - Sorting
      - Searching
      - By
      - Type
      - Of
      - Groupthe
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