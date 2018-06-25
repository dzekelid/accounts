---
name: Azure Logic Apps
x-slug: azure-logic-apps
description: You can connect apps, data, and devices anywhere&mdash;on-premises or
  in the cloud&mdash;with our large ecosystem of software as a service (SaaS) and
  cloud-based connectors that includes Salesforce, Office 365, Twitter, Dropbox, Google
  services, and more. Its never been easier to access data and keep your disparate
  systems up-to-date, in real-time. New connectors are being added to the Azure Marketplace
  all of the time.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Accounts
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Logic Apps API Integration Accounts List By Subscription
  x-api-slug: azure-logic-apps-api
  description: Gets a list of integration accounts by subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Logic/integrationAccounts
  tags: Integration Accounts Subscription
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidprovidersmicrosoft-logicintegrationaccounts-get-openapi.md
- name: Azure Logic Apps API Integration Accounts List By Resource Group
  x-api-slug: azure-logic-apps-api
  description: Gets a list of integration accounts by resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts
  tags: Integration Accounts Resource Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccounts-get-openapi.md
- name: Azure Logic Apps API Integration Accounts Get
  x-api-slug: azure-logic-apps-api
  description: Gets an integration account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}
  tags: Integration Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountname-get-openapi.md
- name: Azure Logic Apps API Integration Accounts Create Or Update
  x-api-slug: azure-logic-apps-api
  description: Creates or updates an integration account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}
  tags: Integration Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountname-put-openapi.md
- name: Azure Logic Apps API Integration Accounts Update
  x-api-slug: azure-logic-apps-api
  description: Updates an integration account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}
  tags: Integration Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountname-patch-openapi.md
- name: Azure Logic Apps API Integration Accounts Delete
  x-api-slug: azure-logic-apps-api
  description: Deletes an integration account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}
  tags: Integration Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountname-delete-openapi.md
- name: Azure Logic Apps API Integration Accounts Get Callback Url
  x-api-slug: azure-logic-apps-api
  description: Gets the integration account callback URL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/listCallbackUrl
  tags: Integration Accounts Callback Url
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamelistcallbackurl-post-openapi.md
- name: Azure Logic Apps API Schemas List By Integration Accounts
  x-api-slug: azure-logic-apps-api
  description: Gets a list of integration account schemas.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/schemas
  tags: Schemas Integration Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnameschemas-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnameschemas-get-openapi.md
- name: Azure Logic Apps API Maps List By Integration Accounts
  x-api-slug: azure-logic-apps-api
  description: Gets a list of integration account maps.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/maps
  tags: Maps Integration Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamemaps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamemaps-get-openapi.md
- name: Azure Logic Apps API Partners List By Integration Accounts
  x-api-slug: azure-logic-apps-api
  description: Gets a list of integration account partners.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/partners
  tags: Partners Integration Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamepartners-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamepartners-get-openapi.md
- name: Azure Logic Apps API Agreements List By Integration Accounts
  x-api-slug: azure-logic-apps-api
  description: Gets a list of integration account agreements.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/agreements
  tags: Agreements Integration Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnameagreements-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnameagreements-get-openapi.md
- name: Azure Logic Apps API Certificates List By Integration Accounts
  x-api-slug: azure-logic-apps-api
  description: Gets a list of integration account certificates.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/certificates
  tags: Certificates Integration Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamecertificates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamecertificates-get-openapi.md
- name: Azure Logic Apps API Sessions List By Integration Accounts
  x-api-slug: azure-logic-apps-api
  description: Gets a list of integration account sessions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/sessions
  tags: Sessions Integration Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamesessions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamesessions-get-openapi.md
- name: Azure Logic Apps API
  x-api-slug: azure-logic-apps-api
  description: You can connect apps, data, and devices anywhere&mdash;on-premises
    or in the cloud&mdash;with our large ecosystem of software as a service (SaaS)
    and cloud-based connectors that includes Salesforce, Office 365, Twitter, Dropbox,
    Google services, and more. Its never been easier to access data and keep your
    disparate systems up-to-date, in real-time. New connectors are being added to
    the Azure Marketplace all of the time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com//
  tags: Accounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounts/master/_listings/azure-logic-apps/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/logic-apps/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/logic-apps/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/logic-apps/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/logic-apps/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---