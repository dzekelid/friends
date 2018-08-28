swagger: "2.0"
x-collection-name: Fitbit
x-complete: 1
info:
  title: Fitbit
  description: bring-fitbit-health-data-into-your-apps-including-user-activities-sleep-heart-glucose-and-blood-pressure-information-
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
      x-api-path-slug: userfriendsinvitations-json-get
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
      x-api-path-slug: userfriendsleaderboard-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Friends
      - Leaderboard.json