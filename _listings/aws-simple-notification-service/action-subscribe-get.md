---
swagger: "2.0"
info:
  title: AWS Simple Notification Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=Subscribe&k=1:
    get:
      summary: ' Subscribe '
      description: Prepares to subscribe an endpoint by sending the endpoint a confirmation
        message
      operationId: subscribe
      parameters:
      - in: query
        name: Endpoint
        description: The endpoint that you want to receive notifications
        type: string
      - in: query
        name: Protocol
        description: The protocol you want to use
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic you want to subscribe to
        type: string
      responses:
        200:
          description: OK
      tags:
      - endpoints
definitions: []
x-collection-name: AWS Simple Notification Service
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