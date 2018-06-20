{
  "info": {
    "name": "Fitbit Get User Friends Leaderboard.json",
    "_postman_id": "bd8833e7-4c31-42c0-abf3-c958d2417f22",
    "description": "Get a leaderboard of user's friends progress in the format requested using units in the unit system which corresponds to the Accept-Language header provided. Authorized user himself is also included in the response.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "965de450-490d-4e72-b4ef-40544a731f92",
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
              "id": "7d625272-8afc-43d9-8632-5f45211a2d8e"
            }
          ]
        },
        {
          "id": "d3d6bfd0-74b0-4a43-add3-1f7d265fdaaf",
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
              "id": "d02e414a-79b7-4b27-afbe-af4e9f70a5ff"
            }
          ]
        }
      ]
    }
  ]
}