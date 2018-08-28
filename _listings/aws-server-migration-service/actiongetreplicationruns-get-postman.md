{
  "info": {
    "name": "AWS Server Migration Service API Get Replication Runs",
    "_postman_id": "4401565c-9aad-4fec-8741-cc78ca857b8c",
    "description": "The get-replication-runs API will return all ReplicationRuns for a given ReplicationJob.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Replication Jobs",
      "item": [
        {
          "id": "9edca283-c932-43f0-8f85-5d6fe5b17f7a",
          "name": "createReplicationJob",
          "request": {
            "url": "http://example.com/api/?Action=CreateReplicationJob?description=description&frequency=frequency&licenseType=licenseType&roleName=roleName&seedReplicationTime=seedReplicationTime&serverId=serverId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The create-replication-job API is used to create a ReplicationJob to replicate a server on AWS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85239792-6d81-4abe-85ac-4a12c36a15fa"
            }
          ]
        },
        {
          "id": "8a0c7988-c3e4-4500-9d62-536cbbfd6213",
          "name": "deleteReplicationJob",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReplicationJob?replicationJobId=replicationJobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The delete-replication-job API is used to delete a ReplicationJob, resulting in no further ReplicationRuns."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1b86ef9-0f91-48c1-bf79-9e8f3dc6d1e8"
            }
          ]
        },
        {
          "id": "08cb7c96-fd5f-4f5b-bd73-c7be557138a3",
          "name": "getReplicationJobs",
          "request": {
            "url": "http://example.com/api/?Action=GetReplicationJobs?maxResults=maxResults&nextToken=nextToken&replicationJobId=replicationJobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The get-replication-jobs API will return all of your ReplicationJobs and their details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11cd6dd0-4504-45cf-ad3c-8c7498b121a8"
            }
          ]
        }
      ]
    },
    {
      "name": "Server Catalog",
      "item": [
        {
          "id": "3345c17d-7ce2-4fab-a26f-30dc66ce18ae",
          "name": "deleteServerCatalog",
          "request": {
            "url": "http://example.com/api/?Action=DeleteServerCatalog",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The delete-server-catalog API clears all servers from your server catalog."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e47ea03-e330-4f29-892e-4604311e4308"
            }
          ]
        }
      ]
    },
    {
      "name": "Connectors",
      "item": [
        {
          "id": "ac942484-1da4-4ee1-93f5-ab21f1873467",
          "name": "disassociateConnector",
          "request": {
            "url": "http://example.com/api/?Action=DisassociateConnector?connectorId=connectorId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The disassociate-connector API will disassociate a connector from the Server Migration Service, rendering it unavailable to support replication jobs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd30fc52-56f7-417e-ae49-2850f6b6a629"
            }
          ]
        },
        {
          "id": "cdc4236a-0672-459a-9d22-efb10bbd49d3",
          "name": "getConnectors",
          "request": {
            "url": "http://example.com/api/?Action=GetConnectors?maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The get-connectors API returns a list of connectors that are registered with the Server Migration Service."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62ccbc6d-2cb4-4823-8d66-c1fd105904da"
            }
          ]
        }
      ]
    },
    {
      "name": "Replication Runs",
      "item": [
        {
          "id": "201acb8b-ce2d-4820-90c1-d4ed485b9bdd",
          "name": "getReplicationRuns",
          "request": {
            "url": "http://example.com/api/?Action=GetReplicationRuns?maxResults=maxResults&nextToken=nextToken&replicationJobId=replicationJobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The get-replication-runs API will return all ReplicationRuns for a given ReplicationJob."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ec85d81-344c-4ea4-8503-c261f69986fe"
            }
          ]
        }
      ]
    }
  ]
}