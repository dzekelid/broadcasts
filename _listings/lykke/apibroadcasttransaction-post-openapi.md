---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Add API Broadcasttransaction
  version: 1.0.0
  description: Add api broadcasttransaction.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/BitcoinCash/broadcast:
    post:
      summary: Add API Bitcoincash Broadcast
      description: Add api bitcoincash broadcast.
      operationId: ApiBitcoinCashBroadcastPost
      x-api-path-slug: apibitcoincashbroadcast-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bitcoincash
      - Broadcast
  /api/BroadcastTransaction:
    post:
      summary: Add API Broadcasttransaction
      description: Add api broadcasttransaction.
      operationId: ApiBroadcastTransactionPost
      x-api-path-slug: apibroadcasttransaction-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: transaction
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Broadcasttransaction
  /api/Ethereum/privateWallet/broadcastTransaction:
    post:
      summary: Add API Ethereum Privatewallet Broadcasttransaction
      description: Add api ethereum privatewallet broadcasttransaction.
      operationId: ApiEthereumPrivateWalletBroadcastTransactionPost
      x-api-path-slug: apiethereumprivatewalletbroadcasttransaction-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: transaction
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Privatewallet
      - Broadcasttransaction
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