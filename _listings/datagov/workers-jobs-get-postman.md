{
  "info": {
    "name": "Data.gov API Get Workers Jobs",
    "_postman_id": "fc564876-90b3-490b-b3db-298bff0cebbf",
    "description": "List all scheduled jobs",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "workers",
      "item": [
        {
          "id": "f41ea769-db4f-434d-a822-8f8025af1166",
          "name": "getWorkersJobs",
          "request": {
            "url": "http://catalog.data.gov/api/3/workers/jobs/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all scheduled jobs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "241b435c-098c-4a94-8663-f2380a0dfb5a"
            }
          ]
        }
      ]
    }
  ]
}