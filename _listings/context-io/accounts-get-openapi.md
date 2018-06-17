---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Get Accounts
  description: Lists accounts.
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts:
    get:
      summary: Get Accounts
      description: Lists accounts.
      operationId: listAccounts_
      x-api-path-slug: accounts-get
      parameters:
      - in: query
        name: email
        description: Only return account associated to this email address
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      - in: query
        name: status
        description: Only return accounts with sources whose status is of a specific
          value
      - in: query
        name: status_ok
        description: Set to 0 to get all accounts with sources that are not working
          correctly
      - in: query
        name: token
        description: The unique random token used for the graphical account creation
          process
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