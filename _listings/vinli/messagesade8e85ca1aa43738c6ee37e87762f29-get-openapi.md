---
swagger: "2.0"
x-collection-name: Vinli
x-complete: 0
info:
  title: Vinli Get a Specific Telemety Message
  description: Get a specific telemety message.
  version: 1.0.0
host: events.vin.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices/cf217c2d-df3c-41f7-b610-8bc3e11b4b79/messages:
    get:
      summary: List Telemetry Messages
      description: List telemetry messages.
      operationId: DevicesCf217c2dDf3c41f7B6108bc3e11b4b79MessagesGet
      x-api-path-slug: devicescf217c2ddf3c41f7b6108bc3e11b4b79messages-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - Telemetry
      - Messages
  /messages/ade8e85c-a1aa-4373-8c6e-e37e87762f29:
    get:
      summary: Get a Specific Telemety Message
      description: Get a specific telemety message.
      operationId: MessagesAde8e85cA1aa43738c6eE37e87762f29Get
      x-api-path-slug: messagesade8e85ca1aa43738c6ee37e87762f29-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Telemety
      - Message
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