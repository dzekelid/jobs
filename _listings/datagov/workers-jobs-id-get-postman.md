{
  "info": {
    "name": "Data.gov API Get Workers Jobs",
    "_postman_id": "1fa318ef-2990-4f6d-9efe-bc6b2b9e3566",
    "description": "Fetch a single scheduled job",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "workers",
      "item": [
        {
          "id": "903fd96a-2748-48a5-8daa-55926bab4b32",
          "name": "getWorkersJobs",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch a single scheduled job"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e627a108-b5d6-42b8-94f8-4541f947a55f"
            }
          ]
        }
      ]
    }
  ]
}