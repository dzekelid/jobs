{
  "info": {
    "name": "Pay Run.IO Get all DPS jobs",
    "_postman_id": "40d267fa-0d91-444b-9472-7e9e9a04efe9",
    "description": "Gets all the DPS jobs",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "DPJobs",
      "item": [
        {
          "id": "40138786-dcb9-4c9d-9551-59f624997105",
          "name": "GetDpsJobs",
          "request": {
            "url": "http://api.test.payrun.io/Jobs/Dps",
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the DPS jobs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffcc68c1-9397-4acb-b686-8fed106a843a"
            }
          ]
        }
      ]
    }
  ]
}