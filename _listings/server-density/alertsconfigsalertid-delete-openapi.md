---
swagger: "2.0"
x-collection-name: Server Density
x-complete: 0
info:
  title: Alerts API Deleting an alert
  description: Deleting an alert
  version: 1.0.0
host: api.serverdensity.io.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? '/alerts?check_id={check_id}&amp;severity={severity}&amp;enabled={enabled}&amp;target_type={target_type}&amp;target_id={target_id} '
  : ' get ':
      summary: Alerts
      description: Gets alerts filtered by set of optional parameters.
      operationId: -alertscheck-idcheck-idampseverityseverityampenabledenabledamptarget-typetarget-typeamptarget-idtarg
      x-api-path-slug: alertscheck-idcheck-idampseverityseverityampenabledenabledamptarget-typetarget-typeamptarget-idtarget-id-get
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/{alert_id} ':
    ' get ':
      summary: Alerts
      description: Gets alert by Id.
      operationId: -alerts-alert-id-
      x-api-path-slug: alertsalert-id-get
      responses:
        200:
          description: OK
      tags:
      - Alerts
    ' put ':
      summary: Alerts
      description: Updates alert.
      operationId: -alerts-alert-id-
      x-api-path-slug: alertsalert-id-put
      responses:
        200:
          description: OK
      tags:
      - Alerts
    ' delete ':
      summary: Alerts
      description: Deletes alert by Id.
      operationId: -alerts-alert-id-
      x-api-path-slug: alertsalert-id-delete
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/{alert_type} ':
    ' post ':
      summary: Alerts
      description: Creates a new alert.
      operationId: -alerts-alert-type-
      x-api-path-slug: alertsalert-type-post
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/recipients ':
    ' get ':
      summary: Alerts Recipients
      description: Gets a list of all alert recipient's targets that are visible to
        you as a customer.
      operationId: -alerts-recipients-
      x-api-path-slug: alertsrecipients-get
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/recipients/{recipient_id} ':
    ' get ':
      summary: Alerts Recipients
      description: Gets a information about alert recipient's targets.
      operationId: -alerts-recipients-recipient-id-
      x-api-path-slug: alertsrecipientsrecipient-id-get
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/recipient/{recipient_id} ':
    ' put ':
      summary: Alerts Recipient
      description: Updates recipient along with sms and email targets associated.
      operationId: -alerts-recipient-recipient-id-
      x-api-path-slug: alertsrecipientrecipient-id-put
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/recipient ':
    ' post ':
      summary: Alerts Recipient
      description: Creates a new recipient with one sms and one email target associated.
      operationId: -alerts-recipient-
      x-api-path-slug: alertsrecipient-post
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/targets ':
    ' get ':
      summary: Alerts Targets
      description: Gets a list of all alert targets that are visible to you as a customer.
      operationId: -alerts-targets-
      x-api-path-slug: alertstargets-get
      responses:
        200:
          description: OK
      tags:
      - Alerts
  /alerts/configs/alertId:
    delete:
      summary: Deleting an alert
      description: Deleting an alert
      operationId: deleting-an-alert
      x-api-path-slug: alertsconfigsalertid-delete
      parameters:
      - in: path
        name: alertId
        description: The ID of the alert to be deleted
        type: string
      - in: path
        name: token
        description: Your API token
        type: string
      - in: body
        name: token
        description: Your API token
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: token
        description: Your API token
        type: string
      responses:
        200:
          description: OK
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