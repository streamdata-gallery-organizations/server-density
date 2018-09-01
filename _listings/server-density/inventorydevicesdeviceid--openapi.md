---
swagger: "2.0"
x-collection-name: Server Density
x-complete: 0
info:
  title: Devices API Updating a device
  description: Update a device and the associated metadata.
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
  /alerts/configs/subjectId:
    get:
      summary: Listing alerts by subject
      description: Get a list of all configured alerts for a specific subject (device
        or service).
      operationId: listing-alerts-by-subject
      x-api-path-slug: alertsconfigssubjectid-get
      parameters:
      - in: path
        name: subjectId
        description: The ID of the subject e
        type: string
      - in: path
        name: subjectType
        description: The type of the subject - device or service
        type: string
      - in: query
        name: subjectType
        description: The type of the subject - device or service
        type: string
      - in: path
        name: token
        description: Your API token
        type: string
      - in: query
        name: token
        description: Your API token
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
  /alerts/triggered:
    get:
      summary: Triggered Alerts
      description: Get a list of all triggered alerts on your account, per subject
        (device or service) or per alert config.
      operationId: triggered-alerts
      x-api-path-slug: alertstriggered-get
      parameters:
      - in: query
        name: closed
        description: Whether to filter by closed or open alerts - unset = all alerts,
          false = open alerts, true = closed alerts
        type: string
      - in: query
        name: filter
        description: You can provide a JSON encoded hash filter for the search that
          will return items that match the filter
        type: string
      - in: query
        name: subjectType
        description: The type of the subject - device, service, deviceGroup or serviceGroup
          if you also specify the subjectId as part of the URL (see examples below)
        type: string
      - in: query
        name: token
        description: Your API token
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
  /users/dashboards/dashboardId:
    "":
      summary: Deleting a dashboard
      description: Deleting a dashboard.
      operationId: deleting-a-dashboard
      x-api-path-slug: usersdashboardsdashboardid-
      parameters:
      - in: path
        name: dashboardId
        description: ID of the dashboard to delete
        type: string
      - in: path
        name: layout
        description: Dictionary with the ids of the widgets from this dashboard as
          keys
        type: string
      - in: body
        name: layout
        description: Dictionary with the ids of the widgets from this dashboard as
          keys
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: Name of the dashboard
        type: string
      - in: body
        name: name
        description: Name of the dashboard
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: token
        description: Your API token
        type: string
      - in: body
        name: token
        description: Your API token
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
      - Dashboards
  /users/dashboards/duplicate/dasboardId:
    "":
      summary: Duplicating a dashboard
      description: Duplicating a dashboard.
      operationId: duplicating-a-dashboard
      x-api-path-slug: usersdashboardsduplicatedasboardid-
      parameters:
      - in: body
        name: dashboardId
        description: ID of the dashboard to duplicate
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: new_name
        description: Name of the new, duplicated dashboard
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: token
        description: Your API token
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
      - Dashboards
  /inventory/devices:
    "":
      summary: Creating a device
      description: |-
        You can create new devices via the API, useful if you want to automatically provision new devices and start monitoring automatically.
        This API method is used by our Puppet manifest, Chef cookbook and installer shell script to automatically create devices during the agent installation.
      operationId: creating-a-device
      x-api-path-slug: inventorydevices-
      parameters:
      - in: body
        name: cpuCores
        description: Item???s number of cores
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: group
        description: Name of group
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: hostname
        description: Device???s hostname
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: installedRAM
        description: RAM installed
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: location
        description: A dictionary containing countryCode, text (which is the city)
          and countryName
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: name
        description: Name of device
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: os
        description: A dictionary containing code and name
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: privateIPs
        description: Item???s private IP addresses as a JSON encoded list
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: provider
        description: The provider dependent string that identifies this item
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: publicIPs
        description: Item???s public IP addresses as a JSON encoded list
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: swapSpace
        description: Item???s swap space
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: tags
        description: A JSON list of tag IDs
        schema:
          $ref: '#/definitions/holder'
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
      - Devices
  /inventory/devices/deviceId:
    "":
      summary: Updating a device
      description: Update a device and the associated metadata.
      operationId: updating-a-device
      x-api-path-slug: inventorydevicesdeviceid-
      parameters:
      - in: path
        name: cpuCores
        description: Item???s number of cores
        type: string
      - in: body
        name: cpuCores
        description: Item???s number of cores
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: deviceId
        description: The ID of the device to update
        type: string
      - in: path
        name: group
        description: Name of group
        type: string
      - in: body
        name: group
        description: Name of group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: hostname
        description: Item???s hostname
        type: string
      - in: body
        name: hostname
        description: Item???s hostname
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: installedRAM
        description: RAM installed
        type: string
      - in: body
        name: installedRAM
        description: RAM installed
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: Name of the device
        type: string
      - in: body
        name: name
        description: Name of the device
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: os
        description: Operating system that it runs
        type: string
      - in: body
        name: os
        description: Operating system that it runs
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: privateIPs
        description: Item???s private IP addresses as a JSON encoded list
        type: string
      - in: body
        name: privateIPs
        description: Item???s private IP addresses as a JSON encoded list
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: provider
        description: Provider where the item is hosted
        type: string
      - in: body
        name: provider
        description: Provider where the item is hosted
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: providerId
        description: The provider dependent string that identifies this item
        type: string
      - in: body
        name: providerId
        description: The provider dependent string that identifies this item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: publicIPs
        description: Item???s public IP addresss as a JSON encoded list
        type: string
      - in: body
        name: publicIPs
        description: Item???s public IP addresss as a JSON encoded list
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: swapSpace
        description: Item???s swap space
        type: string
      - in: body
        name: swapSpace
        description: Item???s swap space
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tags
        description: A JSON list of tag IDs
        type: string
      - in: body
        name: tags
        description: A JSON list of tag IDs
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: token
        description: Your API token
        type: string
      - in: body
        name: token
        description: Your API token
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
      - Devices
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