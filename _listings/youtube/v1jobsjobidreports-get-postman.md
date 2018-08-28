{
  "info": {
    "name": "Youtube Get Jobs Job Reports",
    "_postman_id": "5f89bf4b-24f0-440d-9320-029cba36834d",
    "description": "Lists reports created by a specific job.\nReturns NOT_FOUND if the job does not exist.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "v1",
      "item": [
        {
          "id": "9d6e42a9-b676-4387-9a54-8574634c273c",
          "name": "getV1JobsJobReports",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "youtube",
                "v1",
                "v1/jobs/:jobId/reports"
              ],
              "query": [
                {
                  "key": "createdAfter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "onBehalfOfContentOwner",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startTimeAtOrAfter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startTimeBefore",
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
            "description": "Lists reports created by a specific job"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70543f98-bece-47e4-9a97-40cbc921f1e1"
            }
          ]
        }
      ]
    }
  ]
}