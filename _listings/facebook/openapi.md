---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook Graph (Achievement Type) API
  description: api-for-managing-facebook-achievement-types
  termsOfService: https://www.facebook.com/policies/
  version: 1.0.0
host: graph.facebook.com
basePath: /v3.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /&#123;test-user-1&#125;/friends/&#123;test-user-2&#125;:
    post:
      summary: Post Test User 1 Friends Test User 2
      description: The friends of a test user. This is identical to the /&#123;user-id&#125;/friends
        edge aside from the publishing operation explained below.
      operationId: postTestUser1FriendsTestUser2
      x-api-path-slug: 123testuser1125friends123testuser2125-post
      responses:
        200:
          description: OK
      tags:
      - Test
      - User
      - "1"
      - Friends
      - Test
      - User
      - "2"
  /&#123;user-id&#125;/invitable_friends:
    get:
      summary: Get User Invitable Friends
      description: User Invitable Friends
      operationId: getUserInvitableFriends
      x-api-path-slug: 123userid125invitable-friends-get
      parameters:
      - in: query
        name: "100"
        description: Invalid parameter
        type: string
      - in: query
        name: "110"
        description: Invalid user id
        type: string
      - in: query
        name: "200"
        description: Permissions error
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Invitable
      - Friends
  /&#123;user-id&#125;/taggable_friends:
    get:
      summary: Get User Taggable Friends
      description: User Taggable Friends
      operationId: getUserTaggableFriends
      x-api-path-slug: 123userid125taggable-friends-get
      parameters:
      - in: query
        name: "100"
        description: Invalid parameter
        type: string
      - in: query
        name: "110"
        description: Invalid user id
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Taggable
      - Friends
---