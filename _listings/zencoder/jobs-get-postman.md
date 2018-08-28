{
  "info": {
    "name": "Zencoder API List Jobs",
    "_postman_id": "41cbbdf9-83f4-4e79-a257-f70f63d67a03",
    "description": "A list of jobs can be obtained by sending an HTTP GET request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "30d37762-89ec-455b-9bc3-2081d744049d",
          "name": "getAccount",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account?api_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Account Details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51183a51-4451-40af-aab1-8dfbc78bfb99"
            }
          ]
        },
        {
          "id": "f671bf2b-f0b3-450b-8551-a05f95ec6885",
          "name": "postAccount",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account?email=%7B%7D&password=%7B%7D&password_confirmation=%7B%7D&terms_of_service=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an Account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79d51ad7-f3b6-4053-a82f-0214b9b42d33"
            }
          ]
        },
        {
          "id": "5eafdb6e-a9b2-4ffd-8801-85bb6743c37b",
          "name": "putAccountIntegration",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account/integration?api_key=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Integration Mode"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0d72767-110b-4071-89dc-09c32a656444"
            }
          ]
        },
        {
          "id": "100152ac-e3c7-4c73-87d0-cc1ed8114b3e",
          "name": "putAccountLive",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account/live",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Integration Mode - Live"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "801c1209-f234-44fd-9a84-b5bb1d90f0ae"
            }
          ]
        }
      ]
    },
    {
      "name": "Inputs",
      "item": [
        {
          "id": "40afd16f-4cdd-4e25-ab1a-52dcaef2fff2",
          "name": "getInupdatesInupdate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "inputs/:input_id"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "input_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Input Details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ccfaff3-bf57-42c1-845a-93129af4c373"
            }
          ]
        },
        {
          "id": "918483aa-c85c-422c-9476-dda17720b709",
          "name": "getInupdatesInupdateProgress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "inputs/:input_id/progress"
              ],
              "variable": [
                {
                  "id": "input_id",
                  "value": "input_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The return will contain one or more of the following keys: state, current_event, current_event_progress and progress."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38348c97-6222-485e-8654-1d5eb20a5baa"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "ece42b52-6c73-4ae9-bed6-87d66bb3245d",
          "name": "getJobs",
          "request": {
            "url": "http://app.zencoder.com/api/v2/jobs?api_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A list of jobs can be obtained by sending an HTTP GET request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0af1d3d-daba-439d-b5fe-50354b98acf1"
            }
          ]
        }
      ]
    }
  ]
}