{
  "info": {
    "name": "AWS Snowball API Get Job Manifest",
    "_postman_id": "999f6705-05fb-419d-aacb-070febed4a9d",
    "description": "Returns a link to an Amazon S3 presigned URL for the manifest file associated with the\n      specified JobId value.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clusters",
      "item": [
        {
          "id": "5c1cd857-1671-419a-ad36-945f35561d55",
          "name": "cancelCluster",
          "request": {
            "url": "http://example.com/api/?Action=CancelCluster?ClusterId=ClusterId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels a cluster job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45118f2e-cffa-4453-bcb0-b5b8654059d6"
            }
          ]
        },
        {
          "id": "241ccc73-f5a2-49c1-a92b-ccd25c04041a",
          "name": "createCluster",
          "request": {
            "url": "http://example.com/api/?Action=CreateCluster?AddressId=AddressId&Description=Description&JobType=JobType&KmsKeyARN=KmsKeyARN&Notification=Notification&Resources=Resources&RoleARN=RoleARN&ShippingOption=ShippingOption&SnowballType=SnowballType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an empty cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60dc9ab2-df3f-41f2-9e6d-123da1811d47"
            }
          ]
        },
        {
          "id": "ca6c9d56-647d-4d5e-b70a-a1e8f31b1a09",
          "name": "describeCluster",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCluster?ClusterId=ClusterId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific cluster including shipping information, cluster\n      status, and other important metadata."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf2c98f8-a8ed-4e10-a1cb-c4a0b7331cff"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "56b2765d-7930-4901-8215-c85b86491867",
          "name": "cancelJob",
          "request": {
            "url": "http://example.com/api/?Action=CancelJob?JobId=JobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels the specified job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "514acab9-339c-4c3d-87b1-551cf070808d"
            }
          ]
        },
        {
          "id": "1ca655d7-a337-4738-86a7-2eeaa128be5a",
          "name": "createJob",
          "request": {
            "url": "http://example.com/api/?Action=CreateJob?AddressId=AddressId&ClusterId=ClusterId&Description=Description&JobType=JobType&KmsKeyARN=KmsKeyARN&Notification=Notification&Resources=Resources&RoleARN=RoleARN&ShippingOption=ShippingOption&SnowballCapacityPreference=SnowballCapacityPreference&SnowballType=SnowballType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a job to import or export data between Amazon S3 and your on-premises data\n      center."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1cc00eb4-1ae8-48f5-beb9-e01235203cde"
            }
          ]
        },
        {
          "id": "a5c0bb30-bdac-4e61-acfb-c4ebcbabc825",
          "name": "describeJob",
          "request": {
            "url": "http://example.com/api/?Action=DescribeJob?JobId=JobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific job including shipping information, job status,\n      and other important metadata."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a966689-4a28-47b7-9ca5-cc0010f34734"
            }
          ]
        }
      ]
    },
    {
      "name": "Addresses",
      "item": [
        {
          "id": "cf4bdc3d-47ba-4e06-b3d6-ca9f22e31e40",
          "name": "createAddress",
          "request": {
            "url": "http://example.com/api/?Action=CreateAddress?Address=Address",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an address for a Snowball to be shipped to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66d62f66-4733-4e51-8939-269a674e0f34"
            }
          ]
        },
        {
          "id": "07ddfb1d-2608-4384-a20d-7a4709302f13",
          "name": "describeAddress",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAddress?AddressId=AddressId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Takes an AddressId and returns specific details about that address in the\n      form of an Address object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebda62c2-81a1-4656-beaa-2f0e253acd3d"
            }
          ]
        },
        {
          "id": "bfdc57fc-80f3-48bc-b09d-d7b539c50f5c",
          "name": "describeAddresses",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAddresses?MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a specified number of ADDRESS objects."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10220122-05c3-4a86-9e84-5994103481a9"
            }
          ]
        }
      ]
    },
    {
      "name": "Job Manifest",
      "item": [
        {
          "id": "72fed488-e9f8-4f6e-aa8b-506d32cda621",
          "name": "getJobManifest",
          "request": {
            "url": "http://example.com/api/?Action=GetJobManifest?JobId=JobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a link to an Amazon S3 presigned URL for the manifest file associated with the\n      specified JobId value."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07cc80fc-302e-4168-9254-1d69e44c3ac5"
            }
          ]
        }
      ]
    }
  ]
}