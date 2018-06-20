---
swagger: "2.0"
x-collection-name: Venmo
x-complete: 0
info:
  title: Venmo API Get Users User Friends
  description: Get users user friends.
  version: 1.0.0
host: api.venmo.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/friends:
    get:
      summary: Get Users User Friends
      description: Get users user friends.
      operationId: getUsersUserFriends
      x-api-path-slug: usersuser-idfriends-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Friends
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