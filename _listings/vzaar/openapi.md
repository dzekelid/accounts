swagger: "2.0"
x-collection-name: Vzaar
x-complete: 1
info:
  title: VZaar API
  description: vzaar-is-an-online-video-hosting-service-with-fantastic-features-that-are-designed-for-business--deliver-to-mobile-or-the-web-straight-from-your-site-
  termsOfService: http://vzaar.com/policies
  version: v1
host: vzaar.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accounts/{account}.{format}:
    get:
      summary: Get Api Accounts Account
      description: 'nnThis API call returns the details and rights for each vzaar
        subscription account type along with its relevant metadata. This will show
        the details of the packages available here: http://vzaar.com/pricingnn'
      operationId: getApiAccountsAccount.Format
      x-api-path-slug: apiaccountsaccount-format-get
      parameters:
      - in: query
        name: account is the vzaar account type. This is an integer.
      responses:
        200:
          description: OK
      tags:
      - Api
      - Accounts
      - Account
      - Format