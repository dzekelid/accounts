---
name: Capital One DevExchange
x-slug: capital-one-devexchange
description: What unites us all is a desire to create better end customer experiences.
  Were building a full suite of tools and technology that make essential things in
  peoples everyday life &ndash; money, finances, identity &ndash; simpler for you.
  Now is the time to join our beta program, and help us shape the future.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Accounts
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/apis.md
specificationVersion: "0.14"
apis:
- name: Capital One DevExchange Get all accounts
  x-api-slug: capital-one-devexchange
  description: Returns the accounts that have been assigned to you.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts
  tags: Banks,Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accounts-get-openapi.md
- name: Capital One DevExchange Get account by id
  x-api-slug: capital-one-devexchange
  description: Returns the account with the specific id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}
  tags: Banks,Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsid-get-openapi.md
- name: Capital One DevExchange Update a specific existing account
  x-api-slug: capital-one-devexchange
  description: Updates the specific account
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}
  tags: Banks,Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsid-put-openapi.md
- name: Capital One DevExchange Delete a specific existing account
  x-api-slug: capital-one-devexchange
  description: Deletes the specific account
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}
  tags: Banks,Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsid-delete-openapi.md
- name: Capital One DevExchange Create an account
  x-api-slug: capital-one-devexchange
  description: Creates an account for the customer with the id provided
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////customers/{id}/accounts
  tags: Banks,Customers, , Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/customersidaccounts-post-openapi.md
- name: Capital One DevExchange Get accounts by customer id
  x-api-slug: capital-one-devexchange
  description: Returns the accounts associated with the specific customer
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////customers/{id}/accounts
  tags: Banks,Customers, , Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/customersidaccounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/customersidaccounts-get-openapi.md
- name: Capital One DevExchange Get customer that owns the specified account
  x-api-slug: capital-one-devexchange
  description: Returns the customer that the account belongs to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/customer
  tags: Banks,Accounts, , Customer
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidcustomer-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidcustomer-get-openapi.md
- name: Capital One DevExchange Get all bills for a specific account
  x-api-slug: capital-one-devexchange
  description: Returns the bills that are tied to the specific account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/bills
  tags: Banks,Accounts, , Bills
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidbills-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidbills-get-openapi.md
- name: Capital One DevExchange Create a bill
  x-api-slug: capital-one-devexchange
  description: Creates a bill for the specific account
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/bills
  tags: Banks,Accounts, , Bills
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidbills-post-openapi.md
- name: Capital One DevExchange Get all deposits
  x-api-slug: capital-one-devexchange
  description: Returns the deposits that you are involved in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/deposits
  tags: Banks,Accounts, , Deposits
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsiddeposits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsiddeposits-get-openapi.md
- name: Capital One DevExchange Create a deposit
  x-api-slug: capital-one-devexchange
  description: Creates a deposit where the account with the ID specified receives
    the amount.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/deposits
  tags: Banks,Accounts, , Deposits
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsiddeposits-post-openapi.md
- name: Capital One DevExchange Get all loans
  x-api-slug: capital-one-devexchange
  description: Returns the loans that you are involved in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/loans
  tags: Banks,Accounts, , Loans
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidloans-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidloans-get-openapi.md
- name: Capital One DevExchange Create a loan
  x-api-slug: capital-one-devexchange
  description: Creates a loan where the account with the ID specified is debitted.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/loans
  tags: Banks,Accounts, , Loans
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidloans-post-openapi.md
- name: Capital One DevExchange Get all purchases
  x-api-slug: capital-one-devexchange
  description: Returns the purchases that you are involved in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/purchases
  tags: Banks,Accounts, , Purchases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidpurchases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidpurchases-get-openapi.md
- name: Capital One DevExchange Create a purchase
  x-api-slug: capital-one-devexchange
  description: Creates a purchase where the account with the ID specified is the payer.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/purchases
  tags: Banks,Accounts, , Purchases
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidpurchases-post-openapi.md
- name: Capital One DevExchange Get all purchases by account and merchant
  x-api-slug: capital-one-devexchange
  description: Returns the purchases that a merchant is involved in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////merchants/{id}/accounts/{accountId}/purchases
  tags: Banks,Merchants, , Accounts, Account, Purchases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/merchantsidaccountsaccountidpurchases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/merchantsidaccountsaccountidpurchases-get-openapi.md
- name: Capital One DevExchange Get all transfers
  x-api-slug: capital-one-devexchange
  description: Returns the transfers that you are involved in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/transfers
  tags: Banks,Accounts, , Transfers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidtransfers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidtransfers-get-openapi.md
- name: Capital One DevExchange Create a transfer
  x-api-slug: capital-one-devexchange
  description: Creates a transfer where the account with the ID specified is the payer.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/transfers
  tags: Banks,Accounts, , Transfers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidtransfers-post-openapi.md
- name: Capital One DevExchange Get all withdrawals
  x-api-slug: capital-one-devexchange
  description: Returns the withdrawals that you are involved in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/withdrawals
  tags: Banks,Accounts, , Withdrawals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidwithdrawals-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidwithdrawals-get-openapi.md
- name: Capital One DevExchange Create a withdrawal
  x-api-slug: capital-one-devexchange
  description: Creates a withdrawal where the account with the ID specified is debitted.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/withdrawals
  tags: Banks,Accounts, , Withdrawals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/accountsidwithdrawals-post-openapi.md
- name: Capital One DevExchange
  x-api-slug: capital-one-devexchange
  description: What unites us all is a desire to create better end customer experiences.
    Were building a full suite of tools and technology that make essential things
    in peoples everyday life &ndash; money, finances, identity &ndash; simpler for
    you. Now is the time to join our beta program, and help us shape the future.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com//
  tags: Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/capital-one-devexchange/openapi.md
x-common:
- type: x-authentication
  url: https://developer.capitalone.com/platform-documentation/authorization-with-oauth-20/
- type: x-blog
  url: https://developer.capitalone.com/blogs/
- type: x-developer
  url: https://developer.capitalone.com/
- type: x-documentation
  url: https://developer.capitalone.com/platform-documentation/
- type: x-errors
  url: https://developer.capitalone.com/platform-documentation/errors/
- type: x-getting-started
  url: https://developer.capitalone.com/platform-documentation/getting-started/
- type: x-github
  url: https://github.com/capitalone
- type: x-website
  url: http://capitalone.com
- type: x-open-source
  url: https://developer.capitalone.com/open-source/
- type: x-sandbox
  url: https://developer.capitalone.com/platform-documentation/using-the-sandbox/
- type: x-login
  url: https://developer.capitalone.com/sign-in/
- type: x-selfservice-registration
  url: https://developer.capitalone.com/sign-up
- type: x-support
  url: https://developer.capitalone.com/support/
- type: x-privacy-policy
  url: https://www.capitalone.com/identity-protection/privacy/statement
- type: x-terms-of-service
  url: https://developer.capitalone.com/single/terms-and-conditions/
- type: x-twitter
  url: https://twitter.com/CapitalOneDevEx
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---