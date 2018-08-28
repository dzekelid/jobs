{
  "info": {
    "name": "AWS Elastic MapReduce API Run Job Flow",
    "_postman_id": "36dcbd23-1814-4710-aba9-2ced91452a22",
    "description": "RunJobFlow creates and starts running a new job flow.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Instance Groups",
      "item": [
        {
          "id": "6e9c552f-939c-4ec8-a14e-eb0b8ab2d578",
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
              "id": "46d4302a-1d1d-43f2-9351-085e1540e78b"
            }
          ]
        },
        {
          "id": "de24c888-b26d-4feb-8c6c-703aa6e8ae7e",
          "name": "listInstanceGroups",
          "request": {
            "url": "http://example.com/api/?Action=ListInstanceGroups?ClusterId=ClusterId&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides all available details about the instance groups in a cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0c8f88a-2e70-4aae-a342-54457a3d00fb"
            }
          ]
        },
        {
          "id": "43b47df9-fa51-4b5f-921a-dbff4bacfa8d",
          "name": "modifyInstanceGroups",
          "request": {
            "url": "http://example.com/api/?Action=ModifyInstanceGroups?ClusterId=ClusterId&InstanceGroups=InstanceGroups",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "ModifyInstanceGroups modifies the number of nodes and configuration settings of an instance group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "289e9088-ddc4-4cd0-9569-637a4b967903"
            }
          ]
        }
      ]
    },
    {
      "name": "Job Flow Steps",
      "item": [
        {
          "id": "988a137e-6fc6-442a-8e89-04ff5f4cdd4b",
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
              "id": "a9c9227b-cabe-4a07-a7c6-07d332f2ad7d"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "b6b88b9c-a1ba-4fe0-a5e4-e06e34321fbd",
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
              "id": "6b8369d1-cfbf-4705-8fef-de4c494f2959"
            }
          ]
        },
        {
          "id": "7806f711-8b51-4ced-8818-51de68277ad9",
          "name": "removeTags",
          "request": {
            "url": "http://example.com/api/?Action=RemoveTags?ResourceId=ResourceId&TagKeys=TagKeys",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes tags from an Amazon EMR resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e03a359-2903-4b14-9725-364e8921d66a"
            }
          ]
        }
      ]
    },
    {
      "name": "Steps",
      "item": [
        {
          "id": "4428e41a-6a7e-4cc8-a972-d427b819c5fe",
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
              "id": "9f6a09d4-dc89-46c1-9e4b-589f026d78a6"
            }
          ]
        },
        {
          "id": "acabf858-b87e-4ab6-a9a8-3e453325c212",
          "name": "describeStep",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStep?ClusterId=ClusterId&StepId=StepId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides more detail about the cluster step."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c522285-34b2-4e53-8981-40a548fe9861"
            }
          ]
        },
        {
          "id": "815086d9-7b68-4ae4-853f-94c90ff597f2",
          "name": "listSteps",
          "request": {
            "url": "http://example.com/api/?Action=ListSteps?ClusterId=ClusterId&Marker=Marker&StepIds=StepIds&StepStates=StepStates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides a list of steps for the cluster in reverse order unless you specify stepIds with the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b5a0229-ad01-4f33-b796-470dda0369bd"
            }
          ]
        }
      ]
    },
    {
      "name": "Security Configurations",
      "item": [
        {
          "id": "eea204df-60fd-446a-9a0b-3ce241209de5",
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
              "id": "462cc72a-0f1f-49eb-988e-d372bdbe367d"
            }
          ]
        },
        {
          "id": "5365ede8-26bb-4184-bf2b-8ade3e24907c",
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
              "id": "06f3cce8-407d-4708-80cc-f24a18a77dcc"
            }
          ]
        },
        {
          "id": "19b1d14d-f81d-41c8-add8-cd932b98df03",
          "name": "describeSecurityConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSecurityConfiguration?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides the details of a security configuration by returning the configuration JSON."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "566954b7-5dc7-48b2-91d0-20b150f16eee"
            }
          ]
        },
        {
          "id": "bb64fbda-9d87-42df-95e2-8763d4d90960",
          "name": "listSecurityConfigurations",
          "request": {
            "url": "http://example.com/api/?Action=ListSecurityConfigurations?Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the security configurations visible to this account, providing their creation dates and times, and their names."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85179652-37bf-430c-99a9-cfb6b68c9bfd"
            }
          ]
        }
      ]
    },
    {
      "name": "Clusters",
      "item": [
        {
          "id": "35423ea5-93b3-4c2d-a4e4-8aea0a004ff1",
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
              "id": "8cf1678c-e6f5-486c-8a49-0e7d274f5f6b"
            }
          ]
        },
        {
          "id": "61ffd7d6-0acc-417c-aff2-084fd0bcfce2",
          "name": "listClusters",
          "request": {
            "url": "http://example.com/api/?Action=ListClusters?ClusterStates=ClusterStates&CreatedAfter=CreatedAfter&CreatedBefore=CreatedBefore&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides the status of all clusters visible to this AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14150be5-58dc-4857-b0d2-2a2eab480758"
            }
          ]
        }
      ]
    },
    {
      "name": "Job Flows",
      "item": [
        {
          "id": "edfd42e3-548e-4f48-982d-c79b36703511",
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
              "id": "47d096c0-6880-4de5-a961-92de9f664330"
            }
          ]
        },
        {
          "id": "09ff639f-6c9f-4cad-aa27-577c043a64ce",
          "name": "runJobFlow",
          "request": {
            "url": "http://example.com/api/?Action=RunJobFlow?AdditionalInfo=AdditionalInfo&AmiVersion=AmiVersion&Applications=Applications&AutoScalingRole=AutoScalingRole&BootstrapActions=BootstrapActions&Configurations=Configurations&Instances=Instances&JobFlowRole=JobFlowRole&LogUri=LogUri&Name=Name&NewSupportedProducts=NewSupportedProducts&ReleaseLabel=ReleaseLabel&ScaleDownBehavior=ScaleDownBehavior&SecurityConfiguration=SecurityConfiguration&ServiceRole=ServiceRole&Steps=Steps&SupportedProducts=SupportedProducts&Tags=Tags&VisibleToAllUsers=VisibleToAllUsers",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "RunJobFlow creates and starts running a new job flow."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d85fafcb-0610-4119-99eb-1e5eef72ba5b"
            }
          ]
        }
      ]
    },
    {
      "name": "Bootstrap Actions",
      "item": [
        {
          "id": "90166cc2-e32c-4d45-9dbc-4a8a8037091f",
          "name": "listBootstrapActions",
          "request": {
            "url": "http://example.com/api/?Action=ListBootstrapActions?ClusterId=ClusterId&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides information about the bootstrap actions associated with a cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88943780-f2b8-4df8-a0f3-0218022e311f"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "30738e68-67a5-4855-a3b4-b672f3b7beb6",
          "name": "listInstances",
          "request": {
            "url": "http://example.com/api/?Action=ListInstances?ClusterId=ClusterId&InstanceGroupId=InstanceGroupId&InstanceGroupTypes=InstanceGroupTypes&InstanceStates=InstanceStates&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides information about the cluster instances that Amazon EMR provisions on behalf of a user \n         when it creates the cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c733e643-d6e6-4909-b446-d8de90e42b77"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto Scaling Policies",
      "item": [
        {
          "id": "16b1efc0-b517-48c4-911c-9caa718c1886",
          "name": "putAutoScalingPolicy",
          "request": {
            "url": "http://example.com/api/?Action=PutAutoScalingPolicy?AutoScalingPolicy=AutoScalingPolicy&ClusterId=ClusterId&InstanceGroupId=InstanceGroupId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates or updates an automatic scaling policy for a core instance group or task instance group in an Amazon EMR cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f14ebf05-5c66-4868-9156-82fcf65606df"
            }
          ]
        },
        {
          "id": "f6ee1786-c76a-4f6c-8f4b-11ff1a507977",
          "name": "removeAutoScalingPolicy",
          "request": {
            "url": "http://example.com/api/?Action=RemoveAutoScalingPolicy?ClusterId=ClusterId&InstanceGroupId=InstanceGroupId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an automatic scaling policy from a specified instance group within an EMR cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "818b1011-d047-4d0c-9135-86066bc882e1"
            }
          ]
        }
      ]
    }
  ]
}