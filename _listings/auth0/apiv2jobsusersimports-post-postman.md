{
  "info": {
    "name": "Auth0 Jobs API Jobs Users Imports",
    "_postman_id": "e48661b7-b368-473d-b59b-93bd20aa9b07",
    "description": "jobs users imports.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Jobs",
      "item": [
        {
          "id": "1da7cc57-bed8-4a2c-a4c2-77b0c434d40b",
          "name": "post_users-imports",
          "request": {
            "url": "http://login.auth0.com/jobs/api/v2/jobs/users-imports",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "connection_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the connection to which users will be added"
                },
                {
                  "key": "users",
                  "value": "{}",
                  "disabled": false,
                  "description": "A file containing the users to import"
                }
              ]
            },
            "description": "jobs users imports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1cc856e2-3a3a-43de-b7d5-7d9921a16d16"
            }
          ]
        }
      ]
    }
  ]
}