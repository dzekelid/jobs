{
  "info": {
    "name": "AWS Code Pipeline API Acknowledge Job",
    "_postman_id": "df201b5d-bd3e-4f78-9de4-01ec0f068855",
    "description": "Returns information about a specified job and whether that job has been received by\n            the job worker.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acknowledge",
      "item": [
        {
          "id": "f34fc1f6-5c6f-47c0-baaa-4fabed044e21",
          "name": "acknowledgeJob",
          "request": {
            "url": "http://example.com/api/?Action=AcknowledgeJob?DryRun=DryRun&jobId=jobId&nonce=nonce&SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specified job and whether that job has been received by\n            the job worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35738d01-3fee-40f3-8b92-99015bdc5b83"
            }
          ]
        }
      ]
    }
  ]
}