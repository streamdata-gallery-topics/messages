---
swagger: "2.0"
x-collection-name: Flowroute
x-complete: 0
info:
  title: FlowRoute API List Inbound Routes
  description: Returns a list of your inbound routes. From the list, you can then
    select routes to use as the primary and failover routes for a phone number, which
    you can do via "Update Primary Voice Route for a Phone Number" and "Update Failover
    Voice Route for a Phone Number".
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2.1/messages:
    get:
      summary: Look Up a Set of Messages
      description: Retrieves a list of Message Detail Records (MDRs) within a specified
        date range. Date and time is based on Coordinated Universal Time (UTC).
      operationId: retrieves-a-list-of-message-detail-records-mdrs-within-a-specified-date-range-date-and-time-is-based
      x-api-path-slug: v2-1messages-get
      parameters:
      - in: query
        name: end_date
        description: The ending date and time, in UTC, on which to perform an MDR
          search
      - in: query
        name: limit
        description: The number of MDRs to retrieve at one time
      - in: query
        name: offset
        description: The number of MDRs to skip when performing a query
      - in: query
        name: start_date
        description: The beginning date and time, in UTC, on which to perform an MDR
          search
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Look
      - Up
      - Set
      - Of
      - Messages
    post:
      summary: Send a Message
      description: Sends an SMS or MMS from a Flowroute long code or toll-free phone
        number to another valid phone number.
      operationId: sends-an-sms-or-mms-from-a-flowroute-long-code-or-tollfree-phone-number-to-another-valid-phone-numbe
      x-api-path-slug: v2-1messages-post
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Send
      - Message
  /v2.1/messages/{id}:
    get:
      summary: Look Up a Message Detail Record
      description: Searches for a specific message record ID and returns a Message
        Detail Record (in MDR2 format).
      operationId: searches-for-a-specific-message-record-id-and-returns-a-message-detail-record-in-mdr2-format
      x-api-path-slug: v2-1messagesid-get
      parameters:
      - in: path
        name: id
        description: The unique message detail record identifier (MDR ID) of any message
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Look
      - Up
      - Message
      - Detail
      - Record
  /v2/routes:
    get:
      summary: List Inbound Routes
      description: Returns a list of your inbound routes. From the list, you can then
        select routes to use as the primary and failover routes for a phone number,
        which you can do via "Update Primary Voice Route for a Phone Number" and "Update
        Failover Voice Route for a Phone Number".
      operationId: returns-a-list-of-your-inbound-routes-from-the-list-you-can-then-select-routes-to-use-as-the-primary
      x-api-path-slug: v2routes-get
      parameters:
      - in: query
        name: limit
        description: Limits the number of routes to retrieve
      - in: query
        name: offset
        description: Offsets the list of routes by your specified value
      - in: query
        name: route_type
        description: Restricts the results to inbound routes with your specified route
          type
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - List
      - Inbound
      - Routes
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