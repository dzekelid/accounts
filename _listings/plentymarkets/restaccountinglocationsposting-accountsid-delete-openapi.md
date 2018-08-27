---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Delete an posting account
  description: Delete an posting account.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounting/locations/existing_accounts:
    get:
      summary: Get all unique posting accounts
      description: Get all unique posting accounts.
      operationId: getRestAccountingLocationsExistingAccounts
      x-api-path-slug: restaccountinglocationsexisting-accounts-get
      responses:
        200:
          description: OK
      tags:
      - Unique
      - Posting
      - Accounts
  /rest/accounting/locations/posting_accounts:
    get:
      summary: Get all posting accounts
      description: Get all posting accounts.
      operationId: getRestAccountingLocationsAddingAccounts
      x-api-path-slug: restaccountinglocationsposting-accounts-get
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Accounts
    post:
      summary: Save posting accounts
      description: Save posting accounts.
      operationId: postRestAccountingLocationsAddingAccounts
      x-api-path-slug: restaccountinglocationsposting-accounts-post
      responses:
        200:
          description: OK
      tags:
      - Save
      - Posting
      - Accounts
  /rest/accounting/locations/{locationId}/debtor_accounts/{mode}:
    get:
      summary: Lists the debtor accounts by mode.
      description: Lists the debtor accounts of an accounting location by mode. The
        ID of the accounting location and the mode have to be specified.
      operationId: getRestAccountingLocationsLocationDebtorAccountsMode
      x-api-path-slug: restaccountinglocationslocationiddebtor-accountsmode-get
      parameters:
      - in: path
        name: locationId
      - in: path
        name: mode
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Debtor
      - Accounts
      - By
      - Mode
  /rest/accounting/locations/{locationId}/posting_accounts:
    get:
      summary: Get all posting accounts by locationId
      description: Get all posting accounts by locationid.
      operationId: getRestAccountingLocationsLocationAddingAccounts
      x-api-path-slug: restaccountinglocationslocationidposting-accounts-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Accounts
      - By
      - LocationId
  /rest/accounting/locations/{locationId}/{type}/posting_accounts:
    get:
      summary: Get all posting accounts by locationId and type
      description: Get all posting accounts by locationid and type.
      operationId: getRestAccountingLocationsLocationTypeAddingAccounts
      x-api-path-slug: restaccountinglocationslocationidtypeposting-accounts-get
      parameters:
      - in: path
        name: locationId
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Accounts
      - By
      - LocationId
      - Type
  /rest/accounts:
    get:
      summary: List accounts
      description: List accounts.
      operationId: getRestAccounts
      x-api-path-slug: restaccounts-get
      parameters:
      - in: query
        name: createdAt
        description: Filter that restricts the search result to accounts that were
          created according to given filters
      - in: query
        name: updatedAt
        description: Filter that restricts the search result to accounts that were
          updated according to given filters
      responses:
        200:
          description: OK
      tags:
      - List
      - Accounts
    post:
      summary: Create an account
      description: Create an account.
      operationId: postRestAccounts
      x-api-path-slug: restaccounts-post
      parameters:
      - in: body
        name: /rest/accounts
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
  /rest/accounts/contacts/{contactId}/banks:
    get:
      summary: List bank accounts
      description: Lists bank accounts of the contact. The ID of the contact must
        be specified.
      operationId: getRestAccountsContactsContactBanks
      x-api-path-slug: restaccountscontactscontactidbanks-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - List
      - Bank
      - Accounts
  /rest/items/sales_prices/{id}/accounts:
    get:
      summary: List referrer accounts
      description: Lists all activated referrer accounts of a sales price.
      operationId: getRestItemsSalesPricesAccounts
      x-api-path-slug: restitemssales-pricesidaccounts-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Referrer
      - Accounts
    post:
      summary: Activate a referrer account
      description: Activates a referrer account for a sales price.
      operationId: postRestItemsSalesPricesAccounts
      x-api-path-slug: restitemssales-pricesidaccounts-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/accounts
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Referrer
      - Account
  /rest/payments/methods/ebics:
    get:
      summary: Get EBICS Accounts
      description: Get ebics accounts.
      operationId: getRestPaymentsMethodsEbics
      x-api-path-slug: restpaymentsmethodsebics-get
      responses:
        200:
          description: OK
      tags:
      - EBICS
      - Accounts
    post:
      summary: Create an EBICS Account
      description: Create an ebics account.
      operationId: postRestPaymentsMethodsEbics
      x-api-path-slug: restpaymentsmethodsebics-post
      parameters:
      - in: query
        name: name
        description: The name of the EBICS Account
      responses:
        200:
          description: OK
      tags:
      - EBICS
      - Account
  /rest/accounting/locations/posting_accounts/{id}:
    delete:
      summary: Delete an posting account
      description: Delete an posting account.
      operationId: deleteRestAccountingLocationsAddingAccounts
      x-api-path-slug: restaccountinglocationsposting-accountsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Account
    get:
      summary: Gets posting account by the unique id
      description: Gets posting account by the unique id.
      operationId: getRestAccountingLocationsAddingAccounts
      x-api-path-slug: restaccountinglocationsposting-accountsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - S
      - Posting
      - Account
      - By
      - Unique
      - Id
  /rest/accounting/locations/revenue_account_configurations:
    get:
      summary: List revenue account configurations
      description: Lists revenue account configurations of a system. The revenue accounts
        are returned as paginated result. By default 50 revenue accounts are on one
        page.
      operationId: getRestAccountingLocationsRevenueAccountConfigurations
      x-api-path-slug: restaccountinglocationsrevenue-account-configurations-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of revenue accounts to be displayed per page
      - in: query
        name: page
        description: The page to get
      responses:
        200:
          description: OK
      tags:
      - List
      - Revenue
      - Account
      - Configurations
  /rest/accounting/locations/{locationId}/countries/{countryId}/revenue_accounts:
    get:
      summary: Get the revenue account configuration of a country
      description: Get the revenue account configuration of a country. The ID of the
        accounting location that the country is associated with as well as the ID
        of the country must be specified.
      operationId: getRestAccountingLocationsLocationCountriesCountryRevenueAccounts
      x-api-path-slug: restaccountinglocationslocationidcountriescountryidrevenue-accounts-get
      parameters:
      - in: path
        name: countryId
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Revenue
      - Account
      - Configuration
      - Of
      - Country
  /rest/accounting/locations/{locationId}/debtor_account_configurations:
    get:
      summary: Get debtor account configuration of an accounting location
      description: Gets the debtor account configuration of an accounting location.
        The ID of the accounting location has to be specified. The debtor account
        configuration can contain one standard debtor account only or e.g. several
        accounts for each country of delivery.
      operationId: getRestAccountingLocationsLocationDebtorAccountConfigurations
      x-api-path-slug: restaccountinglocationslocationiddebtor-account-configurations-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Debtor
      - Account
      - Configuration
      - Of
      - Accounting
      - Location
  /rest/accounting/locations/{locationId}/revenue_account_configurations:
    get:
      summary: Get the revenue account configuration of an accounting location
      description: Gets the revenue account configuration of an accounting location.
        A revenue account location configuration contains several revenue accounts.
        The ID of the accounting location has to be specified.
      operationId: getRestAccountingLocationsLocationRevenueAccountConfigurations
      x-api-path-slug: restaccountinglocationslocationidrevenue-account-configurations-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Revenue
      - Account
      - Configuration
      - Of
      - Accounting
      - Location
  /rest/accounts/contact_relations/{accountContactRelationId}:
    delete:
      summary: Deletes an account contact relation. The ID of the account contact
        relation must be specified.
      description: Deletes an account contact relation. the id of the account contact
        relation must be specified..
      operationId: deleteRestAccountsContactRelationsAccountcontactrelation
      x-api-path-slug: restaccountscontact-relationsaccountcontactrelationid-delete
      parameters:
      - in: path
        name: accountContactRelationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Account
      - Contact
      - Relation
      - ""
      - ID
      - Of
      - Account
      - Contact
      - Relation
      - Must
      - Be
      - Specified
    get:
      summary: Gets an account contact releation. The ID of the account contact relation
        must be specified.
      description: Gets an account contact releation. the id of the account contact
        relation must be specified..
      operationId: getRestAccountsContactRelationsAccountcontactrelation
      x-api-path-slug: restaccountscontact-relationsaccountcontactrelationid-get
      parameters:
      - in: path
        name: accountContactRelationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Account
      - Contact
      - Releation
      - ""
      - ID
      - Of
      - Account
      - Contact
      - Relation
      - Must
      - Be
      - Specified
  /rest/accounts/contacts/banks:
    post:
      summary: Create a bank account
      description: Create a bank account.
      operationId: postRestAccountsContactsBanks
      x-api-path-slug: restaccountscontactsbanks-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/banks
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bank
      - Account
  /rest/accounts/contacts/banks/{contactBankId}:
    delete:
      summary: Delete a bank account
      description: Deletes a bank account. The ID of the bank account must be specified.
      operationId: deleteRestAccountsContactsBanksContactbank
      x-api-path-slug: restaccountscontactsbankscontactbankid-delete
      parameters:
      - in: path
        name: contactBankId
      responses:
        200:
          description: OK
      tags:
      - Bank
      - Account
    get:
      summary: Get a bank account
      description: Gets a bank account of the contact. The ID of the bank account
        must be specified.
      operationId: getRestAccountsContactsBanksContactbank
      x-api-path-slug: restaccountscontactsbankscontactbankid-get
      parameters:
      - in: path
        name: contactBankId
      responses:
        200:
          description: OK
      tags:
      - Bank
      - Account
    put:
      summary: Update a bank account
      description: Updates a bank account. The ID of the bank account must be specified.
      operationId: putRestAccountsContactsBanksContactbank
      x-api-path-slug: restaccountscontactsbankscontactbankid-put
      parameters:
      - in: body
        name: /rest/accounts/contacts/banks/{contactBankId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contactBankId
      responses:
        200:
          description: OK
      tags:
      - Bank
      - Account
  /rest/accounts/contacts/{contactId}/accounts/{accountId}:
    delete:
      summary: Delete an account of the contact
      description: Deletes an account of the contact. The ID of the contact and the
        ID of the account must be specified.
      operationId: deleteRestAccountsContactsContactAccountsAccount
      x-api-path-slug: restaccountscontactscontactidaccountsaccountid-delete
      parameters:
      - in: path
        name: accountId
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Account
      - Of
      - Contact
    get:
      summary: Get an account of the contact
      description: Gets an account of the contact. The ID of the contact and the ID
        of the account must be specified.
      operationId: getRestAccountsContactsContactAccountsAccount
      x-api-path-slug: restaccountscontactscontactidaccountsaccountid-get
      parameters:
      - in: path
        name: accountId
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Account
      - Of
      - Contact
    put:
      summary: Update an account
      description: Updates an account. The ID of the contact and the ID of the account
        must be specified.
      operationId: putRestAccountsContactsContactAccountsAccount
      x-api-path-slug: restaccountscontactscontactidaccountsaccountid-put
      parameters:
      - in: path
        name: accountId
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Account
  /rest/accounts/{accountId}:
    delete:
      summary: Delete an account
      description: Deletes an account. The ID of the account must be specified.
      operationId: deleteRestAccountsAccount
      x-api-path-slug: restaccountsaccountid-delete
      parameters:
      - in: path
        name: accountId
      responses:
        200:
          description: OK
      tags:
      - Account
    get:
      summary: Get an account
      description: Gets an account. The ID of the account must be specified.
      operationId: getRestAccountsAccount
      x-api-path-slug: restaccountsaccountid-get
      parameters:
      - in: path
        name: accountId
      responses:
        200:
          description: OK
      tags:
      - Account
    put:
      summary: Update an account
      description: Updates an account. The ID of the account must be specified.
      operationId: putRestAccountsAccount
      x-api-path-slug: restaccountsaccountid-put
      parameters:
      - in: body
        name: /rest/accounts/{accountId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: accountId
      responses:
        200:
          description: OK
      tags:
      - Account
  /rest/items/sales_prices/{id}/accounts/{accountType}/{accountId}:
    delete:
      summary: Deactivate a referrer account
      description: Deactivates a referrer account for a sales price.
      operationId: deleteRestItemsSalesPricesAccountsAccounttypeAccount
      x-api-path-slug: restitemssales-pricesidaccountsaccounttypeaccountid-delete
      parameters:
      - in: path
        name: accountId
      - in: path
        name: accountType
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Referrer
      - Account
  /rest/accounts/contacts/{contactId}/accounts:
    post:
      summary: Create an account for existing contact
      description: Creates an account for an existing contact. The ID of the contact
        must be specified.
      operationId: postRestAccountsContactsContactAccounts
      x-api-path-slug: restaccountscontactscontactidaccounts-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/{contactId}/accounts
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Accountexisting
      - Contact
  /rest/accounting/locations/{webstoreId}/{countryId}/posting_accounts:
    get:
      summary: Get all posting accounts for a country of a webstore
      description: Get all posting accounts for a country of a webstore.
      operationId: getRestAccountingLocationsWebstoreCountryAddingAccounts
      x-api-path-slug: restaccountinglocationswebstoreidcountryidposting-accounts-get
      parameters:
      - in: query
        name: $webstoreId
        description: The ID of the webstore
      - in: path
        name: countryId
      - in: path
        name: webstoreId
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Accountsa
      - Country
      - Of
      - Webstore
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