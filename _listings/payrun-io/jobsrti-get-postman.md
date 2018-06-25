{
  "info": {
    "name": "Pay Run.IO Get all RTI jobs",
    "_postman_id": "39232a3d-2872-4786-b0a8-5073bcad3939",
    "description": "Gets all the RTI jobs",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "DPJobs",
      "item": [
        {
          "id": "9df09827-b6bf-4780-8e05-f4cd4d1fef46",
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
              "id": "d83a0602-dc68-42fb-aca8-b103ada543fc"
            }
          ]
        }
      ]
    },
    {
      "name": "PayRun",
      "item": [
        {
          "id": "b44caab3-62ce-4246-acec-4a42e728703d",
          "name": "GetPayRunJobs",
          "request": {
            "url": "http://api.test.payrun.io/Jobs/PayRuns",
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
            "description": "Gets all the pay run jobs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d8c35b1-2a1b-4f7c-9644-7adbacc56290"
            }
          ]
        }
      ]
    },
    {
      "name": "RTI",
      "item": [
        {
          "id": "f356877b-60f2-4940-a747-396413dce0f9",
          "name": "GetRtiJobs",
          "request": {
            "url": "http://api.test.payrun.io/Jobs/Rti",
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
            "description": "Gets all the RTI jobs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c540a301-d381-4e8c-9760-f436d22fd2e1"
            }
          ]
        }
      ]
    }
  ]
}