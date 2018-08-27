swagger: "2.0"
x-collection-name: PredictHQ
x-complete: 1
info:
  title: PredictHQ API
  description: todo-add-description
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