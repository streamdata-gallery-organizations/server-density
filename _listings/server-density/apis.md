---
name: Server Density
x-slug: server-density
description: SaaS infrastructure monitoring. Dashboards, graphs and alerts to help
  you improve performance and maintain uptime. Organizer of @humanops
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
x-kinRank: "7"
x-alexaRank: "209719"
tags: Server Density
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/apis.md
specificationVersion: "0.14"
apis:
- name: Alerts API Alerts?check_id={check_id}&amp;severity={severity}&amp;enabled={enabled}&amp;target_type={target_type}&amp;target_id={target_id}
  x-api-slug: alerts-api
  description: Gets alerts filtered by set of optional parameters.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: '://api.serverdensity.io.///alerts?check_id={check_id}&amp;severity={severity}&amp;enabled={enabled}&amp;target_type={target_type}&amp;target_id={target_id} '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertscheck-idcheck-idampseverityseverityampenabledenabledamptarget-typetarget-typeamptarget-idtarget-id-get-openapi.md
- name: Alerts API Alerts {alert_id}
  x-api-slug: alerts-api
  description: Gets alert by Id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: '://api.serverdensity.io.///alerts/{alert_id} '
  tags: Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsalert-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsalert-id-get-openapi.md
- name: Alerts API Alerts {alert_id}
  x-api-slug: alerts-api
  description: Updates alert.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: '://api.serverdensity.io.///alerts/{alert_id} '
  tags: Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsalert-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsalert-id-put-openapi.md
- name: Alerts API Alerts {alert_id}
  x-api-slug: alerts-api
  description: Deletes alert by Id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: '://api.serverdensity.io.///alerts/{alert_id} '
  tags: Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsalert-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsalert-id-delete-openapi.md
- name: Alerts API Alerts {alert_type}
  x-api-slug: alerts-api
  description: Creates a new alert.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: '://api.serverdensity.io.///alerts/{alert_type} '
  tags: Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsalert-type-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsalert-type-post-openapi.md
- name: Alerts API Alerts Recipients
  x-api-slug: alerts-api
  description: Gets a list of all alert recipient's targets that are visible to you
    as a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: '://api.serverdensity.io.///alerts/recipients '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsrecipients-get-openapi.md
- name: Alerts API Alerts Recipients {recipient_id}
  x-api-slug: alerts-api
  description: Gets a information about alert recipient's targets.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: '://api.serverdensity.io.///alerts/recipients/{recipient_id} '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsrecipientsrecipient-id-get-openapi.md
- name: Alerts API Alerts Recipient {recipient_id}
  x-api-slug: alerts-api
  description: Updates recipient along with sms and email targets associated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: '://api.serverdensity.io.///alerts/recipient/{recipient_id} '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsrecipientrecipient-id-put-openapi.md
- name: Alerts API Alerts Recipient
  x-api-slug: alerts-api
  description: Creates a new recipient with one sms and one email target associated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: '://api.serverdensity.io.///alerts/recipient '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsrecipient-post-openapi.md
- name: Alerts API Alerts Targets
  x-api-slug: alerts-api
  description: Gets a list of all alert targets that are visible to you as a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: '://api.serverdensity.io.///alerts/targets '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertstargets-get-openapi.md
- name: Alerts API Deleting an alert
  x-api-slug: alerts-api
  description: Deleting an alert
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///alerts/configs/alertId
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsconfigsalertid-delete-openapi.md
- name: Alerts API Listing alerts by subject
  x-api-slug: alerts-api
  description: Get a list of all configured alerts for a specific subject (device
    or service).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///alerts/configs/subjectId
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsconfigssubjectid-get-openapi.md
- name: Alerts API Triggered alerts
  x-api-slug: alerts-api
  description: Get a list of all triggered alerts on your account, per subject (device
    or service) or per alert config.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///alerts/triggered
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertstriggered-get-openapi.md
- name: Alerts API
  x-api-slug: alerts-api
  description: SaaS infrastructure monitoring. Dashboards, graphs and alerts to help
    you improve performance and maintain uptime. Organizer of @humanops
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io./
  tags: Server Density
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/openapi.md
- name: Dashboards API Deleting a dashboard
  x-api-slug: dashboards-api
  description: Deleting a dashboard.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///users/dashboards/dashboardId
  tags: Dashboards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/usersdashboardsdashboardid--openapi.md
- name: Dashboards API Duplicating a dashboard
  x-api-slug: dashboards-api
  description: Duplicating a dashboard.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///users/dashboards/duplicate/dasboardId
  tags: Dashboards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/usersdashboardsduplicatedasboardid--openapi.md
- name: Dashboards API
  x-api-slug: dashboards-api
  description: SaaS infrastructure monitoring. Dashboards, graphs and alerts to help
    you improve performance and maintain uptime. Organizer of @humanops
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io./
  tags: Server Density
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/openapi.md
- name: Devices API Creating a device
  x-api-slug: devices-api
  description: |-
    You can create new devices via the API, useful if you want to automatically provision new devices and start monitoring automatically.
    This API method is used by our Puppet manifest, Chef cookbook and installer shell script to automatically create devices during the agent installation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///inventory/devices
  tags: Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/inventorydevices--openapi.md
- name: Devices API Updating a device
  x-api-slug: devices-api
  description: Update a device and the associated metadata.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///inventory/devices/deviceId
  tags: Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/inventorydevicesdeviceid--openapi.md
- name: Devices API View device by agent key
  x-api-slug: devices-api
  description: View device by agent key.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///inventory/devices/agentKey/byagentkey
  tags: Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/inventorydevicesagentkeybyagentkey--openapi.md
- name: Devices API
  x-api-slug: devices-api
  description: SaaS infrastructure monitoring. Dashboards, graphs and alerts to help
    you improve performance and maintain uptime. Organizer of @humanops
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io./
  tags: Server Density
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/openapi.md
- name: History API Listing costs
  x-api-slug: history-api
  description: |-
    Get the alerts history items limited by the given filter. If configId filter is set, then the results contains all events for that alert configuration. In any other case, the results are aggregated by itemId and configId including the following derived values:

    duration the sum of event durations.
    triggeredCount the number of events for that alert in that item.
    cost the HumanOps cost in seconds. For more information please check our support docs


    When the query is aggregated, the non-derived fields are from the document whose startDate is the newest. In addition to this, an unique id is generated by concatenating the itemId and the configId.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///alerts/history/
  tags: Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertshistory--postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertshistory--openapi.md
- name: History API
  x-api-slug: history-api
  description: SaaS infrastructure monitoring. Dashboards, graphs and alerts to help
    you improve performance and maintain uptime. Organizer of @humanops
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io./
  tags: Server Density
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/openapi.md
- name: Postbacks API Creating a postback
  x-api-slug: postbacks-api
  description: You can use this method to post data back to Server Density without
    using the agent, for example using your own scripts or to integrate in something
    custom you are doing. You will still be restricted to posting back once per minute
    using this method, as you would be using the agent.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///alerts/postbacks/
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertspostbacks--openapi.md
- name: Postbacks API
  x-api-slug: postbacks-api
  description: SaaS infrastructure monitoring. Dashboards, graphs and alerts to help
    you improve performance and maintain uptime. Organizer of @humanops
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io./
  tags: Server Density
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/openapi.md
- name: Service Status API Listing service alert metrics
  x-api-slug: service-status-api
  description: Devices and services have different alert metrics which you can configure
    in the ui. The section correspond to the top-level of the alert metric whereas
    field corresponds to the subsection of the given section.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///alerts/service_alerts.json
  tags: Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsservice-alerts-json--postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/alertsservice-alerts-json--openapi.md
- name: Service Status API Location service status (last)
  x-api-slug: service-status-api
  description: Get the current results from a service check.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///service-monitor/last/serviceId
  tags: Service Monitor
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/servicemonitorlastserviceid--postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/servicemonitorlastserviceid--openapi.md
- name: Service Status API
  x-api-slug: service-status-api
  description: SaaS infrastructure monitoring. Dashboards, graphs and alerts to help
    you improve performance and maintain uptime. Organizer of @humanops
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io./
  tags: Server Density
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/openapi.md
- name: Tokens API Getting a token via the API
  x-api-slug: tokens-api
  description: |-
    If you need to generate tokens programmatically, you can request a token through the API with your username and password. All future requests can then be performed using the returned token.
    If the user generating the token has Multi Factor Authentication enabled, you cannot use this method and must create the token via the web UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///tokens
  tags: Tokens
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/tokens--openapi.md
- name: Tokens API Create a token
  x-api-slug: tokens-api
  description: Create a token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///tokens/
  tags: Tokens
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/tokens--openapi.md
- name: Tokens API Delete a token
  x-api-slug: tokens-api
  description: Delete a token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///tokens/tokenId
  tags: Tokens
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/tokenstokenid--openapi.md
- name: Tokens API
  x-api-slug: tokens-api
  description: SaaS infrastructure monitoring. Dashboards, graphs and alerts to help
    you improve performance and maintain uptime. Organizer of @humanops
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io./
  tags: Server Density
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/openapi.md
- name: Widgets API Deleting a widget
  x-api-slug: widgets-api
  description: Deleting a widget.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///users/widgets/widgetId
  tags: Widgets
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/userswidgetswidgetid--openapi.md
- name: Widgets API Duplicating a widget
  x-api-slug: widgets-api
  description: Duplicating a widget.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///users/widgets/duplicate/widgetId
  tags: Widgets
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/userswidgetsduplicatewidgetid--openapi.md
- name: Widgets API
  x-api-slug: widgets-api
  description: SaaS infrastructure monitoring. Dashboards, graphs and alerts to help
    you improve performance and maintain uptime. Organizer of @humanops
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io./
  tags: Server Density
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/server-density/master/_listings/server-density/openapi.md
x-common:
- type: x-website
  url: https://www.serverdensity.com
- type: x-blog
  url: http://blog.serverdensity.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/serverdensity
- type: x-crunchbase
  url: https://crunchbase.com/organization/server-density
- type: x-crunchbase
  url: http://www.crunchbase.com/company/server-density
- type: x-email
  url: hello@serverdensity.com
- type: x-github
  url: https://github.com/serverdensity
- type: x-linkedin
  url: https://www.linkedin.com/company/server-density
- type: x-twitter
  url: https://twitter.com/serverdensity
- type: x-website
  url: http://www.serverdensity.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---