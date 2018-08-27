---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Create a new System account eg. new client account
  version: 1.0.0
  description: Create a new system account eg. new client account.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/account/all:
    get:
      summary: Get all accounts paginated
      description: Get all accounts paginated.
      operationId: Account_GetAllBypageSizeBypageNumber
      x-api-path-slug: apiaccountall-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Paginated
  /api/account/setstatus:
    post:
      summary: Set an accounts status
      description: Set an accounts status.
      operationId: Account_SetStatusBydataContract
      x-api-path-slug: apiaccountsetstatus-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Accounts
      - Status
  /api/account/systemaccounts:
    get:
      summary: Get list of all system accounts
      description: Get list of all system accounts.
      operationId: Account_GetSystemAccounts
      x-api-path-slug: apiaccountsystemaccounts-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - System
      - Accounts
  /api/account/pm/list:
    post:
      summary: Get list of accounts with sorting and searching and by type of group
        for the accounts
      description: Get list of accounts with sorting and searching and by type of
        group for the accounts.
      operationId: Account_GetPMAccountsBydataContractBypageSizeBypageNumber
      x-api-path-slug: apiaccountpmlist-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Accounts
      - Sorting
      - Searching
      - By
      - Type
      - Of
      - Groupthe
      - Accounts
  /api/account/customer/overview:
    get:
      summary: Get an overview of customer accounts
      description: Get an overview of customer accounts.
      operationId: Account_GetCustomersOverview
      x-api-path-slug: apiaccountcustomeroverview-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Overview
      - Of
      - Customer
      - Accounts
  /api/accountingsystem/officeaccounts:
    get:
      summary: Get list of office accounts associated with the accounting system
      description: Get list of office accounts associated with the accounting system.
      operationId: AccountingSystem_GetOfficeAccounts
      x-api-path-slug: apiaccountingsystemofficeaccounts-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Office
      - Accounts
      - Associated
      - Accounting
      - System
  /api/transfer/interaccount:
    post:
      summary: Transfer funds between bank accounts (also Deposit Cash/Cheques from
        Cash Held)
      description: Transfer funds between bank accounts (also deposit cash/cheques
        from cash held).
      operationId: Transfer_ProcessIatByiatDataContract
      x-api-path-slug: apitransferinteraccount-post
      parameters:
      - in: body
        name: iatDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Transfer
      - Funds
      - Between
      - Bank
      - Accounts
      - (also
      - Deposit
      - Cash
      - Cheques
      - From
      - Cash
      - Held)
  /api/account/{id}:
    get:
      summary: Get Account By Id
      description: Get account by id.
      operationId: Account_GetByid
      x-api-path-slug: apiaccountid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
  /api/account/{id}/ledger:
    post:
      summary: Retrieve ledger posting details for an account
      description: Retrieve ledger posting details for an account.
      operationId: Account_GetLedgerByidBydataContract
      x-api-path-slug: apiaccountidledger-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Ledger
      - Posting
      - Detailsan
      - Account
  /api/account/ledger:
    post:
      summary: Retrive ledger postings without account id
      description: Retrive ledger postings without account id.
      operationId: Account_GetAllLedgerBydataContract
      x-api-path-slug: apiaccountledger-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Retrive
      - Ledger
      - Postings
      - Without
      - Account
      - Id
  /api/account/{id}/update:
    put:
      summary: Update account details
      description: Update account details.
      operationId: Account_UpdateAccountDetailsByidBydetailsDataContract
      x-api-path-slug: apiaccountidupdate-put
      parameters:
      - in: body
        name: detailsDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Account
      - Details
  /api/account/{id}/statement:
    post:
      summary: Get a statement for an account
      description: Get a statement for an account.
      operationId: Account_GetStatementByidBystatementDataContract
      x-api-path-slug: apiaccountidstatement-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: statementDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Statementan
      - Account
  /api/account/createsystemaccount:
    post:
      summary: Create a new System account eg. new client account
      description: Create a new system account eg. new client account.
      operationId: Account_CreateSystemAccountBydataContract
      x-api-path-slug: apiaccountcreatesystemaccount-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - New
      - System
      - Account
      - Eg
      - ""
      - New
      - Client
      - Account
  /api/account/{id}/balances:
    get:
      summary: Get balance of an account
      description: Get balance of an account.
      operationId: Account_GetAccountBalancesByidBystartDateByendDate
      x-api-path-slug: apiaccountidbalances-get
      parameters:
      - in: query
        name: endDate
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: startDate
      responses:
        200:
          description: OK
      tags:
      - Balance
      - Of
      - Account
  /api/account/payments/overview:
    get:
      summary: Get an overview of account amounts and totals
      description: Get an overview of account amounts and totals.
      operationId: Account_GetPaymentsOverview
      x-api-path-slug: apiaccountpaymentsoverview-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Overview
      - Of
      - Account
      - Amounts
      - Totals
  /api/account/{id}/deposits:
    get:
      summary: Get Deposits processed for an Account
      description: Get deposits processed for an account.
      operationId: Account_GetDepositsByid
      x-api-path-slug: apiaccountiddeposits-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Deposits
      - Processedan
      - Account
  /api/account/{id}/invoiceoverview:
    post:
      summary: Get summary of an account based on invoice amounts allocated
      description: Get summary of an account based on invoice amounts allocated.
      operationId: Account_GetInvoiceOverviewByidBydataContract
      x-api-path-slug: apiaccountidinvoiceoverview-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Summary
      - Of
      - Account
      - Based
      - "On"
      - Invoice
      - Amounts
      - Ocated
  /api/account/{id}/paymentoverview:
    post:
      summary: Get payment overview for an account
      description: Get payment overview for an account.
      operationId: Account_GetAccountPaymentOverviewByid
      x-api-path-slug: apiaccountidpaymentoverview-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Overviewan
      - Account
  /api/accountingsystem/suspense:
    get:
      summary: Get amount of funds held in suspense account of the accounting system
      description: Get amount of funds held in suspense account of the accounting
        system.
      operationId: AccountingSystem_GetSuspenseFunds
      x-api-path-slug: apiaccountingsystemsuspense-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Amount
      - Of
      - Funds
      - Held
      - In
      - Suspense
      - Account
      - Of
      - Accounting
      - System
  /api/accountingsystem/agentcash:
    get:
      summary: Gets overview of the agent cash account
      description: Gets overview of the agent cash account.
      operationId: AccountingSystem_GetAgentCash
      x-api-path-slug: apiaccountingsystemagentcash-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Overview
      - Of
      - Agent
      - Cash
      - Account
  /api/agency/accountmanager:
    get:
      summary: Get the account manager for an agency
      description: Get the account manager for an agency.
      operationId: Agency_AccountManager
      x-api-path-slug: apiagencyaccountmanager-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Account
      - Manageran
      - Agency
  /api/deposit/allocate:
    post:
      summary: Receipt (optional) and allocate deposit funds to holding account
      description: Receipt (optional) and allocate deposit funds to holding account.
      operationId: Deposit_ReceiptAndAllocateDepositBymoveDataContract
      x-api-path-slug: apidepositallocate-post
      parameters:
      - in: body
        name: moveDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Receipt
      - (optional)
      - Ocate
      - Deposit
      - Funds
      - To
      - Holding
      - Account
  /api/digitalsignature/signable/setup/{brandId}/{logoId}/{colour}:
    get:
      summary: creates a new account on signable
      description: Creates a new account on signable.
      operationId: DigitalSignature_SetupBybrandIdBylogoIdBycolourByemailAddress
      x-api-path-slug: apidigitalsignaturesignablesetupbrandidlogoidcolour-get
      parameters:
      - in: path
        name: brandId
        description: brand to associate this sub account to
      - in: path
        name: colour
        description: the web colour to be used in the signable app as a background
          colour, should probably match a logo colour
      - in: query
        name: emailAddress
        description: unique email address for this brand
      - in: path
        name: logoId
        description: logo id used for whitelabelling
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Account
      - "On"
      - Signable
  /api/digitalsignature/signable/delete/{brandId}:
    delete:
      summary: delete a sub account on signable
      description: Delete a sub account on signable.
      operationId: DigitalSignature_DeleteBybrandId
      x-api-path-slug: apidigitalsignaturesignabledeletebrandid-delete
      parameters:
      - in: path
        name: brandId
        description: brand to associate this sub account to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Delete
      - Sub
      - Account
      - "On"
      - Signable
  /api/posting/suspense:
    get:
      summary: Get all ledger postings in the suspense account
      description: Get all ledger postings in the suspense account.
      operationId: Posting_GetSuspensePostingsBypageSizeBypageNumber
      x-api-path-slug: apipostingsuspense-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Ledger
      - Postings
      - In
      - Suspense
      - Account
  /api/receipt/addfunds:
    post:
      summary: Add funds to an account/group by id or suspense account
      description: Add funds to an account/group by id or suspense account.
      operationId: Receipt_ReceiptFundsByreceiptFundsDataContract
      x-api-path-slug: apireceiptaddfunds-post
      parameters:
      - in: body
        name: receiptFundsDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Funds
      - To
      - Account
      - Group
      - By
      - Id
      - Suspense
      - Account
  /api/receipt/interestearned:
    post:
      summary: Add interest earned to suspense account
      description: Add interest earned to suspense account.
      operationId: Receipt_ReceiptInterestEarnedByinterestEarnedDataContract
      x-api-path-slug: apireceiptinterestearned-post
      parameters:
      - in: body
        name: interestEarnedDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Interest
      - Earned
      - To
      - Suspense
      - Account
  /api/receipt/recordpayment:
    post:
      summary: Makes payment to supplied account.
      description: Makes payment to supplied account..
      operationId: Receipt_RecordPaymentByrecordPaymentDataContract
      x-api-path-slug: apireceiptrecordpayment-post
      parameters:
      - in: body
        name: recordPaymentDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Makes
      - Payment
      - To
      - Supplied
      - Account
  /api/receipt/fundsshortfall:
    post:
      summary: Records funds from office account into client account and then to client
        if necessary.
      description: Records funds from office account into client account and then
        to client if necessary..
      operationId: Receipt_ReceiptFundsShortfallBydataContract
      x-api-path-slug: apireceiptfundsshortfall-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Funds
      - From
      - Office
      - Account
      - Into
      - Client
      - Account
      - Then
      - To
      - Client
      - If
      - Necessary
  /api/reconcile/account/{id}/statements:
    get:
      summary: Get reconcile statements for bank account
      description: Get reconcile statements for bank account.
      operationId: Reconcile_GetStatementsByid
      x-api-path-slug: apireconcileaccountidstatements-get
      parameters:
      - in: path
        name: id
        description: Bank Account Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Reconcile
      - Statementsbank
      - Account
  /api/tax/pay/hmrc:
    post:
      summary: Pay tax out of tax held account
      description: Pay tax out of tax held account.
      operationId: Tax_PayTaxHmrcBypayTaxDataContract
      x-api-path-slug: apitaxpayhmrc-post
      parameters:
      - in: body
        name: payTaxDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Tax
      - Out
      - Of
      - Tax
      - Held
      - Account
  /api/transfer/suspend:
    post:
      summary: Move funds to suspense account to another ledger
      description: Move funds to suspense account to another ledger.
      operationId: Transfer_ProcessSuspendFundsBysuspendDataContract
      x-api-path-slug: apitransfersuspend-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: suspendDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Move
      - Funds
      - To
      - Suspense
      - Account
      - To
      - Another
      - Ledger
  /api/transfer/unsuspend:
    post:
      summary: Move funds from suspense account to another ledger
      description: Move funds from suspense account to another ledger.
      operationId: Transfer_ProcessUnsuspendFundsBysuspendDataContract
      x-api-path-slug: apitransferunsuspend-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: suspendDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Move
      - Funds
      - From
      - Suspense
      - Account
      - To
      - Another
      - Ledger
  /api/account/create:
    post:
      summary: Create account for groupId provided
      description: Create account for groupid provided.
      operationId: Account_CreateGroupAccountBydataContract
      x-api-path-slug: apiaccountcreate-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - AccountgroupId
      - Provided
  /api/account/systemaccount:
    get:
      summary: Get System Account for the Accounting System
      description: Get system account for the accounting system.
      operationId: Account_GetSystemAccount
      x-api-path-slug: apiaccountsystemaccount-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - System
      - Accountthe
      - Accounting
      - System
  /api/accountingsystem/createofficeaccount:
    post:
      summary: Create an office account for the accounting system
      description: Create an office account for the accounting system.
      operationId: AccountingSystem_CreateOfficeAccountBydataContract
      x-api-path-slug: apiaccountingsystemcreateofficeaccount-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Office
      - Accountthe
      - Accounting
      - System
  /api/posting/cash:
    get:
      summary: Get all postings in the cash account for the agent
      description: Get all postings in the cash account for the agent.
      operationId: Posting_GetCashFunds
      x-api-path-slug: apipostingcash-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Postings
      - In
      - Cash
      - Accountthe
      - Agent
  /api/accountingsystem/setprimaryaccount:
    post:
      summary: Set Primary Bank Account for Accounting System
      description: Set primary bank account for accounting system.
      operationId: AccountingSystem_SetPrimarySystemBankAccountByid
      x-api-path-slug: apiaccountingsystemsetprimaryaccount-post
      parameters:
      - in: query
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Primary
      - Bank
      - AccountAccounting
      - System
  /api/accountingsystem/taxstatus:
    get:
      summary: Get Tax Status of Accounting System
      description: Get tax status of accounting system.
      operationId: AccountingSystem_GetTaxStatus
      x-api-path-slug: apiaccountingsystemtaxstatus-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Tax
      - Status
      - Of
      - Accounting
      - System
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