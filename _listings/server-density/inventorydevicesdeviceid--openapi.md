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
        description: Items number of cores
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: group
        description: Name of group
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: hostname
        description: Devices hostname
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
        description: Items private IP addresses as a JSON encoded list
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: provider
        description: The provider dependent string that identifies this item
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: publicIPs
        description: Items public IP addresses as a JSON encoded list
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: swapSpace
        description: Items swap space
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
        description: Items number of cores
        type: string
      - in: body
        name: cpuCores
        description: Items number of cores
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
        description: Items hostname
        type: string
      - in: body
        name: hostname
        description: Items hostname
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
        description: Items private IP addresses as a JSON encoded list
        type: string
      - in: body
        name: privateIPs
        description: Items private IP addresses as a JSON encoded list
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
        description: Items public IP addresss as a JSON encoded list
        type: string
      - in: body
        name: publicIPs
        description: Items public IP addresss as a JSON encoded list
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: swapSpace
        description: Items swap space
        type: string
      - in: body
        name: swapSpace
        description: Items swap space
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