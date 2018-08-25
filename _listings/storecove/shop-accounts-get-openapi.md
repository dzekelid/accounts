---
swagger: "2.0"
x-collection-name: Storecove
x-complete: 0
info:
  title: Storecove Get ShopAccounts for an entity
  description: |-
    Retrieve all active ShopAccounts for one of your entities.
    include::examples/shop_accounts/shop_accounts_index/tabs.adoc[]
  version: 2.0.1
host: api.storecove.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shop_accounts:
    get:
      summary: Get ShopAccounts for an entity
      description: |-
        Retrieve all active ShopAccounts for one of your entities.
        include::examples/shop_accounts/shop_accounts_index/tabs.adoc[]
      operationId: shop_accounts_index
      x-api-path-slug: shop-accounts-get
      parameters:
      - in: query
        name: external_user_id
        description: Filter by the external_user_id
      responses:
        200:
          description: OK
      tags:
      - Shop
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