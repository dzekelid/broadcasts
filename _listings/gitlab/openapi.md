swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/internal/broadcast_message:
    get:
      summary: Get Internal Broadcast Message
      description: Get internal broadcast message.
      operationId: getV3InternalBroadcastMessage
      x-api-path-slug: v3internalbroadcast-message-get
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Broadcast
      - Message