---
swagger: "2.0"
x-collection-name: Server Density
x-complete: 0
info:
  title: Alerts API Alerts {alert_id}
  description: Updates alert.
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
      summary: Alerts?check_id={check_id}&amp;severity={severity}&amp;enabled={enabled}&amp;target_type={target_type}&amp;target_id={target_id}
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
      summary: Alerts {alert_id}
      description: Gets alert by Id.
      operationId: -alerts-alert-id-
      x-api-path-slug: alertsalert-id-get
      responses:
        200:
          description: OK
      tags:
      - Alerts
    ' put ':
      summary: Alerts {alert_id}
      description: Updates alert.
      operationId: -alerts-alert-id-
      x-api-path-slug: alertsalert-id-put
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