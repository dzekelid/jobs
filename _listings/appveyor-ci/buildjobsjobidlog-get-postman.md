{
  "info": {
    "name": "App Veyor Get Buildjobs Jobid Log",
    "_postman_id": "b83b4763-30c7-41cb-9be6-1a1498755ccf",
    "description": "Get buildjobs jobid log.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Builds",
      "item": [
        {
          "id": "2da2edfc-2394-4607-a133-1d6fbbd46759",
          "name": "getBuildjobsJobLog",
          "request": {
            "url": {
              "protocol": "http",
              "host": "ci.appveyor.com",
              "path": [
                "api",
                "buildjobs/:jobId/log"
              ],
              "variable": [
                {
                  "id": "jobId",
                  "value": "jobId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get buildjobs jobid log."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a06ca6c6-6e50-42bd-abc8-8a68e52fefac"
            }
          ]
        }
      ]
    }
  ]
}