---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Deposit into bank account
  description: Deposit crypto currency into the bank.  In sandbox mode, the account
    used is the demo account on the blockchain server.
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /basicfns/GetAccountBalance:
    post:
      summary: Get user's account balance (*)
      description: Get information about an user's account balance.  The call is restricted
        to the unlocked user's account / query only. <br/>* In this sandbox, you can
        query any user's account balance for testing purposes.  All accounts are test
        accounts and no actual value or account is exposed in the sandbox.
      operationId: BasicfnsGetAccountBalancePost
      x-api-path-slug: basicfnsgetaccountbalance-post
      parameters:
      - in: formData
        name: accountId
      - in: header
        name: ApiKey
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Users
      - Account
      - Balance
      - (*)
  /ethbank/withdraw:
    post:
      summary: Withdraw from bank account
      description: Withdraw crypto currency into the bank.  In sandbox mode, the account
        used is the demo account on the blockchain server. Of course, you can only
        withdraw if there is money in the account!
      operationId: EthbankWithdrawPost
      x-api-path-slug: ethbankwithdraw-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: value
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Withdraw
      - From
      - Bank
      - Account
  /ethbank/deposit:
    post:
      summary: Deposit into bank account
      description: Deposit crypto currency into the bank.  In sandbox mode, the account
        used is the demo account on the blockchain server.
      operationId: EthbankDepositPost
      x-api-path-slug: ethbankdeposit-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: value
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Deposit
      - Into
      - Bank
      - Account
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