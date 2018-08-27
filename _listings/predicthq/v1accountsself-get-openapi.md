---
swagger: "2.0"
x-collection-name: PredictHQ
x-complete: 0
info:
  title: PredictHQ Retrieve Account Details
  description: If you need your account details for whatever reason, it's really easy
    to get them.
  version: 1.0.0
host: api.predicthq.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/accounts/self/:
    get:
      summary: Retrieve Account Details
      description: If you need your account details for whatever reason, it's really
        easy to get them.
      operationId: V1AccountsSelfGet
      x-api-path-slug: v1accountsself-get
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Self
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