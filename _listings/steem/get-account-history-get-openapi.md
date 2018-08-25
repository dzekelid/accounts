---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem Account history
  description: Account history
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_account_count:
    get:
      summary: number of accounts
      description: Get Number of Accounts from Steem
      operationId: get-number-of-accounts-from-steem
      x-api-path-slug: get-account-count-get
      responses:
        200:
          description: OK
      tags:
      - Number
      - Of
      - Accounts
  /lookup_witness_accounts:
    get:
      summary: lookup_witness_accounts
      description: lookup_witness_accounts regex search
      operationId: lookup-witness-accounts-regex-search
      x-api-path-slug: lookup-witness-accounts-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: lowerBoundName
        description: lowerBoundName
      responses:
        200:
          description: OK
      tags:
      - Lookup
      - Witness
      - Accounts
  /lookup_accounts:
    get:
      summary: lookup_accounts
      description: lookup_accounts regex search
      operationId: lookup-accounts-regex-search
      x-api-path-slug: lookup-accounts-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: lowerBoundName
        description: lowerBoundName
      responses:
        200:
          description: OK
      tags:
      - Lookup
      - Accounts
  /get_witness_by_account:
    get:
      summary: get_witness_by_account
      description: get_witness_by_account
      operationId: get-witness-by-account
      x-api-path-slug: get-witness-by-account-get
      parameters:
      - in: query
        name: accountName
        description: witness account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - Witness
      - By
      - Account
  /get_account_votes:
    get:
      summary: get_account_votes
      description: get_account_votes
      operationId: get-account-votes
      x-api-path-slug: get-account-votes-get
      parameters:
      - in: query
        name: voter
        description: account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - Account
      - Votes
  /get_account_history:
    get:
      summary: Account history
      description: Account history
      operationId: account-history
      x-api-path-slug: get-account-history-get
      parameters:
      - in: query
        name: account
        description: name of account
      - in: query
        name: from
        description: from
      - in: query
        name: limit
        description: limit
      responses:
        200:
          description: OK
      tags:
      - Account
      - History
  /get_accounts:
    get:
      summary: Account
      description: Get Accounts from Steem
      operationId: get-accounts-from-steem
      x-api-path-slug: get-accounts-get
      parameters:
      - in: query
        name: names[]
        description: name of account
      responses:
        200:
          description: OK
      tags:
      - Account
  /lookup_account_names:
    get:
      summary: lookup_account_names
      description: lookup_account_names example of accountNames ["good-karma", "fabien"]
      operationId: lookup-account-names-example-of-accountnames-goodkarma-fabien
      x-api-path-slug: lookup-account-names-get
      parameters:
      - in: query
        name: accountNames
        description: accountNames [good-karma, fabien]
      responses:
        200:
          description: OK
      tags:
      - Lookup
      - Account
      - Names
  /get_account_bandwidth:
    get:
      summary: get_account_bandwidth
      description: get_account_bandwidth
      operationId: get-account-bandwidth
      x-api-path-slug: get-account-bandwidth-get
      parameters:
      - in: query
        name: account
        description: account name
      - in: query
        name: bandwidthType
        description: bandwidthType
      responses:
        200:
          description: OK
      tags:
      - Get
      - Account
      - Bandwidth
  /verify_account_authority:
    get:
      summary: verify_account_authority
      description: verify_account_authority
      operationId: verify-account-authority
      x-api-path-slug: verify-account-authority-get
      parameters:
      - in: query
        name: nameOrId
        description: nameOrId
      - in: query
        name: signers
        description: signers
      responses:
        200:
          description: OK
      tags:
      - Verify
      - Account
      - Authority
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