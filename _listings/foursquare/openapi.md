---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 1
info:
  title: Foursquare
  description: checkin-explore-your-city-and-connect-people-and-places-bapi-v2-b
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{USER_ID}/friends:
    get:
      summary: Get Users Friends
      description: /users/{USER_ID}/checkins
      operationId: usersuser-idcheckins
      x-api-path-slug: usersuser-idfriends-get
      parameters:
      - in: query
        name: limit
        description: Number of results to return, up to 500
      - in: query
        name: offset
        description: Used to page through results
      - in: query
        name: USER_ID
        description: Identity of the user to get friends of
      - in: path
        name: USER_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Friends
---