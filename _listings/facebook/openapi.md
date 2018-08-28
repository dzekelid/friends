swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{user}/friends:
    get:
      summary: Get User Friends
      description: The user's friends
      operationId: getUserFriends
      x-api-path-slug: userfriends-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Friends
  /{user}/friends/{friend}:
    get:
      summary: Get User Friends Friend
      description: Checks if the given user is a friend of the current user
      operationId: getUserFriendsFriend
      x-api-path-slug: userfriendsfriend-get
      parameters:
      - in: path
        name: friend
        description: Represents the ID of the users friend
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Friends
      - Friend