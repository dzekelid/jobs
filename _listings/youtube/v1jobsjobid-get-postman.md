{
  "info": {
    "name": "Youtube Get Jobs Job",
    "_postman_id": "a1f01e5b-5be9-41fa-a4c0-b07e45c2b77e",
    "description": "Get v1 jobs job",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "v1",
      "item": [
        {
          "id": "d66d76ed-ae46-47f3-b864-effdf72c909e",
          "name": "getV1JobsJob",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "youtube",
                "v1",
                "v1/jobs/:jobId"
              ],
              "query": [
                {
                  "key": "onBehalfOfContentOwner",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "jobId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get v1 jobs job"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2d2151d-7cc1-4799-be99-f389794ad7dd"
            }
          ]
        }
      ]
    }
  ]
}