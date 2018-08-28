{
  "info": {
    "name": "Fitbit Get User User Friends.json",
    "_postman_id": "4159c361-e82d-4233-b990-e88e7fd287c6",
    "description": "Get user's friends in the format requested using units in the unit system which corresponds to the Accept-Language header provided.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "1710c623-b202-4402-8bbe-45360788494a",
          "name": "getUserFriendsInvitations.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/friends/invitations.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the list of invites to become freinds for a user in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "412f5cfc-e73e-4261-b063-a80b55010db8"
            }
          ]
        },
        {
          "id": "33eb1771-8d20-4e02-8fa3-9338bf3ce86a",
          "name": "getUserFriendsLeaderboard.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/friends/leaderboard.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a leaderboard of user's friends progress in the format requested using units in the unit system which corresponds to the Accept-Language header provided. Authorized user himself is also included in the response."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b5913c5-504b-4a1f-b459-b4c763be0319"
            }
          ]
        },
        {
          "id": "ad606d0a-1fa1-406e-a661-e8621a04e783",
          "name": "getUserUserFriends.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/:user-id/friends.json"
              ],
              "variable": [
                {
                  "id": "user-id",
                  "value": "user-id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get user's friends in the format requested using units in the unit system which corresponds to the Accept-Language header provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e33f7c76-6499-42d6-adcd-b7e924b9114a"
            }
          ]
        }
      ]
    }
  ]
}