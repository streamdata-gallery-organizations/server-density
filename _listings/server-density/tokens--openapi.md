---
swagger: "2.0"
x-collection-name: Server Density
x-complete: 0
info:
  title: Tokens API Create a token
  description: Create a token.
  version: 1.0.0
host: api.serverdensity.io.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tokens:
    "":
      summary: Getting a token via the API
      description: |-
        If you need to generate tokens programmatically, you can request a token through the API with your username and password. All future requests can then be performed using the returned token.
        If the user generating the token has Multi Factor Authentication enabled, you cannot use this method and must create the token via the web UI.
      operationId: getting-a-token-via-the-api
      x-api-path-slug: tokens-
      parameters:
      - in: body
        name: accountName
        description: The Server Density account that the user is a member of e
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: password
        description: The token will be associated with this password
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: tokenName
        description: The name of the token, displayed in the UI
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: username
        description: The token will be associated with this username
        schema:
          $ref: '#/definitions/holder'
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Tokens
  /tokens/:
    "":
      summary: Create a token
      description: Create a token.
      operationId: create-a-token
      x-api-path-slug: tokens-
      parameters:
      - in: query
        name: token
        description: Your API token
        type: string
      - in: query
        name: tokenName
        description: The name of your new token
        type: string
      - in: body
        name: tokenName
        description: The name of your new token
        schema:
          $ref: '#/definitions/holder'
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Tokens
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