{
  "info": {
    "name": "AWS Batch API Delete Job Queue",
    "_postman_id": "c3604596-3e93-4ada-9639-6c569536a2f1",
    "description": "Deletes the specified job queue.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Jobs",
      "item": [
        {
          "id": "d85eb3b2-f2e3-45b4-825b-37298f067b9e",
          "name": "cancelJob",
          "request": {
            "url": "http://example.com/api/?Action=CancelJob?jobId=jobId&reason=reason",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels jobs in an AWS Batch job queue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4b209c4-141c-4f10-b7e2-37f0ab7903a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Compute Environment",
      "item": [
        {
          "id": "42cb6635-2a60-4069-9ff0-a4a7d1d48c26",
          "name": "createComputeEnvironment",
          "request": {
            "url": "http://example.com/api/?Action=CreateComputeEnvironment?computeEnvironmentName=computeEnvironmentName&computeResources=computeResources&serviceRole=serviceRole&state=state&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an AWS Batch compute environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0df67508-09bb-4a6a-b1ac-e37373cda859"
            }
          ]
        },
        {
          "id": "779144e0-5a76-474d-8691-8bb1333f566d",
          "name": "deleteComputeEnvironment",
          "request": {
            "url": "http://example.com/api/?Action=DeleteComputeEnvironment?computeEnvironment=computeEnvironment",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an AWS Batch compute environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0a96897-4c6a-4660-9a1b-2b4791d84b07"
            }
          ]
        }
      ]
    },
    {
      "name": "Job Queue",
      "item": [
        {
          "id": "4c105c50-2b62-4013-bb14-fe4b81b1ab01",
          "name": "createJobQueue",
          "request": {
            "url": "http://example.com/api/?Action=CreateJobQueue?computeEnvironmentOrder=computeEnvironmentOrder&jobQueueName=jobQueueName&priority=priority&state=state",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an AWS Batch job queue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e2b000d-4fd3-41b7-8af3-82dbb706133f"
            }
          ]
        },
        {
          "id": "87541a6d-49e6-4b6d-b976-7bda7ba1a30b",
          "name": "deleteJobQueue",
          "request": {
            "url": "http://example.com/api/?Action=DeleteJobQueue?jobQueue=jobQueue",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified job queue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb10a547-126a-4e99-af3b-ee39d05d38e5"
            }
          ]
        }
      ]
    }
  ]
}