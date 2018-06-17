---
swagger: "2.0"
x-collection-name: Open Science Framework
x-complete: 0
info:
  title: Open Science Framework List all addon accounts
  description: |-
    A paginated list of addon accounts authorized by this user.

    #### Permissions

    Addon accounts are visible only to the user that authorized the account.

    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of at most 10 addon account objects. Each resource in the array is a separate  addon account object and contains the full representation of the addon account.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
  contact:
    name: OSF
    url: https://osf.io/support
    email: support@osf.io
  version: "2.0"
host: test-api.osf.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/addons/{provider}/accounts/:
    get:
      summary: List all addon accounts
      description: |-
        A paginated list of addon accounts authorized by this user.

        #### Permissions

        Addon accounts are visible only to the user that authorized the account.

        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of at most 10 addon account objects. Each resource in the array is a separate  addon account object and contains the full representation of the addon account.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
      operationId: Users_addon_accounts_list
      x-api-path-slug: usersuser-idaddonsprovideraccounts-get
      parameters:
      - in: path
        name: provider
        description: The unique identifier of the addon provider
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Addons
      - Provider
      - Accounts
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---