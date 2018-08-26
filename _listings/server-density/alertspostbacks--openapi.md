---
swagger: "2.0"
x-collection-name: Server Density
x-complete: 0
info:
  title: Postbacks API Creating a postback
  description: You can use this method to post data back to Server Density without
    using the agent, for example using your own scripts or to integrate in something
    custom you are doing. You will still be restricted to posting back once per minute
    using this method, as you would be using the agent.
  version: 1.0.0
host: api.serverdensity.io.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /alerts/postbacks/:
    "":
      summary: Creating a postback
      description: You can use this method to post data back to Server Density without
        using the agent, for example using your own scripts or to integrate in something
        custom you are doing. You will still be restricted to posting back once per
        minute using this method, as you would be using the agent.
      operationId: creating-a-postback
      x-api-path-slug: alertspostbacks-
      parameters:
      - in: body
        name: hash
        description: An md5 hash of the JSON encoded payload, used for error checking
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: payload
        description: The payload you want to post back to us
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: token
        description: Your API token
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: X-Forwarded-Host
        description: Set this to your Server Density account url, e
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
      - Alerts
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