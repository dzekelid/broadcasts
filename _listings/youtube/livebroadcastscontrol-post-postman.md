{
  "info": {
    "name": "Youtube Add Live Broadcasts Control",
    "_postman_id": "c7589168-c518-4326-87cb-596bfab17db7",
    "description": "Controls the settings for a slate that can be displayed in the broadcast stream.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "livebroadcasts",
      "item": [
        {
          "id": "796296eb-d2a4-4bc0-a757-fa154e9ac8e7",
          "name": "postLivebroadcastsControl",
          "request": {
            "url": "http://www.googleapis.com/youtube/v1/liveBroadcasts/control?displaySlate=%7B%7D&id=%7B%7D&offsetTimeMs=%7B%7D&onBehalfOfContentOwner=%7B%7D&onBehalfOfContentOwnerChannel=%7B%7D&part=%7B%7D&walltime=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Controls the settings for a slate that can be displayed in the broadcast stream"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86e5e943-338a-429e-a4cb-39a4db76b3fa"
            }
          ]
        }
      ]
    }
  ]
}