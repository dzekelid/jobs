{
  "info": {
    "name": "AWS Batch API Create Job Queue",
    "_postman_id": "44a45737-a1e5-4a08-84d0-eeb41c100d86",
    "description": "Creates an AWS Batch job queue.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Jobs",
      "item": [
        {
          "id": "1aa8120d-9d11-4376-beb2-ff217571bd57",
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
              "id": "6d1f44c4-6226-403a-9b1c-7948a4aa02c9"
            }
          ]
        }
      ]
    },
    {
      "name": "Compute Environment",
      "item": [
        {
          "id": "f460e9a3-6c82-4eb8-9151-786dc7a42395",
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
              "id": "7fc9bca9-a0f1-420d-bbfb-c4b7b3867904"
            }
          ]
        }
      ]
    },
    {
      "name": "Job Queue",
      "item": [
        {
          "id": "1d488823-daa8-4603-a475-f334460f6e96",
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
              "id": "f3cc1007-7c3f-4473-9a0d-d509ef895d10"
            }
          ]
        }
      ]
    }
  ]
}