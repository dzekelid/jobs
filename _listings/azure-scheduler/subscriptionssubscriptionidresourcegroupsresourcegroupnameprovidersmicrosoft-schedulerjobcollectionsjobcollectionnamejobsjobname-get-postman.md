{
  "info": {
    "name": "Azure Scheduler API Jobs Get",
    "_postman_id": "f897370a-685d-4a3e-9a01-7374abb1c2af",
    "description": "Gets a job.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "jobs",
      "item": [
        {
          "id": "e69fb10c-3391-48a1-9954-314fcb390db3",
          "name": "Jobs_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Scheduler/jobCollections/:jobCollectionName/jobs/:jobName"
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a job"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c7258ca-79fc-4f49-a924-22d5768f8473"
            }
          ]
        }
      ]
    }
  ]
}