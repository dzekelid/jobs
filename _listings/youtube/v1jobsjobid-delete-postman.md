{
  "info": {
    "name": "Youtube Delete Jobs Job",
    "_postman_id": "5f16bca6-5bea-4b94-8855-6f1051886d89",
    "description": "Delete v1 jobs job",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "v1",
      "item": [
        {
          "id": "1c196af6-714e-426f-88c2-c3a577500487",
          "name": "deleteV1JobsJob",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete v1 jobs job"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec88c392-b8fb-4a31-ab54-617a4b6c1b0c"
            }
          ]
        }
      ]
    }
  ]
}