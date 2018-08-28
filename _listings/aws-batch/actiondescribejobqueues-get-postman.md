{
  "info": {
    "name": "AWS Batch API Describe Job Queues",
    "_postman_id": "de8c57d3-4a01-41e9-b11a-128b3154bf96",
    "description": "Describes one or more of your job queues.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Jobs",
      "item": [
        {
          "id": "2bbd9f40-cefd-489e-ad21-272aa32a8210",
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
              "id": "1046e5fa-34f0-43c3-ad0e-28ac75076bf4"
            }
          ]
        }
      ]
    },
    {
      "name": "Compute Environment",
      "item": [
        {
          "id": "f31fae00-3404-4cd8-b9d5-c493fc3a21cd",
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
              "id": "59fe3788-47d0-41e2-a38b-b77fa26e5d30"
            }
          ]
        },
        {
          "id": "70412e21-83b6-4035-b8b6-3491809df4cc",
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
              "id": "5cdbf9ca-3e21-41a3-a808-e7ee5e44d8e2"
            }
          ]
        },
        {
          "id": "14b9755c-eed4-4332-90b4-a164f5e99a22",
          "name": "describeComputeEnvironments",
          "request": {
            "url": "http://example.com/api/?Action=DescribeComputeEnvironments?computeEnvironments=computeEnvironments&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your compute environments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "921f70f7-7418-410f-9571-f28822a2bfd0"
            }
          ]
        }
      ]
    },
    {
      "name": "Job Queue",
      "item": [
        {
          "id": "29bd3fba-fa1c-40e4-91b8-c899ec003eaa",
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
              "id": "15990531-c07f-4bbb-aadb-98c080a77e46"
            }
          ]
        },
        {
          "id": "c94ad5be-ab46-459f-ac40-c63f24bcd444",
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
              "id": "c01d1ca4-026e-448a-b8d7-5e33d0bf9237"
            }
          ]
        },
        {
          "id": "8f1fcb4a-3f63-4636-b8a0-d2f48403a42a",
          "name": "describeJobQueues",
          "request": {
            "url": "http://example.com/api/?Action=DescribeJobQueues?jobQueues=jobQueues&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your job queues."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38fa9a50-2f98-491d-9262-996607e1c12d"
            }
          ]
        }
      ]
    },
    {
      "name": "Job Definitions",
      "item": [
        {
          "id": "99fbb1d2-a26e-43b6-b651-c1d8fb7deab1",
          "name": "deregisterJobDefinition",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterJobDefinition?jobDefinition=jobDefinition",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters an AWS Batch job definition."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f4d2e05-e014-45ae-811c-6f2689394eb5"
            }
          ]
        },
        {
          "id": "a3f7419a-0398-4210-a63c-430edb0f76b4",
          "name": "describeJobDefinitions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeJobDefinitions?jobDefinitionName=jobDefinitionName&jobDefinitions=jobDefinitions&maxResults=maxResults&nextToken=nextToken&status=status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a list of job definitions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "228a6736-14f3-4446-b020-88d5ea628a45"
            }
          ]
        }
      ]
    }
  ]
}