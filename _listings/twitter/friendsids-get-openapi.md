---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Get Friends
  description: returns a cursored collection of user IDs followed by user
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