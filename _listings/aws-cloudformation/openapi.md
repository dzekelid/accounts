---
swagger: "2.0"
x-collection-name: AWS CloudFormation
x-complete: 1
info:
  title: AWS CloudFormation API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeAccountLimits:
    get:
      summary: Describe Account Limits
      description: Retrieves your account's AWS CloudFormation limits, such as the
        maximum number of stacks that you can create in your account.
      operationId: describeAccountLimits
      x-api-path-slug: actiondescribeaccountlimits-get
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of limits that you want
          to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Limits
---