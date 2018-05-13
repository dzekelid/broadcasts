{
  "info": {
    "name": "Youtube Delete Live Broadcasts",
    "_postman_id": "83b87291-5e7a-4e0c-8d6e-2b265e964c02",
    "description": "Delete livebroadcasts",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "livebroadcasts",
      "item": [
        {
          "id": "fdb01dc5-9ad5-439e-8be4-5371ab0be979",
          "name": "deleteLivebroadcasts",
          "request": {
            "url": "http://www.googleapis.com/youtube/v1/liveBroadcasts?id=%7B%7D&onBehalfOfContentOwner=%7B%7D&onBehalfOfContentOwnerChannel=%7B%7D",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete livebroadcasts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5d73206-29da-4fd3-a8c2-07df8d65daf2"
            }
          ]
        }
      ]
    }
  ]
}