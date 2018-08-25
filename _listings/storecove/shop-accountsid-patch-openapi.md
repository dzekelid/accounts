---
swagger: "2.0"
x-collection-name: Storecove
x-complete: 0
info:
  title: Storecove Update ShopAccount
  description: |-
    Update a specific ShopAccount.
    include::examples/shop_accounts/update_shop_account/tabs.adoc[]
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
    post:
      summary: Create ShopAccount
      description: |-
        Create a new ShopAccount.
        include::examples/shop_accounts/create_shop_account/tabs.adoc[]
      operationId: create_shop_account
      x-api-path-slug: shop-accounts-post
      parameters:
      - in: body
        name: shop_account
        description: ShopAccount to add
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Accounts
  /shop_accounts/auth_failures:
    get:
      summary: Get ShopAccounts with authorization failures
      description: |-
        Get ShopAccounts with authorization failures.
        include::examples/shop_accounts/shop_accounts_auth_failures/tabs.adoc[]
      operationId: shop_accounts_auth_failures
      x-api-path-slug: shop-accountsauth-failures-get
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Accounts
      - Auth
      - Failures
  /shop_accounts/{id}:
    delete:
      summary: Delete ShopAccount
      description: |-
        Delete a specific ShopAccount.
        include::examples/shop_accounts/delete_shop_account/tabs.adoc[]
      operationId: delete_shop_account
      x-api-path-slug: shop-accountsid-delete
      parameters:
      - in: path
        name: id
        description: shop_account id
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Accounts
    get:
      summary: Get ShopAccount
      description: |-
        Get a specific ShopAccount.
        include::examples/shop_accounts/get_shop_account/tabs.adoc[]
      operationId: get_shop_account
      x-api-path-slug: shop-accountsid-get
      parameters:
      - in: path
        name: id
        description: shop_account id
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Accounts
    patch:
      summary: Update ShopAccount
      description: |-
        Update a specific ShopAccount.
        include::examples/shop_accounts/update_shop_account/tabs.adoc[]
      operationId: update_shop_account
      x-api-path-slug: shop-accountsid-patch
      parameters:
      - in: path
        name: id
        description: shop_account id
      - in: body
        name: shop_account
        description: ShopAccount updates
        schema:
          $ref: '#/definitions/holder'
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