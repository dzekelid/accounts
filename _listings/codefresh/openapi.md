---
swagger: "2.0"
x-collection-name: Codefresh
x-complete: 1
info:
  title: Codefresh API
  description: codefresh-api-swagger2-0-specification
  termsOfService: http://www.codefresh.io
  contact:
    name: Codefresh api team
    url: http://www.codefresh.io
  version: 1.0.0
host: g.codefresh.io
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/accounts:
    get:
      summary: Get Admin Accounts
      description: Get admin accounts.
      operationId: getAdminAccounts
      x-api-path-slug: adminaccounts-get
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
    post:
      summary: Post Admin Accounts
      description: Post admin accounts.
      operationId: postAdminAccounts
      x-api-path-slug: adminaccounts-post
      parameters:
      - in: body
        name: account
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
  /admin/accounts/{id}:
    get:
      summary: Get Admin Accounts
      description: Get admin accounts.
      operationId: getAdminAccounts
      x-api-path-slug: adminaccountsid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
    delete:
      summary: Delete Admin Accounts
      description: Delete admin accounts.
      operationId: deleteAdminAccounts
      x-api-path-slug: adminaccountsid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
  /admin/accounts/{id}/update:
    post:
      summary: Post Admin Accounts Update
      description: Post admin accounts update.
      operationId: postAdminAccountsUpdate
      x-api-path-slug: adminaccountsidupdate-post
      parameters:
      - in: body
        name: accountDetails
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
  /admin/accounts/addpendinguser:
    post:
      summary: Post Admin Accounts Addpendinguser
      description: Post admin accounts addpendinguser.
      operationId: postAdminAccountsAddpendinguser
      x-api-path-slug: adminaccountsaddpendinguser-post
      parameters:
      - in: body
        name: newUser
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
      - Pendinguser
  /accounts/{id}/users:
    get:
      summary: Get Accounts Users
      description: Get accounts users.
      operationId: getAccountsUsers
      x-api-path-slug: accountsidusers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Users
  /accounts/{id}/update:
    post:
      summary: Post Accounts Update
      description: Post accounts update.
      operationId: postAccountsUpdate
      x-api-path-slug: accountsidupdate-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: updateData
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /accounts/{id}/adduser:
    post:
      summary: Post Accounts Adduser
      description: Post accounts adduser.
      operationId: postAccountsAdduser
      x-api-path-slug: accountsidadduser-post
      parameters:
      - in: body
        name: newUser
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - User
  /accounts/{accountId}/{userId}/adduser:
    post:
      summary: Post Accounts Adduser
      description: Post accounts adduser.
      operationId: postAccountsAccountUserAdduser
      x-api-path-slug: accountsaccountiduseridadduser-post
      parameters:
      - in: path
        name: accountId
        description: id of an object
      - in: path
        name: userId
        description: id of an object
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - User
  /accounts/{accountId}/{userId}:
    delete:
      summary: Delete Accounts
      description: Delete accounts.
      operationId: deleteAccountsAccountUser
      x-api-path-slug: accountsaccountiduserid-delete
      parameters:
      - in: path
        name: accountId
        description: id of an object
      - in: path
        name: userId
        description: id of an object
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /accounts/{id}/updateuser:
    post:
      summary: Post Accounts Updateuser
      description: Post accounts updateuser.
      operationId: postAccountsUpdateuser
      x-api-path-slug: accountsidupdateuser-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: userDetails
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - User
  /accounts/{accountId}/{userId}/admin:
    post:
      summary: Post Accounts Admin
      description: Post accounts admin.
      operationId: postAccountsAccountUserAdmin
      x-api-path-slug: accountsaccountiduseridadmin-post
      parameters:
      - in: path
        name: accountId
        description: id of an object
      - in: path
        name: userId
        description: id of an object
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Admin
    delete:
      summary: Delete Accounts Admin
      description: Delete accounts admin.
      operationId: deleteAccountsAccountUserAdmin
      x-api-path-slug: accountsaccountiduseridadmin-delete
      parameters:
      - in: path
        name: accountId
        description: id of an object
      - in: path
        name: userId
        description: id of an object
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Admin
  /user/changeaccount/{accountId}:
    post:
      summary: Post User Changeaccount Accountid
      description: Post user changeaccount accountid.
      operationId: postUserChangeaccountAccount
      x-api-path-slug: userchangeaccountaccountid-post
      parameters:
      - in: path
        name: accountId
        description: id of an object
      responses:
        200:
          description: OK
      tags:
      - User
      - Changeaccount
      - Accountid
  /features/{accountId}:
    get:
      summary: Get Features Accountid
      description: Get features accountid.
      operationId: getFeaturesAccount
      x-api-path-slug: featuresaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The ID of the account to query for feature availability
      responses:
        200:
          description: OK
      tags:
      - Features
      - Accountid
---