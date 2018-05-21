---
name: YouTube
x-slug: youtube
description: YouTube allows billions of people to discover, watch and share originally-created
  videos. YouTube provides a forum for people to connect, inform, and inspire others
  across the globe and acts as a distribution platform for original content creators
  and advertisers large and small.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
x-kinRank: "9"
x-alexaRank: ""
tags: Broadcasts
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/apis.md
specificationVersion: "0.14"
apis:
- name: Youtube Delete Live Broadcasts
  x-api-slug: youtube
  description: Delete livebroadcasts
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts
  tags: Livebroadcasts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcasts-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcasts-delete-openapi.md
- name: Youtube Get Live Broadcasts
  x-api-slug: youtube
  description: Returns a list of YouTube broadcasts that match the API request parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts
  tags: Livebroadcasts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcasts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcasts-get-openapi.md
- name: Youtube Parameters Live Broadcasts
  x-api-slug: youtube
  description: Parameters livebroadcasts
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts
  tags: Livebroadcasts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcasts-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcasts-parameters-openapi.md
- name: Youtube Add Live Broadcasts
  x-api-slug: youtube
  description: Creates a broadcast.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts
  tags: Livebroadcasts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcasts-post-openapi.md
- name: Youtube Put Live Broadcasts
  x-api-slug: youtube
  description: Updates a broadcast. For example, you could modify the broadcast settings
    defined in the liveBroadcast resource's contentDetails object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts
  tags: Livebroadcasts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcasts-put-openapi.md
- name: Youtube Parameters Live Broadcasts Bind
  x-api-slug: youtube
  description: Parameters livebroadcasts bind
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts/bind
  tags: Livebroadcasts, Bind
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcastsbind-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcastsbind-parameters-openapi.md
- name: Youtube Add Live Broadcasts Bind
  x-api-slug: youtube
  description: Binds a YouTube broadcast to a stream or removes an existing binding
    between a broadcast and a stream. A broadcast can only be bound to one video stream,
    though a video stream may be bound to more than one broadcast.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts/bind
  tags: Livebroadcasts, Bind
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcastsbind-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcastsbind-post-openapi.md
- name: Youtube Parameters Live Broadcasts Control
  x-api-slug: youtube
  description: Parameters livebroadcasts control
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts/control
  tags: Livebroadcasts, Control
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcastscontrol-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcastscontrol-parameters-openapi.md
- name: Youtube Add Live Broadcasts Control
  x-api-slug: youtube
  description: Controls the settings for a slate that can be displayed in the broadcast
    stream.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts/control
  tags: Livebroadcasts, Control
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcastscontrol-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcastscontrol-post-openapi.md
- name: Youtube Parameters Live Broadcasts Transition
  x-api-slug: youtube
  description: Parameters livebroadcasts transition
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts/transition
  tags: Livebroadcasts, Transition
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcaststransition-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcaststransition-parameters-openapi.md
- name: Youtube Add Live Broadcasts Transition
  x-api-slug: youtube
  description: Changes the status of a YouTube live broadcast and initiates any processes
    associated with the new status. For example, when you transition a broadcast's
    status to testing, YouTube starts to transmit video to that broadcast's monitor
    stream. Before calling this method, you should confirm that the value of the status.streamStatus
    property for the stream bound to your broadcast is active.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts/transition
  tags: Livebroadcasts, Transition
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcaststransition-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/livebroadcaststransition-post-openapi.md
- name: Youtube
  x-api-slug: youtube
  description: YouTube allows billions of people to discover, watch and share originally-created
    videos. YouTube provides a forum for people to connect, inform, and inspire others
    across the globe and acts as a distribution platform for original content creators
    and advertisers large and small.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1
  tags: Broadcasts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/youtube/openapi.md
x-common:
- type: x-articles
  url: https://developers.google.com/youtube/articles/
- type: x-authentication
  url: https://developers.google.com/youtube/v3/guides/authentication
- type: x-blog
  url: https://youtube-eng.googleblog.com/
- type: x-blog-rss
  url: https://youtube-eng.googleblog.com/feeds/posts/default?alt=rss
- type: x-branding
  url: https://developers.google.com/youtube/branding_guidelines
- type: x-bug-report
  url: https://code.google.com/p/gdata-issues/issues/entry
- type: x-bug-report
  url: https://code.google.com/p/gdata-issues/issues/list?q=label:API-YouTube
- type: x-buttons
  url: https://developers.google.com/youtube/youtube_subscribe_button
- type: x-deprecation-policy
  url: https://developers.google.com/youtube/youtube-api-list
- type: x-developer
  url: https://developers.google.com/youtube/
- type: x-getting-started
  url: https://developers.google.com/youtube/v3/getting-started
- type: x-github
  url: https://github.com/youtube
- type: x-github
  url: https://github.com/youtube/
- type: x-terms-of-service
  url: https://developers.google.com/youtube/terms
- type: x-training
  url: https://developers.google.com/youtube/training/
- type: x-twitter
  url: https://twitter.com/YouTubeDev
- type: x-website
  url: https://www.youtube.com/
- type: x-widgets
  url: https://developers.google.com/youtube/youtube_upload_widget
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---