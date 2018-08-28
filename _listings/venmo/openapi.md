swagger: "2.0"
x-collection-name: Venmo
x-complete: 1
info:
  title: Venmo API
  description: the-venmo-api-provides-developers-a-straightforward-way-to-integrate-venmo-into-their-applications--
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