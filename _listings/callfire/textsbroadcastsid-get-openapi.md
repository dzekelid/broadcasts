---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Find a specific text broadcast
  description: Returns a single TextBroadcast instance for a given text broadcast
    id
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calls/broadcasts:
    get:
      summary: Find call broadcasts
      description: Searches for all voice broadcasts created by user. Can query on
        label, name, and the current running status of the campaign. Returns a paged
        list of voice broadcasts
      operationId: findCallBroadcasts
      x-api-path-slug: callsbroadcasts-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: label
        description: A label of a voice broadcast
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: name
        description: A name of voice broadcast
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: running
        description: Specify whether the campaigns should be running or not
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
    post:
      summary: Create a call broadcast
      description: Creates a call broadcast campaign using the Call Broadcast API.
        Send a CallBroadcast in the message body to add details in a voice broadcast
        campaign. The campaign can be created without contacts and bare minimum configuration,
        but contacts will have to be added further on to use the campaign
      operationId: createCallBroadcast
      x-api-path-slug: callsbroadcasts-post
      parameters:
      - in: body
        name: body
        description: A CallBroadcast object
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: start
        description: Specify whether to immediately start this campaign (not required)
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
  /calls/broadcasts/{id}:
    get:
      summary: Find a specific call broadcast
      description: Returns a single CallBroadcast instance for a given call broadcast
        campaign id
      operationId: getCallBroadcast
      x-api-path-slug: callsbroadcastsid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a CallBroadcast
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
    put:
      summary: Update a call broadcast
      description: This operation lets the user modify the configuration of a voice
        broadcast campaign after call broadcast campaign is created. See CallBroadcast
        for more information on what can/can't be updated on this API
      operationId: updateCallBroadcast
      x-api-path-slug: callsbroadcastsid-put
      parameters:
      - in: body
        name: body
        description: A CallBroadcast object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: An id of a voice broadcast
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
  /calls/broadcasts/{id}/archive:
    post:
      summary: Archive voice broadcast
      description: Archives a voice broadcast (voice broadcast will be hidden in search
        results)
      operationId: archiveVoiceBroadcast
      x-api-path-slug: callsbroadcastsidarchive-post
      parameters:
      - in: path
        name: id
        description: An id of a voice broadcast to archive
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Archive
  /calls/broadcasts/{id}/batches:
    get:
      summary: Find batches in a call broadcast
      description: This endpoint will enable the user to page through all of the batches
        for a particular voice broadcast campaign
      operationId: getCallBroadcastBatches
      x-api-path-slug: callsbroadcastsidbatches-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a call broadcast
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Batches
    post:
      summary: Add batches to a call broadcast
      description: The 'add batch' API allows user to add additional batches to an
        already created voice broadcast campaign. The added batch will go through
        the CallFire validation process, unlike in the recipients version of this
        API. That is why you can use the scrubDuplicates flag to remove duplicates
        from your batch. Batches may be added as a contact list id, a list of contact
        ids, or a list of numbers
      operationId: addCallBroadcastBatch
      x-api-path-slug: callsbroadcastsidbatches-post
      parameters:
      - in: body
        name: body
        description: A request object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: An id of a call broadcast
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Batches
  /calls/broadcasts/{id}/calls:
    get:
      summary: Find calls in a call broadcast
      description: This endpoint will enable the user to page through all calls for
        a particular call broadcast campaign
      operationId: getCallBroadcastCalls
      x-api-path-slug: callsbroadcastsidcalls-get
      parameters:
      - in: query
        name: batchId
        description: An id of a particular batch associated with broadcast
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An Id of a call broadcast
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Calls
  /calls/broadcasts/{id}/recipients:
    post:
      summary: Add recipients to a call broadcast
      description: Use this API to add the recipients to an existing voice broadcast.
        Post a list of Recipient objects to be added to the voice broadcast campaign.
        These contacts will not go through validation process, and will be acted upon
        as they are added. Recipients may be added as a list of contact ids, or list
        of numbers
      operationId: addCallBroadcastRecipients
      x-api-path-slug: callsbroadcastsidrecipients-post
      parameters:
      - in: body
        name: body
        description: A list of CallRecipient objects
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a call broadcast
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Recipients
  /calls/broadcasts/{id}/start:
    post:
      summary: Start voice broadcast
      description: Start a voice broadcast
      operationId: startVoiceBroadcast
      x-api-path-slug: callsbroadcastsidstart-post
      parameters:
      - in: path
        name: id
        description: An id of voice broadcast to start
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Start
  /calls/broadcasts/{id}/stats:
    get:
      summary: Get statistics on call broadcast
      description: Returns broadcast statistics like total number of sent/received
        actions, total cost, number of remaining outbound actions, error count, etc
      operationId: getCallBroadcastStats
      x-api-path-slug: callsbroadcastsidstats-get
      parameters:
      - in: query
        name: begin
        description: Start of the search time interval, formatted in unix time milliseconds
      - in: query
        name: end
        description: End of the search time interval, formatted in unix time milliseconds
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a call broadcast
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Stats
  /calls/broadcasts/{id}/stop:
    post:
      summary: Stop voice broadcast
      description: Stop a voice broadcast
      operationId: stopVoiceBroadcast
      x-api-path-slug: callsbroadcastsidstop-post
      parameters:
      - in: path
        name: id
        description: An id of voice broadcast to stop
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Stop
  /texts/broadcasts:
    get:
      summary: Find text broadcasts
      description: Searches for all text broadcasts created by user. Can query on
        label, name, and the current running status of the campaign. Returns a paged
        list of text broadcasts
      operationId: findTextBroadcasts
      x-api-path-slug: textsbroadcasts-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: label
        description: A label of a text broadcast
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: name
        description: A name of text broadcast
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: running
        description: Returns broadcasts only in running state
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
    post:
      summary: Create a text broadcast
      description: Creates a text broadcast campaign using the Text Broadcast API.
        Send a TextBroadcast object in the message body to detail a text broadcast
        campaign. A campaign can be created without contacts and with bare minimum
        configuration, but contacts have to be added further on to use the campaign.
        It supports scheduling, retry logic, pattern-based messages.
      operationId: createTextBroadcast
      x-api-path-slug: textsbroadcasts-post
      parameters:
      - in: body
        name: body
        description: A TextBroadcast object
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: start
        description: If true then starts the campaign immediately (not required)
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
  /texts/broadcasts/{id}:
    get:
      summary: Find a specific text broadcast
      description: Returns a single TextBroadcast instance for a given text broadcast
        id
      operationId: getTextBroadcast
      x-api-path-slug: textsbroadcastsid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a text broadcast
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
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