{
  "info": {
    "name": "Steem broadcast_block",
    "_postman_id": "178e71d7-e60c-4dcc-bd07-592a352177fd",
    "description": "broadcast_block",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "f928597e-5a29-486e-abc4-ec330c7fb2c0",
          "name": "get-block",
          "request": {
            "url": "http://api.steemjs.com/get_block?blockNum=%7B%7D",
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
            "description": "get block"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0523db64-1d8e-4f7b-af95-e81a6d82947a"
            }
          ]
        },
        {
          "id": "4a0936fb-96c6-4fd8-82e5-f8f280bea8e8",
          "name": "get-block-header",
          "request": {
            "url": "http://api.steemjs.com/get_block_header?blockNum=%7B%7D",
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
            "description": "get block header"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da24ee4f-353e-4cbf-a1c6-fa5309a8b548"
            }
          ]
        },
        {
          "id": "51c6dc29-546e-4289-aa8a-d63fab3e0d31",
          "name": "get-ops-in-block",
          "request": {
            "url": "http://api.steemjs.com/get_ops_in_block?blockNum=%7B%7D&onlyVirtual=%7B%7D",
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
            "description": "get_ops_in_block"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d7cb08c-4074-4962-821d-2648a5d623ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Broadcast",
      "item": [
        {
          "id": "424e2159-5dfe-48aa-a043-3f47aa3e265f",
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
              "id": "0ea72ac3-3bdf-4276-9d6e-e8a2b61ce69a"
            }
          ]
        }
      ]
    }
  ]
}