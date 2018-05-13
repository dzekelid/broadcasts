{
  "info": {
    "name": "Youtube Get Live Broadcasts",
    "_postman_id": "22a5ace1-2268-41ee-9811-a8853beec023",
    "description": "Returns a list of YouTube broadcasts that match the API request parameters.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "livebroadcasts",
      "item": [
        {
          "id": "a00cea24-d769-4017-87a1-d3b31b14821d",
          "name": "getLivebroadcasts",
          "request": {
            "url": "http://www.googleapis.com/youtube/v1/liveBroadcasts?broadcastStatus=%7B%7D&broadcastType=%7B%7D&id=%7B%7D&maxResults=%7B%7D&mine=%7B%7D&onBehalfOfContentOwner=%7B%7D&onBehalfOfContentOwnerChannel=%7B%7D&pageToken=%7B%7D&part=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of YouTube broadcasts that match the API request parameters"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9bb247d-dda2-4a90-8bc5-176922462d18"
            }
          ]
        }
      ]
    }
  ]
}