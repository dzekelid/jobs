{
  "info": {
    "name": "Azure IoT Hub API Iot Hub Resource List Jobs",
    "_postman_id": "89c1e216-0009-4963-9c99-c3ffb1358bad",
    "description": "Get a list of all the jobs in an IoT hub. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-identity-registry.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "iot hub resource jobs",
      "item": [
        {
          "id": "4b6c955e-0d45-463e-a65e-ab01a0bb5ded",
          "name": "IotHubResource_ListJobs",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Devices/IotHubs/:resourceName/jobs"
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
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceName",
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
            "description": "Get a list of all the jobs in an IoT hub"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c05a612f-6dde-4523-b1e4-2b1788ada894"
            }
          ]
        }
      ]
    }
  ]
}