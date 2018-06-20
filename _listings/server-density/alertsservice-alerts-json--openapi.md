---
swagger: "2.0"
x-collection-name: Server Density
x-complete: 0
info:
  title: Service Status API Listing service alert metrics
  description: Devices and services have different alert metrics which you can configure
    in the ui. The section correspond to the top-level of the alert metric whereas
    field corresponds to the subsection of the given section.
  version: 1.0.0
host: api.serverdensity.io.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /alerts/service_alerts.json:
    "":
      summary: Listing service alert metrics
      description: Devices and services have different alert metrics which you can
        configure in the ui. The section correspond to the top-level of the alert
        metric whereas field corresponds to the subsection of the given section.
      operationId: listing-service-alert-metrics
      x-api-path-slug: alertsservice-alerts-json-
      parameters:
      - in: query
        name: token
        description: Your API token
        type: string
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