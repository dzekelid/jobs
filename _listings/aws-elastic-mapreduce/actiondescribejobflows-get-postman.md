{
  "info": {
    "name": "AWS Elastic MapReduce API Describe Job Flows",
    "_postman_id": "b0c5dbdf-e785-45e9-8ffc-62a5e91b5920",
    "description": "This API is deprecated and will eventually be removed.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Instance Groups",
      "item": [
        {
          "id": "1ac55502-e189-4eab-8b5d-a57727e987a2",
          "name": "addInstanceGroups",
          "request": {
            "url": "http://example.com/api/?Action=AddInstanceGroups?InstanceGroups=InstanceGroups&JobFlowId=JobFlowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds one or more instance groups to a running cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5d22519-82cd-4a1e-bc8e-170d492033e4"
            }
          ]
        }
      ]
    },
    {
      "name": "Job Flow Steps",
      "item": [
        {
          "id": "031747c8-17d0-40f6-8da2-6546004c8e39",
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
              "id": "589cb447-dbcb-4f53-9b1b-f18dd0cba8d3"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "71a2365a-7fa9-4987-80b7-57699420be2e",
          "name": "addTags",
          "request": {
            "url": "http://example.com/api/?Action=AddTags?ResourceId=ResourceId&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds tags to an Amazon EMR resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc8b25a7-4646-45c6-96e9-a00cf44be290"
            }
          ]
        }
      ]
    },
    {
      "name": "Steps",
      "item": [
        {
          "id": "185fdde0-65cc-40fb-9388-fc22cdd56445",
          "name": "cancelSteps",
          "request": {
            "url": "http://example.com/api/?Action=CancelSteps?ClusterId=ClusterId&StepIds=StepIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels a pending step or steps in a running cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ea84913-d527-4237-b603-419b60775fb3"
            }
          ]
        }
      ]
    },
    {
      "name": "Security Configurations",
      "item": [
        {
          "id": "1909a50a-d583-4001-a576-ab3e20a0613f",
          "name": "createSecurityConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=CreateSecurityConfiguration?Name=Name&SecurityConfiguration=SecurityConfiguration",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a security configuration, which is stored in the service and can be specified when a cluster is created."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2baadca-646f-4be5-9305-9a91fc54cee4"
            }
          ]
        },
        {
          "id": "78e66491-f246-4393-b502-20099c1c0b48",
          "name": "deleteSecurityConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSecurityConfiguration?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a security configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "003faeb2-78a4-488c-b35e-af4902098184"
            }
          ]
        }
      ]
    },
    {
      "name": "Clusters",
      "item": [
        {
          "id": "dd8673cc-d669-412e-a0f7-b54bacbe1c86",
          "name": "describeCluster",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCluster?ClusterId=ClusterId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides cluster-level details including status, hardware and software configuration, VPC settings, and so on."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2996882-d6dd-49b4-bc75-008548748051"
            }
          ]
        }
      ]
    },
    {
      "name": "Job Flows",
      "item": [
        {
          "id": "f20d3628-9b54-4476-ad50-9d34afa6f4b7",
          "name": "describeJobFlows",
          "request": {
            "url": "http://example.com/api/?Action=DescribeJobFlows?CreatedAfter=CreatedAfter&CreatedBefore=CreatedBefore&JobFlowIds=JobFlowIds&JobFlowStates=JobFlowStates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API is deprecated and will eventually be removed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ed50439-ac46-4fb4-bd89-51d6aa8a08bd"
            }
          ]
        }
      ]
    }
  ]
}