---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 0
info:
  title: Urban Airship Post Push Broadcast
  description: 'Sends a push message to all active APIDs (Broadcast). Important: The
    maximum message size is 1024 bytes. This is calculated as the UTF-8 lengths of
    alert and extra fields together.'
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /push/broadcast:
    post:
      summary: Post Push Broadcast
      description: 'Sends a push message to all active APIDs (Broadcast). Important:
        The maximum message size is 1024 bytes. This is calculated as the UTF-8 lengths
        of alert and extra fields together.'
      operationId: push.broadcast.post
      x-api-path-slug: pushbroadcast-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Push
      - Broadcast
  /airmail/send/broadcast:
    post:
      summary: Post Airmail Send Broadcast
      description: Sends a message to all users (broadcast). Only message is required.
        The message will be sent out to every registered user. Badge numbers will
        be handled automatically as long as the push key is present.
      operationId: airmail.send.broadcast.post
      x-api-path-slug: airmailsendbroadcast-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Airmail
      - Send
      - Broadcast
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