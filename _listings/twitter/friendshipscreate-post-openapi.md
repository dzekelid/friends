---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Follow User
  description: allows users to follow user sepcified by ID
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /friends/ids:
    get:
      summary: Get Friends
      description: returns a cursored collection of user IDs followed by user
      operationId: returns-a-cursored-collection-of-user-ids-followed-by-user
      x-api-path-slug: friendsids-get
      parameters:
      - in: query
        name: count
        description: number of IDs to attempt retrieval of
      - in: query
        name: cursor
        description: causes list of connections to be broken in pages
      - in: query
        name: screen_name
        description: screen name of user for whom to return results for
      - in: query
        name: stringify_ids
        description: IDs converted to strings
      - in: query
        name: user_id
        description: ID of user for whom to return results for
      responses:
        200:
          description: OK
      tags:
      - Social
      - Friends
  /followers/ids:
    get:
      summary: Get Followers
      description: returns a cursored collection of user IDs following the user
      operationId: returns-a-cursored-collection-of-user-ids-following-the-user
      x-api-path-slug: followersids-get
      parameters:
      - in: query
        name: count
        description: number of IDs to attempt retrieval of
      - in: query
        name: cursor
        description: causes list of connections to be broken in pages
      - in: query
        name: screen_name
        description: screen name of user for whom to return results for
      - in: query
        name: stringify_ids
        description: IDs converted to strings
      - in: query
        name: user_id
        description: ID of user for whom to return results for
      responses:
        200:
          description: OK
      tags:
      - Social
      - Friends
  /friendships/incoming:
    get:
      summary: Get Friend Requests
      description: returns collection of IDs of users with pending follow request
      operationId: returns-collection-of-ids-of-users-with-pending-follow-request
      x-api-path-slug: friendshipsincoming-get
      parameters:
      - in: query
        name: cursor
        description: causes list of connections to be broken in pages
      - in: query
        name: stringify_ids
        description: IDs converted to strings
      responses:
        200:
          description: OK
      tags:
      - Social
      - Friends
  /friendships/outgoing:
    get:
      summary: Get Friend Requests
      description: returns collection of IDs of users with pending follow request
        from the user
      operationId: returns-collection-of-ids-of-users-with-pending-follow-request-from-the-user
      x-api-path-slug: friendshipsoutgoing-get
      parameters:
      - in: query
        name: cursor
        description: causes list of connections to be broken in pages
      - in: query
        name: stringify_ids
        description: IDs converted to strings
      responses:
        200:
          description: OK
      tags:
      - Social
      - Friends
  /friendships/create:
    post:
      summary: Follow User
      description: allows users to follow user sepcified by ID
      operationId: allows-users-to-follow-user-sepcified-by-id
      x-api-path-slug: friendshipscreate-post
      parameters:
      - in: query
        name: follow
        description: enable notifications for target user
      - in: query
        name: screen_name
        description: screen name of user for whom to befriend
      - in: query
        name: user_id
        description: ID of user for whom to befriend
      responses:
        200:
          description: OK
      tags:
      - Social
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