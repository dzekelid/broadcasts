swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 1
info:
  title: Urban Airship
  description: the-urban-airships-api-powers-mobile-applications-with-push-rich-push-inapp-purchases-and-subscription-services-
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