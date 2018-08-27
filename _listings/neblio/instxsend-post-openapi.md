---
swagger: "2.0"
x-collection-name: Neblio
x-complete: 0
info:
  title: Neblio Broadcasts a signed raw transaction to the network (not NTP1 specific)
  description: Broadcasts a signed raw transaction to the network. If successful returns
    the txid of the broadcast trasnaction.
  version: 1.0.0
host: ntp1node.nebl.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ntp1/broadcast:
    post:
      summary: Broadcasts a signed raw transaction to the network
      description: Broadcasts a signed raw transaction to the network. If successful
        returns the txid of the broadcast trasnaction.
      operationId: broadcastTx
      x-api-path-slug: ntp1broadcast-post
      parameters:
      - in: body
        name: body
        description: Object representing a transaction to broadcast
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Broadcasts
      - Signed
      - Raw
      - Transaction
      - To
      - Network
  /ins/tx/send:
    post:
      summary: Broadcasts a signed raw transaction to the network (not NTP1 specific)
      description: Broadcasts a signed raw transaction to the network. If successful
        returns the txid of the broadcast trasnaction.
      operationId: sendTx
      x-api-path-slug: instxsend-post
      parameters:
      - in: body
        name: body
        description: Object representing a transaction to broadcast
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Broadcasts
      - Signed
      - Raw
      - Transaction
      - To
      - Network
      - (not
      - NTP1
      - Specific)
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