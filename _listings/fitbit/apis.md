---
name: Fitbit
x-slug: fitbit
description: Find your fit with Fitbits family of fitness products that help you stay
  motivated and improve your health by tracking your activity, exercise, food, weight
  and sleep.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/200-fitbit.jpg
x-kinRank: "9"
x-alexaRank: "2266"
tags: Friends
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/friends/master/_listings/fitbit/apis.md
specificationVersion: "0.14"
apis:
- name: Fitbit - Get User Friends Invitations.json
  x-api-slug: userfriendsinvitations-json-get
  description: Retrieve the list of invites to become freinds for a user in the format
    requested.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/200-fitbit.jpg
  humanURL: http://fitbit.com
  baseURL: https://api.fitbit.com//1
  tags: Sports, Excercise, Devices, Fitness, Wearables, Indie EdTech Data Jam, Stack,
    Mobile, Technology, API Provider, , Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/friends/master/_listings/fitbit/userfriendsinvitations-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/friends/master/_listings/fitbit/userfriendsinvitations-json-get-openapi.md
- name: Fitbit - Get User Friends Leaderboard.json
  x-api-slug: userfriendsleaderboard-json-get
  description: Get a leaderboard of user's friends progress in the format requested
    using units in the unit system which corresponds to the Accept-Language header
    provided. Authorized user himself is also included in the response.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/200-fitbit.jpg
  humanURL: http://fitbit.com
  baseURL: https://api.fitbit.com//1
  tags: Sports, Excercise, Devices, Fitness, Wearables, Indie EdTech Data Jam, Stack,
    Mobile, Technology, API Provider, , Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/friends/master/_listings/fitbit/userfriendsleaderboard-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/friends/master/_listings/fitbit/userfriendsleaderboard-json-get-openapi.md
x-common:
- type: x-api-json--authoritative
  url: https://www.fitbit.com/apis.json
- type: x-openapi
  url: https://dev.fitbit.com/reference/web-api/explore/fitbit-web-api.swagger.json
- type: x-api-gallery
  url: http://first.trust.bank.api.gallery.streamdata.io
- type: x-api-stack
  url: http://fitbit.stack.network
- type: x-apigee-console
  url: https://wiki.fitbit.com/display/API/API+Explorer
- type: x-blog
  url: http://blog.fitbit.com
- type: x-blog-rss
  url: http://blog.fitbit.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/fitbit
- type: x-crunchbase
  url: https://crunchbase.com/organization/fitbit
- type: x-email
  url: privacy@fitbit.com
- type: x-github
  url: https://github.com/fitbit
- type: x-rate-limits
  url: https://wiki.fitbit.com/display/API/Rate+Limit
- type: x-twitter
  url: https://twitter.com/fitbit
- type: x-website
  url: http://fitbit.com
- type: x-website
  url: http://dev.fitbit.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---