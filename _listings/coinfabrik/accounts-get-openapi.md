---
swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 0
info:
  title: CoinFabrik List accounts
  description: "Lists current user\u2019s accounts to which the authentication method
    has access to."
  contact:
    name: CoinFabrik
    url: http://www.coinfabrik.com/
  version: 1.0.0
host: api.coinbase.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts:
    get:
      summary: List accounts
      description: "Lists current user\u2019s accounts to which the authentication
        method has access to."
      operationId: lists-current-users-accounts-to-which-the-authentication-method-has-access-to
      x-api-path-slug: accounts-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
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