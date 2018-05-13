{
  "info": {
    "name": "Azure Scheduler API Jobs Run",
    "_postman_id": "802b3a6b-309b-4672-818d-5748565c7667",
    "description": "Runs a job.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "jobs",
      "item": [
        {
          "id": "6bd22d47-837c-4b43-a9a2-72a27214f938",
          "name": "Jobs_Run",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Scheduler/jobCollections/:jobCollectionName/jobs/:jobName/run"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "jobCollectionName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "jobName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Runs a job"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07b14c81-d03a-43ad-84c3-e7be0b12f947"
            }
          ]
        }
      ]
    }
  ]
}