{
  "info": {
    "name": "Steem broadcast_transaction_synchronous",
    "_postman_id": "140694ea-4665-490e-95a0-54f4bbe5f59b",
    "description": "broadcast_transaction_synchronous",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Broadcast",
      "item": [
        {
          "id": "745b5018-02dc-4611-9642-364c28de2d67",
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
              "id": "540e2de6-2980-4405-b423-530bad41f58a"
            }
          ]
        },
        {
          "id": "9181c78b-215b-4125-8546-ce084c30221f",
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
              "id": "dcfcf497-aedf-42b3-ad90-8b3095d207f4"
            }
          ]
        },
        {
          "id": "9b5c38ba-c4d5-46f2-b867-13fb6eaa874f",
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
              "id": "c33a619d-fe64-4df6-8dde-1e51fefaec36"
            }
          ]
        }
      ]
    },
    {
      "name": "WARNING:",
      "item": [
        {
          "id": "172cdcc8-0c2d-4c27-8dc0-acc2a03e6887",
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
              "id": "03f882ea-5f79-410c-8e0c-e432b51997bb"
            }
          ]
        }
      ]
    }
  ]
}