{
  "info": {
    "name": "Data.gov API Get Workers Jobs Schedulables",
    "_postman_id": "6d858fb5-ed2b-4749-a222-65e4266d0bf5",
    "description": "List all schedulable jobs",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "workers",
      "item": [
        {
          "id": "e28579dd-448a-45af-8cc3-fe4827773646",
          "name": "getWorkersJobsSchedulables",
          "request": {
            "url": "http://catalog.data.gov/api/3/workers/jobs/schedulables",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all schedulable jobs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07f8db22-756a-40ac-b42d-9cbb67c85b8f"
            }
          ]
        }
      ]
    }
  ]
}