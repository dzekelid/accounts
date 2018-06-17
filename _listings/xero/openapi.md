---
swagger: "2.0"
x-collection-name: Xero
x-complete: 1
info:
  title: Accounting
  description: -introductionthe-xero-accounting-api-is-a-restful-web-service-and-uses-the-oauth-v1-0a-protocol-to-authenticate-3rd-party-applications--the-accounting-api-exposes-accounting-and-related-functions-of-the-main-xero-application-and-can-be-used-for-a-variety-of-purposes-such-as-creating-transactions-like-invoices-and-credit-notes-right-through-to-extracting-accounting-data-via-our-reports-endpoint-
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts:
    get:
      summary: Get Accounts
      description: Retrieve the chart of accounts
      operationId: getAccounts
      x-api-path-slug: accounts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Accounts
    post:
      summary: Post Accounts
      description: Post accounts.
      operationId: postAccounts
      x-api-path-slug: accounts-post
      parameters:
      - in: body
        name: Accounts
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Accounts
    put:
      summary: Put Accounts
      description: Put accounts.
      operationId: putAccounts
      x-api-path-slug: accounts-put
      parameters:
      - in: body
        name: Accounts
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Accounts
    x-related-model:
      summary: X-related-model Accounts
      description: X-related-model accounts.
      operationId: x-related-modelAccounts
      x-api-path-slug: accounts-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /Accounts/{AccountID}:
    delete:
      summary: Delete Accounts
      description: Delete accounts account.
      operationId: deleteAccountsAccount
      x-api-path-slug: accountsaccountid-delete
      parameters:
      - in: path
        name: AccountID
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
    get:
      summary: Get Accounts
      description: Get accounts account.
      operationId: getAccountsAccount
      x-api-path-slug: accountsaccountid-get
      parameters:
      - in: path
        name: AccountID
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
    post:
      summary: Post Accounts
      description: Post accounts account.
      operationId: postAccountsAccount
      x-api-path-slug: accountsaccountid-post
      parameters:
      - in: path
        name: AccountID
      - in: body
        name: Accounts
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
    x-related-model:
      summary: X-related-model Accounts
      description: X-related-model accounts account.
      operationId: x-related-modelAccountsAccount
      x-api-path-slug: accountsaccountid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
  /Accounts/{AccountID}/Attachments:
    get:
      summary: Get Accounts Attachments
      description: Get accounts account attachments.
      operationId: getAccountsAccountAttachments
      x-api-path-slug: accountsaccountidattachments-get
      parameters:
      - in: path
        name: AccountID
        description: The Xero generated unique identifier for an account
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
      - Attachments
  /Accounts/{AccountID}/Attachments/{FileName}:
    get:
      summary: Get Accounts Attachments Filename
      description: Get accounts account attachments filename.
      operationId: getAccountsAccountAttachmentsFilename
      x-api-path-slug: accountsaccountidattachmentsfilename-get
      parameters:
      - in: path
        name: AccountID
        description: The Xero generated unique identifier for an account
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
      - Attachments
      - FileName
    post:
      summary: Post Accounts Attachments Filename
      description: Post accounts account attachments filename.
      operationId: postAccountsAccountAttachmentsFilename
      x-api-path-slug: accountsaccountidattachmentsfilename-post
      parameters:
      - in: path
        name: AccountID
        description: The Xero generated unique identifier for an account
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
      - Attachments
      - FileName
---