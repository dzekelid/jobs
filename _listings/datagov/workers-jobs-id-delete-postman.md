{
  "info": {
    "name": "Data.gov API Delete Workers Jobs",
    "_postman_id": "76911efe-3c93-4608-9695-49b337e3da98",
    "description": "Delete a single scheduled job",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "workers",
      "item": [
        {
          "id": "e5e21e11-0830-426d-850e-5cad8bffa837",
          "name": "deleteWorkersJobs",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a single scheduled job"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80625f20-d2ce-4f12-82c9-c6affedfd1cb"
            }
          ]
        }
      ]
    }
  ]
}