{
  "info": {
    "name": "Youtube Get Jobs Job Reports Report",
    "_postman_id": "f56844cc-6712-42e0-a89e-61a23ed6d238",
    "description": "Gets the metadata of a specific report.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "v1",
      "item": [
        {
          "id": "feaf3b5a-f9d9-4a38-82ea-978c224a4c42",
          "name": "getV1JobsJobReportsReport",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "youtube",
                "v1",
                "v1/jobs/:jobId/reports/:reportId"
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
                },
                {
                  "id": "reportId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the metadata of a specific report"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b4db1b4-e492-4c9a-af49-e8e53e1c9801"
            }
          ]
        }
      ]
    }
  ]
}