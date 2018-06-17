---
swagger: "2.0"
x-collection-name: Viddler
x-complete: 0
info:
  title: Viddler  API Resellers GetSubaccounts
  description: List all subaccounts under your account. Only applies to reseller accounts.
    Other accounts do not have access to this method.
  termsOfService: http://www.viddler.com/terms-of-use/
  version: v2
host: api.viddler.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  viddler.resellers.getSubaccounts:
    get:
      summary: Resellers GetSubaccounts
      description: List all subaccounts under your account. Only applies to reseller
        accounts. Other accounts do not have access to this method.
      operationId: resellers-getsubaccounts
      x-api-path-slug: viddler-resellers-getsubaccounts-get
      parameters:
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: sessionid
      - in: query
        name: sort
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Resellers
      - GetSubaccounts
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