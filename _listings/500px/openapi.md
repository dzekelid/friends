---
swagger: "2.0"
x-collection-name: 500px
x-complete: 1
info:
  title: 500px
  description: 500px-is-a-photo-community-powered-by-creative-people-worldwide-that-lets-you-discover-share-buy-and-sell-inspiring-photographs-
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
    delete:
      summary: Delete Users Friends
      description: Removes the user from the list of followers.
      operationId: deleteUsersFriends
      x-api-path-slug: usersidfriends-delete
      parameters:
      - in: path
        name: id
        description: ID of the User to remove from the followers list
      responses:
        200:
          description: OK
      tags:
      - Users
      - Friends
---