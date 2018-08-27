swagger: "2.0"
x-collection-name: Steem
x-complete: 1
info:
  title: Interactive Steem API
  description: interactive-steem-api-lets-you-interact-with-steem-blockchain-and-make-a-request-get-output-and-start-implementing-new-apps-apis-have-default-parameters-set-to-get-you-started-and-see-how-request-works--api-list-is-compiled-from-steem-githubhttpsgithub-comsteemitsteem-1httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappapi-hpp-and-2httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappdatabase-api-hpp--if-you-want-to-contribute-documenting-detail-of-properties-and-output-contact-goodkarmahttpssteemit-chatdirectgoodkarma--you-can-also-check-full-list-here-steem-jshttpssteemjs-com
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /broadcast_transaction:
    get:
      summary: broadcast_transaction
      description: broadcast_transaction
      operationId: broadcast-transaction
      x-api-path-slug: broadcast-transaction-get
      parameters:
      - in: query
        name: trx
        description: transaction
      responses:
        200:
          description: OK
      tags:
      - Broadcast
      - Transaction
  /broadcast_transaction_synchronous:
    get:
      summary: broadcast_transaction_synchronous
      description: broadcast_transaction_synchronous
      operationId: broadcast-transaction-synchronous
      x-api-path-slug: broadcast-transaction-synchronous-get
      parameters:
      - in: query
        name: trx
        description: transaction
      responses:
        200:
          description: OK
      tags:
      - Broadcast
      - Transaction
      - Synchronous
  /broadcast_block:
    get:
      summary: broadcast_block
      description: broadcast_block
      operationId: broadcast-block
      x-api-path-slug: broadcast-block-get
      parameters:
      - in: query
        name: b
        description: block
      responses:
        200:
          description: OK
      tags:
      - Broadcast
      - Block
  /broadcast_transaction_with_callback:
    get:
      summary: 'WARNING: can only be used in Steem node or in scripts broadcast_transaction_with_callback'
      description: broadcast_transaction_with_callback
      operationId: broadcast-transaction-with-callback
      x-api-path-slug: broadcast-transaction-with-callback-get
      parameters:
      - in: query
        name: confirmationCallback
        description: confirmationCallback function
      - in: query
        name: trx
        description: transaction
      responses:
        200:
          description: OK
      tags:
      - 'WARNING:'
      - Can
      - Only
      - Be
      - Used
      - In
      - Steem
      - Node
      - In
      - Scripts
      - Broadcast
      - Transaction
      - Callback