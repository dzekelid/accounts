---
name: Google Content API for Shopping
x-slug: google-content-api-for-shopping
description: 'API allowing retailers to manage their product feed content programmatically.
  Providing item-level data quality information: See if an item was disapproved because
  a landing page URL isn&rsquo;t working on a mobile device or if unique product identifiers
  are inaccurate. Faster pricing and availability updates: Ensure customers have the
  latest price-points and know what&rsquo;s in-stock before they click through to
  your site. More integration options: The newer API supports a broader choice of
  programming languages and data formats.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
x-kinRank: "9"
x-alexaRank: "0"
tags: Accounts
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/google-content-api-for-shopping/apis.md
specificationVersion: "0.14"
apis:
- name: Google Content API for Shopping API Get Accounts
  x-api-slug: google-content-api-for-shopping-api
  description: Lists the sub-accounts in your Merchant Center account. This method
    can only be called for multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2//{merchantId}/accounts
  tags: Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/google-content-api-for-shopping/merchantidaccounts-get-openapi.md
- name: Google Content API for Shopping API Create Accounts
  x-api-slug: google-content-api-for-shopping-api
  description: Creates a Merchant Center sub-account. This method can only be called
    for multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2//{merchantId}/accounts
  tags: Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/google-content-api-for-shopping/merchantidaccounts-post-openapi.md
- name: Google Content API for Shopping API
  x-api-slug: google-content-api-for-shopping-api
  description: 'API allowing retailers to manage their product feed content programmatically.
    Providing item-level data quality information: See if an item was disapproved
    because a landing page URL isn&rsquo;t working on a mobile device or if unique
    product identifiers are inaccurate. Faster pricing and availability updates: Ensure
    customers have the latest price-points and know what&rsquo;s in-stock before they
    click through to your site. More integration options: The newer API supports a
    broader choice of programming languages and data formats.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/google-content-api-for-shopping/openapi.md
x-common:
- type: x-best-practices
  url: https://developers.google.com/shopping-content/v2/best-practices
- type: x-code
  url: https://developers.google.com/shopping-content/v2/libraries
- type: x-testing
  url: https://developers.google.com/shopping-content/v2/how-tos/testing
- type: x-website
  url: https://developers.google.com/shopping-content/v2/quickstart
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---