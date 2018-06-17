---
name: Data2CRM
x-slug: data2crm
description: Data2CRM is all-in-one master touch instrument to create the perfect
  data environment for prosperous internal and external connections.Data2CRM.API,
  a Unified API Provider, to Connect Your Business Software with 17+ CRMs.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Accounts
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/data2crm/apis.md
specificationVersion: "0.14"
apis:
- name: Data2CRM GET for Account
  x-api-slug: data2crm
  description: Returns all accounts from the system
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//account
  tags: Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/data2crm/account-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/data2crm/account-get-openapi.md
- name: Data2CRM POST for Account
  x-api-slug: data2crm
  description: Add account into the system
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//account
  tags: Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/data2crm/account-post-openapi.md
- name: Data2CRM COUNT for Account
  x-api-slug: data2crm
  description: Count all accounts from the system
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//account/count
  tags: Accounts,Count
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/data2crm/accountcount-get-openapi.md
- name: Data2CRM DESCRIBE for Account
  x-api-slug: data2crm
  description: Returns describe for accounts
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//account/describe
  tags: Accounts,Describe
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/data2crm/accountdescribe-get-openapi.md
- name: Data2CRM DELETE for Account
  x-api-slug: data2crm
  description: Delete account information
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//account/{account_id}
  tags: Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/data2crm/accountaccount-id-delete-openapi.md
- name: Data2CRM GET for Account
  x-api-slug: data2crm
  description: Return account information
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//account/{account_id}
  tags: Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/data2crm/accountaccount-id-get-openapi.md
- name: Data2CRM PUT for Account
  x-api-slug: data2crm
  description: Update account information
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//account/{account_id}
  tags: Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/data2crm/accountaccount-id-put-openapi.md
- name: Data2CRM
  x-api-slug: data2crm
  description: Data2CRM is all-in-one master touch instrument to create the perfect
    data environment for prosperous internal and external connections.Data2CRM.API,
    a Unified API Provider, to Connect Your Business Software with 17+ CRMs.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1
  tags: Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/data2crm/openapi.md
x-common:
- type: x-twitter
  url: https://twitter.com/data2crm
- type: x-website
  url: http://data2crm.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---