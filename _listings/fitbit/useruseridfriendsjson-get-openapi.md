---
swagger: "2.0"
x-collection-name: Fitbit
x-complete: 0
info:
  title: Fitbit Get User User Friends.json
  description: Get user's friends in the format requested using units in the unit
    system which corresponds to the Accept-Language header provided.
  version: 1.0.0
host: api.fitbit.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/-/friends/invitations.json:
    get:
      summary: Get User Friends Invitations.json
      description: Retrieve the list of invites to become freinds for a user in the
        format requested.
      operationId: getUserFriendsInvitations.json
      x-api-path-slug: userfriendsinvitationsjson-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Friends
      - Invitations.json
  /user/-/friends/leaderboard.json:
    get:
      summary: Get User Friends Leaderboard.json
      description: Get a leaderboard of user's friends progress in the format requested
        using units in the unit system which corresponds to the Accept-Language header
        provided. Authorized user himself is also included in the response.
      operationId: getUserFriendsLeaderboard.json
      x-api-path-slug: userfriendsleaderboardjson-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Friends
      - Leaderboard.json
  /user/{user-id}/friends.json:
    get:
      summary: Get User User Friends.json
      description: Get user's friends in the format requested using units in the unit
        system which corresponds to the Accept-Language header provided.
      operationId: getUserUserFriends.json
      x-api-path-slug: useruseridfriendsjson-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Friends.json
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