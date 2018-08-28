{
  "info": {
    "name": "App Veyor Get Buildjobs Jobid Artifacts",
    "_postman_id": "11de102a-da3e-4065-8559-322fcf5d6eef",
    "description": "Get buildjobs jobid artifacts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Builds",
      "item": [
        {
          "id": "f66bd5c1-8e3f-4d5b-9962-df2a1f7eaa69",
          "name": "getBuildjobsJobArtifacts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "ci.appveyor.com",
              "path": [
                "api",
                "buildjobs/:jobId/artifacts"
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
            "description": "Get buildjobs jobid artifacts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d60e83c-5fb2-4f20-b2fe-76c8791151a1"
            }
          ]
        }
      ]
    }
  ]
}