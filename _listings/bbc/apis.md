---
name: BBC
x-slug: bbc
description: Breaking news, sport, TV, radio and a whole lot more. The BBC informs,
  educates and entertains - wherever you are, whatever your age.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28554-bbc-nitro.jpg
x-kinRank: "7"
x-alexaRank: "93"
tags: Broadcasts
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/bbc/apis.md
specificationVersion: "0.14"
apis:
- name: BBC Nitro Build schedules and find metadata for TV and radio broadcasts
  x-api-slug: bbc-nitro
  description: Fetch metadata about linear Broadcasts and Services, allowing the generation
    of Television and Radio schedules and other datasets for broadcast items. Use
    /schedules instead of this feed as it is more efficient. Broadcasts will be deprecated
    in the future.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28554-bbc-nitro.jpg
  humanURL: http://www.bbc.com/
  baseURL: https://programmes.api.bbc.com//nitro/api//broadcasts
  tags: Broadcasts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/bbc/broadcasts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/bbc/broadcasts-get-openapi.md
- name: BBC Nitro
  x-api-slug: bbc-nitro
  description: Breaking news, sport, TV, radio and a whole lot more. The BBC informs,
    educates and entertains - wherever you are, whatever your age.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28554-bbc-nitro.jpg
  humanURL: http://www.bbc.com/
  baseURL: https://programmes.api.bbc.com//nitro/api
  tags: Broadcasts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/broadcasts/master/_listings/bbc/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/bbc-news
- type: x-email
  url: dataprotection@bbc.com
- type: x-email
  url: bbcworldwidelearning@bbc.com
- type: x-twitter
  url: https://twitter.com/BBCNews
- type: x-website
  url: http://www.bbc.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---