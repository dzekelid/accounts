---
name: Standard Chartered
x-slug: standard-chartered
description: Standard Chartered PLC is a British multinational banking and financial
  services company headquartered in London, England. It operates a network of more
  than 1,200 branches and outlets (including subsidiaries, associates and joint ventures)
  across more than 70 countries and employs around 87,000 people. It is a universal
  bank with operations in consumer, corporate and institutional banking, and treasury
  services. Despite its UK base, it does not conduct retail banking in the UK, and
  around 90% of its profits come from Asia, Africa and the Middle East.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/standard-charter.png
x-kinRank: "7"
x-alexaRank: "4658"
tags: Accounts
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/standard-chartered/apis.md
specificationVersion: "0.14"
apis:
- name: Standard Chartered Accounts
  x-api-slug: standard-chartered
  description: "The \u201CGetAccountBalance\u201D API upon successful user authentication
    and entitlement checks will return the various types of \u201CAccount Balances\u201D
    applicable for the specified Account Number."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/standard-charter.png
  humanURL: https://developer.sc.com
  baseURL: https://developer.sc.com////cib/service/s2b/api/v1/banks/scb/accounts/{accountId}/{viewId}/account
  tags: Cib, Service, S2b, Api, V1, Banks, Scb, Accounts, Account, View, Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/standard-chartered/cibservices2bapiv1banksscbaccountsaccountidviewidaccount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/standard-chartered/cibservices2bapiv1banksscbaccountsaccountidviewidaccount-get-openapi.md
- name: Standard Chartered Finds all support transaction types for a given account
  x-api-slug: standard-chartered
  description: "The \u201CGetTransactionTypes\u201D API upon successful user authentication
    and entitlement checks will return the supported transaction types for the specified
    account"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/standard-charter.png
  humanURL: https://developer.sc.com
  baseURL: https://developer.sc.com////cib/service/s2b/api/v1/banks/scb/accounts/{accountId}/{viewId}/transaction-request-types
  tags: Cib, Service, S2b, Api, V1, Banks, Scb, Accounts, Account, View, Transaction,
    Request, Types
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/standard-chartered/cibservices2bapiv1banksscbaccountsaccountidviewidtransactionrequesttypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/standard-chartered/cibservices2bapiv1banksscbaccountsaccountidviewidtransactionrequesttypes-get-openapi.md
- name: Standard Chartered Account Details & Balances
  x-api-slug: standard-chartered
  description: List available bank accounts
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/standard-charter.png
  humanURL: https://developer.sc.com
  baseURL: https://developer.sc.com////cib/service/s2b/api/v1/banks/scb/accounts/{viewId}/accounts
  tags: Cib, Service, S2b, Api, V1, Banks, Scb, Accounts, View, Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/standard-chartered/cibservices2bapiv1banksscbaccountsviewidaccounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/standard-chartered/cibservices2bapiv1banksscbaccountsviewidaccounts-get-openapi.md
- name: Standard Chartered
  x-api-slug: standard-chartered
  description: Standard Chartered PLC is a British multinational banking and financial
    services company headquartered in London, England. It operates a network of more
    than 1,200 branches and outlets (including subsidiaries, associates and joint
    ventures) across more than 70 countries and employs around 87,000 people. It is
    a universal bank with operations in consumer, corporate and institutional banking,
    and treasury services. Despite its UK base, it does not conduct retail banking
    in the UK, and around 90% of its profits come from Asia, Africa and the Middle
    East.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/standard-charter.png
  humanURL: https://developer.sc.com
  baseURL: https://developer.sc.com//
  tags: Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/standard-chartered/openapi.md
x-common:
- type: x-accessibility
  url: https://developer.sc.com/cib/#/accessibility
- type: x-applications
  url: https://developer.sc.com/cib/#/showcases
- type: x-crunchbase
  url: https://crunchbase.com/organization/standard-chartered-bank
- type: x-documentation
  url: https://developer.sc.com/cib/#/api-documentation/3
- type: x-privacy-policy
  url: https://developer.sc.com/cib/#/privacy
- type: x-terms-of-service
  url: https://developer.sc.com/cib/#/legal-notice
- type: x-twitter
  url: https://twitter.com/StanChart
- type: x-website
  url: https://developer.sc.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---