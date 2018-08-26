{
  "info": {
    "name": "Steem broadcast_transaction",
    "_postman_id": "f13f7b3d-739d-44b3-84ca-e5727d0b3e51",
    "description": "broadcast_transaction",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Broadcast",
      "item": [
        {
          "id": "71f34d32-5e9b-4912-91f3-e4c2289bb570",
          "name": "broadcast-transaction",
          "request": {
            "url": "http://api.steemjs.com/broadcast_transaction?trx=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "broadcast_transaction"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33a16b64-8590-434d-b0fe-374957f8dde1"
            }
          ]
        },
        {
          "id": "fc29fae9-cdea-408a-8949-0117ad02f19d",
          "name": "broadcast-transaction-synchronous",
          "request": {
            "url": "http://api.steemjs.com/broadcast_transaction_synchronous?trx=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "broadcast_transaction_synchronous"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1607695a-96f1-46da-b8bd-80f4411e25c0"
            }
          ]
        },
        {
          "id": "bc989242-d46a-4118-93f1-3aec54a48550",
          "name": "broadcast-block",
          "request": {
            "url": "http://api.steemjs.com/broadcast_block?b=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "broadcast_block"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "856c014d-9b4a-430f-a809-7cd8205ed0bd"
            }
          ]
        }
      ]
    },
    {
      "name": "WARNING:",
      "item": [
        {
          "id": "1b0d1219-65c2-4ac1-91ef-a3cf969bd038",
          "name": "broadcast-transaction-with-callback",
          "request": {
            "url": "http://api.steemjs.com/broadcast_transaction_with_callback?confirmationCallback=%7B%7D&trx=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "broadcast_transaction_with_callback"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f54a43da-d104-4027-bcb8-a11dfde3054f"
            }
          ]
        }
      ]
    }
  ]
}