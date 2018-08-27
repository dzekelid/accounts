swagger: "2.0"
x-collection-name: Flowroute
x-complete: 1
info:
  title: Flowroute APIs
  description: the-flowroute-apis-are-organized-around-rest--our-apis-have-resourceoriented-urls-support-http-verbs-and-respond-with-http-status-codes--all-api-requests-and-responses-including-errors-will-be-represented-as-json-objects--you-can-use-the-flowroute-apis-to-manage-your-flowroute-phone-numbers-including-setting-primary-and-failover-routes-for-inbound-calls-and-sending-text-messages-sms-and-mms-using-longcode-or-tollfree-numbers-in-your-account-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/numbers:
    get:
      summary: Account Phone Numbers
      description: Returns a list of all phone numbers currently on your Flowroute
        account. The response includes details such as the phone number's rate center,
        state, number type, and whether CNAM Lookup is enabled for that number.
      operationId: returns-a-list-of-all-phone-numbers-currently-on-your-flowroute-account-the-response-includes-detail
      x-api-path-slug: v2numbers-get
      parameters:
      - in: query
        name: contains
        description: Retrieves phone numbers containing the specified value
      - in: query
        name: ends_with
        description: Retrieves phone numbers that end with the specified value
      - in: query
        name: limit
        description: Limits the number of items to retrieve
      - in: query
        name: offset
        description: Offsets the list of phone numbers by your specified value
      - in: query
        name: starts_with
        description: Retrieves phone numbers that start with the specified value
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Account
      - Phone
      - Numbers