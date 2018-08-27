{
  "info": {
    "name": "GitLab Get Internal Broadcast Message",
    "_postman_id": "5682bc48-cc0e-40f3-891c-1ff6d1609564",
    "description": "Get internal broadcast message.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Internal",
      "item": [
        {
          "id": "21de8a0e-8032-4ef6-a282-20ebae3b5a66",
          "name": "getV3InternalBroadcastMessage",
          "request": {
            "url": "http://localhost:3000/api/v3/internal/broadcast_message",
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
            "description": "Get internal broadcast message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "878c9086-4d8d-477f-b908-4a610a1ad0fa"
            }
          ]
        }
      ]
    }
  ]
}