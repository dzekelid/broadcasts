---
swagger: "2.0"
x-collection-name: Neblio
x-complete: 1
info:
  title: Neblio REST API Suite
  description: apis-for-interacting-with-ntp1-tokens--the-neblio-blockchain
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
  /testnet/ins/tx/send:
    post:
      summary: Broadcasts a signed raw transaction to the network (not NTP1 specific)
      description: Broadcasts a signed raw transaction to the network. If successful
        returns the txid of the broadcast trasnaction.
      operationId: testnet_sendTx
      x-api-path-slug: testnetinstxsend-post
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
  /testnet/ntp1/broadcast:
    post:
      summary: Broadcasts a signed raw transaction to the network
      description: Broadcasts a signed raw transaction to the network. If successful
        returns the txid of the broadcast trasnaction.
      operationId: testnet_broadcastTx
      x-api-path-slug: testnetntp1broadcast-post
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
---