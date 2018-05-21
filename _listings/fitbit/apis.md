---
name: Fitbit
x-slug: fitbit
description: Fitbit Inc. is a company headquartered in San Francisco, California,
  United States. Founded and managed by James Park and Eric Friedman, the company
  is known for its product of the same name, the Fitbit Tracker, a wireless-enabled
  wearable device that measures data such as the number of steps walked, quality of
  sleep, and other personal metrics. The average price of the Fitbit is between $60&ndash;$130,
  depending on the model. However, data cannot be downloaded off the fitbit website
  unless one pays the premium membership price of $49 per year. Intraday data analysis
  cannot be downloaded at all.
image: https://avatars2.githubusercontent.com/u/1039877?v=4
x-kinRank: "9"
x-alexaRank: ""
tags: Friends
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/friends/master/_listings/fitbit/apis.md
specificationVersion: "0.14"
apis:
- name: Fitbit Get User Friends Invitations.json
  x-api-slug: fitbit
  description: Retrieve the list of invites to become freinds for a user in the format
    requested.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/friends/invitations.json
  tags: User,-,Friends,Invitations.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/friends/master/_listings/fitbit/userfriendsinvitationsjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/friends/master/_listings/fitbit/userfriendsinvitationsjson-get-openapi.md
- name: Fitbit Get User Friends Leaderboard.json
  x-api-slug: fitbit
  description: Get a leaderboard of user's friends progress in the format requested
    using units in the unit system which corresponds to the Accept-Language header
    provided. Authorized user himself is also included in the response.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/friends/leaderboard.json
  tags: User,-,Friends,Leaderboard.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/friends/master/_listings/fitbit/userfriendsleaderboardjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/friends/master/_listings/fitbit/userfriendsleaderboardjson-get-openapi.md
- name: Fitbit Get User User Friends.json
  x-api-slug: fitbit
  description: Get user's friends in the format requested using units in the unit
    system which corresponds to the Accept-Language header provided.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/{user-id}/friends.json
  tags: User,User-id,Friends.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/friends/master/_listings/fitbit/useruseridfriendsjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/friends/master/_listings/fitbit/useruseridfriendsjson-get-openapi.md
- name: Fitbit
  x-api-slug: fitbit
  description: Fitbit Inc. is a company headquartered in San Francisco, California,
    United States. Founded and managed by James Park and Eric Friedman, the company
    is known for its product of the same name, the Fitbit Tracker, a wireless-enabled
    wearable device that measures data such as the number of steps walked, quality
    of sleep, and other personal metrics. The average price of the Fitbit is between
    $60&ndash;$130, depending on the model. However, data cannot be downloaded off
    the fitbit website unless one pays the premium membership price of $49 per year.
    Intraday data analysis cannot be downloaded at all.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1
  tags: Friends
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/friends/master/_listings/fitbit/openapi.md
x-common:
- type: x-apijson--authoritative
  url: https://www.fitbit.com/apis.json
- type: x-apigee-console
  url: https://wiki.fitbit.com/display/API/API+Explorer
- type: x-blog
  url: http://blog.fitbit.com
- type: x-blog-rss
  url: http://blog.fitbit.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/fitbit
- type: x-github
  url: https://github.com/fitbit
- type: x-rate-limits
  url: https://wiki.fitbit.com/display/API/Rate+Limit
- type: x-twitter
  url: https://twitter.com/fitbit
- type: x-website
  url: http://dev.fitbit.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---