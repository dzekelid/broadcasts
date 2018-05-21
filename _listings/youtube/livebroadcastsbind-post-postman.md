{
  "info": {
    "name": "Youtube Add Live Broadcasts Bind",
    "_postman_id": "50aba94e-f209-4816-8b73-6330992d52f9",
    "description": "Binds a YouTube broadcast to a stream or removes an existing binding between a broadcast and a stream. A broadcast can only be bound to one video stream, though a video stream may be bound to more than one broadcast.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "livebroadcasts",
      "item": [
        {
          "id": "ca44a2db-e917-42ae-b1b2-7cbd77b2968e",
          "name": "postLivebroadcastsBind",
          "request": {
            "url": "http://www.googleapis.com/youtube/v1/liveBroadcasts/bind?id=%7B%7D&onBehalfOfContentOwner=%7B%7D&onBehalfOfContentOwnerChannel=%7B%7D&part=%7B%7D&streamId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Binds a YouTube broadcast to a stream or removes an existing binding between a broadcast and a stream"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8558e054-9049-4247-80c8-5ed0bffa3d42"
            }
          ]
        }
      ]
    }
  ]
}