---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 0
info:
  title: Youtube Add Live Broadcasts Control
  description: Controls the settings for a slate that can be displayed in the broadcast
    stream.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /liveBroadcasts:
    delete:
      summary: Delete Live Broadcasts
      description: Delete livebroadcasts
      operationId: deleteLivebroadcasts
      x-api-path-slug: livebroadcasts-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube live broadcast ID for
          the resource that is being deleted
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      responses:
        200:
          description: OK
      tags:
      - Livebroadcasts
    get:
      summary: Get Live Broadcasts
      description: Returns a list of YouTube broadcasts that match the API request
        parameters.
      operationId: getLivebroadcasts
      x-api-path-slug: livebroadcasts-get
      parameters:
      - in: query
        name: broadcastStatus
        description: The broadcastStatus parameter filters the API response to only
          include broadcasts with the specified status
      - in: query
        name: broadcastType
        description: The broadcastType parameter filters the API response to only
          include broadcasts with the specified type
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of YouTube
          broadcast IDs that identify the broadcasts being retrieved
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: The mine parameter can be used to instruct the API to only return
          broadcasts owned by the authenticated user
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more liveBroadcast resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Livebroadcasts
    post:
      summary: Add Live Broadcasts
      description: Creates a broadcast.
      operationId: postLivebroadcasts
      x-api-path-slug: livebroadcasts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Livebroadcasts
    put:
      summary: Put Live Broadcasts
      description: Updates a broadcast. For example, you could modify the broadcast
        settings defined in the liveBroadcast resource's contentDetails object.
      operationId: putLivebroadcasts
      x-api-path-slug: livebroadcasts-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Livebroadcasts
  /liveBroadcasts/bind:
    post:
      summary: Add Live Broadcasts Bind
      description: Binds a YouTube broadcast to a stream or removes an existing binding
        between a broadcast and a stream. A broadcast can only be bound to one video
        stream, though a video stream may be bound to more than one broadcast.
      operationId: postLivebroadcastsBind
      x-api-path-slug: livebroadcastsbind-post
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the unique ID of the broadcast that
          is being bound to a video stream
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more liveBroadcast resource properties that the API response will include
      - in: query
        name: streamId
        description: The streamId parameter specifies the unique ID of the video stream
          that is being bound to a broadcast
      responses:
        200:
          description: OK
      tags:
      - Livebroadcasts
      - Bind
  /liveBroadcasts/control:
    post:
      summary: Add Live Broadcasts Control
      description: Controls the settings for a slate that can be displayed in the
        broadcast stream.
      operationId: postLivebroadcastsControl
      x-api-path-slug: livebroadcastscontrol-post
      parameters:
      - in: query
        name: displaySlate
        description: The displaySlate parameter specifies whether the slate is being
          enabled or disabled
      - in: query
        name: id
        description: The id parameter specifies the YouTube live broadcast ID that
          uniquely identifies the broadcast in which the slate is being updated
      - in: query
        name: offsetTimeMs
        description: The offsetTimeMs parameter specifies a positive time offset when
          the specified slate change will occur
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more liveBroadcast resource properties that the API response will include
      - in: query
        name: walltime
        description: The walltime parameter specifies the wall clock time at which
          the specified slate change will occur
      responses:
        200:
          description: OK
      tags:
      - Livebroadcasts
      - Control
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