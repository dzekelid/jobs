{
  "info": {
    "name": "Data.gov API Put Workers Jobs",
    "_postman_id": "2c7268a5-099a-4670-8f6c-fd713cbf163a",
    "description": "Update a single scheduled job",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "workers",
      "item": [
        {
          "id": "7e3ff265-c4cc-4549-9a46-3f47df0d7f60",
          "name": "putWorkersJobs",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "workers/jobs/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a single scheduled job"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52dd5947-1343-4574-858c-99373ebe0358"
            }
          ]
        }
      ]
    }
  ]
}