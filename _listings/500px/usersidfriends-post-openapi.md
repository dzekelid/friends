---
swagger: "2.0"
x-collection-name: 500px
x-complete: 0
info:
  title: 500px Post Users Friends
  description: Add the user to the list of followers.
  version: v1
host: api.500px.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/:id/friends:
    delete:
      summary: Delete Users Friends
      description: Removes the user from the list of followers.
      operationId: deleteUsersFriends
      x-api-path-slug: usersidfriends-delete
      parameters:
      - in: query
        name: id (required)
        description: ID of the User to remove from the followers list
      responses:
        200:
          description: OK
      tags:
      - Users
      - Friends
    get:
      summary: Get Users Friends
      description: Returns a list of friends for the specified user.
      operationId: getUsersFriends
      x-api-path-slug: usersidfriends-get
      parameters:
      - in: query
        name: id (required)
        description: Return information for the specified user ID
      - in: query
        name: page
        description: Return the specified page of the resource
      - in: query
        name: rpp
        description: Results Per Page, default 20, max 100
      responses:
        200:
          description: OK
      tags:
      - Users
      - Friends
    post:
      summary: Post Users Friends
      description: Add the user to the list of followers.
      operationId: postUsersFriends
      x-api-path-slug: usersidfriends-post
      parameters:
      - in: query
        name: id (required)
        description: ID of the User to add to the followers list
      responses:
        200:
          description: OK
      tags:
      - Users
      - Friends
  /users/{id}/friends:
    get:
      summary: Get Users Friends
      description: Returns a list of friends for the specified user.
      operationId: getUsersFriends
      x-api-path-slug: usersidfriends-get
      parameters:
      - in: path
        name: id
        description: Return information for the specified user ID
      - in: query
        name: page
        description: Return the specified page of the resource
      - in: query
        name: rpp
        description: Results Per Page, default 20, max 100
      responses:
        200:
          description: OK
      tags:
      - Users
      - Friends
    post:
      summary: Post Users Friends
      description: Add the user to the list of followers.
      operationId: postUsersFriends
      x-api-path-slug: usersidfriends-post
      parameters:
      - in: path
        name: id
        description: ID of the User to add to the followers list
      responses:
        200:
          description: OK
      tags:
      - Users
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