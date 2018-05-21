---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Post Test User 1 Friends Test User 2
  description: The friends of a test user. This is identical to the /&#123;user-id&#125;/friends
    edge aside from the publishing operation explained below.
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