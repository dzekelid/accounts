swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 1
info:
  title: AWS Auto Scaling API
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
      description: Describes the current Auto Scaling resource limits for your AWS
        account.
      operationId: describeAccountLimits
      x-api-path-slug: actiondescribeaccountlimits-get
      parameters:
      - in: query
        name: MaxNumberOfAutoScalingGroups
        description: The maximum number of groups allowed for your AWS account
        type: string
      - in: query
        name: MaxNumberOfLaunchConfigurations
        description: The maximum number of launch configurations allowed for your
          AWS account
        type: string
      - in: query
        name: NumberOfAutoScalingGroups
        description: The current number of groups for your AWS account
        type: string
      - in: query
        name: NumberOfLaunchConfigurations
        description: The current number of launch configurations for your AWS account
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Limits