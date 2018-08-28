{
  "info": {
    "name": "AWS Elastic MapReduce API Add Job Flow Steps",
    "_postman_id": "821533bf-32f6-44cc-bd05-734a1d3f8db2",
    "description": "AddJobFlowSteps adds new steps to a running job flow.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Job Flow Steps",
      "item": [
        {
          "id": "182f674d-cb79-4c21-8b02-92618b8aaf2b",
          "name": "addJobFlowSteps",
          "request": {
            "url": "http://example.com/api/?Action=AddJobFlowSteps?JobFlowId=JobFlowId&Steps=Steps",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "AddJobFlowSteps adds new steps to a running job flow."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d382fe45-9b13-453b-aed6-e36c3179fbad"
            }
          ]
        }
      ]
    }
  ]
}