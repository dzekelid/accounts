---
swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 1
info:
  title: Coinbase API
  description: the-coinbase-v2-api
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
    post:
      summary: Create account
      description: Creates a new account for user.
      operationId: creates-a-new-account-for-user
      x-api-path-slug: accounts-post
      parameters:
      - in: body
        name: account_properties
        description: Account properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Account
  /accounts/{account_id}:
    get:
      summary: Show an account
      description: "Show current user\u2019s account. To access user\u2019s primary
        account, primary keyword can be used instead of the account id in the URL."
      operationId: show-current-users-account-to-access-users-primary-account-primary-keyword-can-be-used-instead-of-th
      x-api-path-slug: accountsaccount-id-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Show
      - Account
    put:
      summary: Update account
      description: "Modifies user\u2019s account name."
      operationId: modifies-users-account-name
      x-api-path-slug: accountsaccount-id-put
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: body
        name: account_properties
        description: Properties to update
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Account
    delete:
      summary: Delete account
      description: "Removes user\u2019s account. In order to remove an account it
        can\u2019t be\n\n- Primary account\n- Account with non-zero balance\n- Fiat
        account\n- Vault with a pending withdrawal"
      operationId: removes-users-account-in-order-to-remove-an-account-it-cant-be-primary-account-account-with-nonzero-
      x-api-path-slug: accountsaccount-id-delete
      parameters:
      - in: path
        name: account_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Account
  /accounts/{account_id}/primary:
    get:
      summary: Set account as primary
      description: Promote an account as primary account.
      operationId: promote-an-account-as-primary-account
      x-api-path-slug: accountsaccount-idprimary-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Set
      - Account
      - As
      - Primary
---