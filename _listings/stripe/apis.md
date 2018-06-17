---
name: Stripe
x-slug: stripe
description: Online payment processing for internet businesses. Stripe is a suite
  of payment APIs that powers commerce for online businesses of all sizes, including
  fraud prevention, and subscription management. Use Stripe???s payment platform to
  accept and process p...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
x-kinRank: "10"
x-alexaRank: "1793"
tags: Accounts
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/apis.md
specificationVersion: "0.14"
apis:
- name: Stripe Add Account Bank Accounts
  x-api-slug: stripe
  description: Post Account, Bank, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///account/bank_accounts
  tags: Account, Bank, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountbank-accounts-post-openapi.md
- name: Stripe Delete Account Bank Accounts
  x-api-slug: stripe
  description: Delete Account, Bank, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///account/bank_accounts/{id}
  tags: Account, Bank, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountbank-accountsid-delete-openapi.md
- name: Stripe Get Account Bank Accounts
  x-api-slug: stripe
  description: Get Account, Bank, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///account/bank_accounts/{id}
  tags: Account, Bank, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountbank-accountsid-get-openapi.md
- name: Stripe Add Account Bank Accounts
  x-api-slug: stripe
  description: Updates the metadata of a bank account belonging to a Custom account,
    and optionally sets it as the default for its currency. Other bank account details
    are not editable by design.You can re-enable a disabled bank account by performing
    an update call without providing any arguments or changes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///account/bank_accounts/{id}
  tags: Account, Bank, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountbank-accountsid-post-openapi.md
- name: Stripe Get Account External Accounts
  x-api-slug: stripe
  description: Get Account, External, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///account/external_accounts
  tags: Account, External, Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountexternal-accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountexternal-accounts-get-openapi.md
- name: Stripe Add Account External Accounts
  x-api-slug: stripe
  description: Post Account, External, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///account/external_accounts
  tags: Account, External, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountexternal-accounts-post-openapi.md
- name: Stripe Delete Account External Accounts
  x-api-slug: stripe
  description: Delete Account, External, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///account/external_accounts/{id}
  tags: Account, External, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountexternal-accountsid-delete-openapi.md
- name: Stripe Get Account External Accounts
  x-api-slug: stripe
  description: Get Account, External, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///account/external_accounts/{id}
  tags: Account, External, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountexternal-accountsid-get-openapi.md
- name: Stripe Add Account External Accounts
  x-api-slug: stripe
  description: Updates the metadata of a bank account belonging to a Custom account,
    and optionally sets it as the default for its currency. Other bank account details
    are not editable by design.You can re-enable a disabled bank account by performing
    an update call without providing any arguments or changes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///account/external_accounts/{id}
  tags: Account, External, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountexternal-accountsid-post-openapi.md
- name: Stripe Get Accounts
  x-api-slug: stripe
  description: "Returns a list of accounts connected to your platform via Connect.
    If you\u2019re not a platform, the list is empty."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts
  tags: Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accounts-get-openapi.md
- name: Stripe Add Accounts
  x-api-slug: stripe
  description: Post Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts
  tags: Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accounts-post-openapi.md
- name: Stripe Delete Accounts Account
  x-api-slug: stripe
  description: With Connect, you may delete Custom accounts you manage.Custom accounts
    created using test-mode keys can be deleted at any time. Custom accounts created
    using live-mode keys may only be deleted once all balances are zero.If you are
    looking to close your own account, use the data tab in your account settings instead.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}
  tags: Accounts, Account
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccount-delete-openapi.md
- name: Stripe Get Accounts Account
  x-api-slug: stripe
  description: Retrieves the details of the account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}
  tags: Accounts, Account
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccount-get-openapi.md
- name: Stripe Add Accounts Account
  x-api-slug: stripe
  description: Updates a connected Express or Custom account by setting the values
    of the parameters passed. Any parameters not provided are left unchanged. To update
    your own account, use the Dashboard.Refer to our Connect documentation to learn
    more about updating accounts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}
  tags: Accounts, Account
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccount-post-openapi.md
- name: Stripe Add Accounts Account Bank Accounts
  x-api-slug: stripe
  description: Post Accounts, Account, Bank, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}/bank_accounts
  tags: Accounts, Account, Bank, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccountbank-accounts-post-openapi.md
- name: Stripe Delete Accounts Account Bank Accounts
  x-api-slug: stripe
  description: Delete Accounts, Account, Bank, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}/bank_accounts/{id}
  tags: Accounts, Account, Bank, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccountbank-accountsid-delete-openapi.md
- name: Stripe Get Accounts Account Bank Accounts
  x-api-slug: stripe
  description: Get Accounts, Account, Bank, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}/bank_accounts/{id}
  tags: Accounts, Account, Bank, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccountbank-accountsid-get-openapi.md
- name: Stripe Add Accounts Account Bank Accounts
  x-api-slug: stripe
  description: Updates the metadata of a bank account belonging to a Custom account,
    and optionally sets it as the default for its currency. Other bank account details
    are not editable by design.You can re-enable a disabled bank account by performing
    an update call without providing any arguments or changes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}/bank_accounts/{id}
  tags: Accounts, Account, Bank, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccountbank-accountsid-post-openapi.md
- name: Stripe Get Accounts Account External Accounts
  x-api-slug: stripe
  description: Get Accounts, Account, External, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}/external_accounts
  tags: Accounts, Account, External, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccountexternal-accounts-get-openapi.md
- name: Stripe Add Accounts Account External Accounts
  x-api-slug: stripe
  description: Post Accounts, Account, External, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}/external_accounts
  tags: Accounts, Account, External, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccountexternal-accounts-post-openapi.md
- name: Stripe Delete Accounts Account External Accounts
  x-api-slug: stripe
  description: Delete Accounts, Account, External, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}/external_accounts/{id}
  tags: Accounts, Account, External, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccountexternal-accountsid-delete-openapi.md
- name: Stripe Get Accounts Account External Accounts
  x-api-slug: stripe
  description: Get Accounts, Account, External, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}/external_accounts/{id}
  tags: Accounts, Account, External, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccountexternal-accountsid-get-openapi.md
- name: Stripe Add Accounts Account External Accounts
  x-api-slug: stripe
  description: Updates the metadata of a bank account belonging to a Custom account,
    and optionally sets it as the default for its currency. Other bank account details
    are not editable by design.You can re-enable a disabled bank account by performing
    an update call without providing any arguments or changes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}/external_accounts/{id}
  tags: Accounts, Account, External, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccountexternal-accountsid-post-openapi.md
- name: Stripe Add Accounts Account Login Links
  x-api-slug: stripe
  description: Creates a single-use login link for an Express account to access their
    Stripe dashboard.You may only create login links for Express accounts connected
    to your platform.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}/login_links
  tags: Accounts, Account, Login, Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccountlogin-links-post-openapi.md
- name: Stripe Put Accounts Account Logout
  x-api-slug: stripe
  description: Invalidates all sessions for a light account, for a platform to use
    during platform logout.You may only log out Express accounts connected to your
    platform.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}/logout
  tags: Accounts, Account, Logout
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccountlogout-put-openapi.md
- name: Stripe Add Accounts Account Reject
  x-api-slug: stripe
  description: With Connect, you may flag accounts as suspicious.Test-mode Custom
    and Express accounts can be rejected at any time. Accounts created using live-mode
    keys may only be rejected once all balances are zero.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///accounts/{account}/reject
  tags: Accounts, Account, Reject
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/accountsaccountreject-post-openapi.md
- name: Stripe Get Customers Customer Bank Accounts
  x-api-slug: stripe
  description: You can see a list of the bank accounts belonging to a Customer. Note
    that the 10 most recent sources are always available by default on the Customer.
    If you need more than those 10, you can use this API method and the limit and
    starting_after parameters to page through additional bank accounts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/bank_accounts
  tags: Customers, Customer, Bank, Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/customerscustomerbank-accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/customerscustomerbank-accounts-get-openapi.md
- name: Stripe Add Customers Customer Bank Accounts
  x-api-slug: stripe
  description: Post Customers, Customer, Bank, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/bank_accounts
  tags: Customers, Customer, Bank, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/customerscustomerbank-accounts-post-openapi.md
- name: Stripe Delete Customers Customer Bank Accounts
  x-api-slug: stripe
  description: Delete Customers, Customer, Bank, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/bank_accounts/{id}
  tags: Customers, Customer, Bank, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/customerscustomerbank-accountsid-delete-openapi.md
- name: Stripe Get Customers Customer Bank Accounts
  x-api-slug: stripe
  description: By default, you can see the 10 most recent sources stored on a Customer
    directly on the object, but you can also retrieve details about a specific bank
    account stored on the Stripe account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/bank_accounts/{id}
  tags: Customers, Customer, Bank, Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/customerscustomerbank-accountsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/customerscustomerbank-accountsid-get-openapi.md
- name: Stripe Add Customers Customer Bank Accounts
  x-api-slug: stripe
  description: Post Customers, Customer, Bank, Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/bank_accounts/{id}
  tags: Customers, Customer, Bank, Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/customerscustomerbank-accountsid-post-openapi.md
- name: Stripe Add Customers Customer Bank Accounts  Verify
  x-api-slug: stripe
  description: Post Customers, Customer, Bank, Accounts, , Verify
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/bank_accounts/{id}/verify
  tags: Customers, Customer, Bank, Accounts, , Verify
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/customerscustomerbank-accountsidverify-post-openapi.md
- name: Stripe
  x-api-slug: stripe
  description: Web and mobile payments, built for developers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/stripe/openapi.md
x-common:
- type: x-base
  url: https://api.stripe.com/
- type: x-blog
  url: https://stripe.com/blog
- type: x-blog-rss
  url: https://stripe.com/blog/feed.rss
- type: x-change-log
  url: https://stripe.com/docs/upgrades
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stripe
- type: x-crunchbase
  url: https://crunchbase.com/organization/stripe
- type: x-email
  url: info@stripe.com
- type: x-email
  url: privacy@stripe.com
- type: x-email
  url: atlas@stripe.com
- type: x-email
  url: notices@stripe.com
- type: x-email
  url: jane.diaz@stripe.com
- type: x-email
  url: nonprofit@stripe.com
- type: x-email
  url: support@stripe.com
- type: x-github
  url: https://github.com/stripe
- type: x-pricing
  url: https://stripe.com/us/pricing
- type: x-twitter
  url: https://twitter.com/stripe
- type: x-website
  url: https://stripe.com/
- type: x-website
  url: http://stripe.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---