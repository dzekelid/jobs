{
  "info": {
    "name": "AWS Device Farm API Get Job",
    "_postman_id": "9767998a-7477-40f5-be93-0b7c58b5797b",
    "description": "Gets information about a job.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device Pool",
      "item": [
        {
          "id": "99bb797c-0c80-4178-b52c-38cac591f6b7",
          "name": "createDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=CreateDevicePool?description=description&name=name&projectArn=projectArn&rules=rules",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "449628c1-8aa8-4d17-9ba0-357079cff823"
            }
          ]
        },
        {
          "id": "540d733a-d828-4b7a-921c-d2f85a5fb3e5",
          "name": "deleteDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDevicePool?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a device pool given the pool ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "adfafa73-67ac-45e0-bbf9-9ffa17fec33e"
            }
          ]
        },
        {
          "id": "d36a90f2-86ca-42ef-8198-fc75799aebdf",
          "name": "getDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=GetDevicePool?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18020fc8-316b-40cb-b2a6-7289e0888747"
            }
          ]
        },
        {
          "id": "e5c9ca58-1c65-4ef0-8480-105aa962f138",
          "name": "getDevicePoolCompatibility",
          "request": {
            "url": "http://example.com/api/?Action=GetDevicePoolCompatibility?appArn=appArn&devicePoolArn=devicePoolArn&testType=testType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about compatibility with a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63d9bfc0-3be0-4bc7-9acc-66536454bec7"
            }
          ]
        }
      ]
    },
    {
      "name": "Project",
      "item": [
        {
          "id": "47092082-7c7e-46db-b475-5c26c034c027",
          "name": "createProject",
          "request": {
            "url": "http://example.com/api/?Action=CreateProject?name=name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cb017da-ee07-41cc-9219-878010b53e2c"
            }
          ]
        }
      ]
    },
    {
      "name": "Remote Access Sessions",
      "item": [
        {
          "id": "a5e197d3-f893-471a-a84b-208674aeacc6",
          "name": "createRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=CreateRemoteAccessSession?configuration=configuration&deviceArn=deviceArn&name=name&projectArn=projectArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Specifies and starts a remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a04f46c-8464-4ccb-b95a-062a78016351"
            }
          ]
        },
        {
          "id": "e96f7fe8-79e9-45ed-bac8-e8ec3aac1b57",
          "name": "deleteRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRemoteAccessSession?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a completed remote access session and its results."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "395c8fa2-af38-4c1a-9318-a9a119e3e2eb"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "255e7bc3-92f9-4229-9153-a6e666e6f206",
          "name": "createUpload",
          "request": {
            "url": "http://example.com/api/?Action=CreateUpload?contentType=contentType&name=name&projectArn=projectArn&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Uploads an app or test scripts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c30850e-7067-4f40-a279-e1b978d0f2bd"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "5a240335-67ad-469c-8957-c4e72a569ea5",
          "name": "deleteProject",
          "request": {
            "url": "http://example.com/api/?Action=DeleteProject?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an AWS Device Farm project, given the project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2dbff89a-585d-46ac-be24-b89094342199"
            }
          ]
        }
      ]
    },
    {
      "name": "Runs",
      "item": [
        {
          "id": "b593e4a7-a8e6-4855-b637-55f8cafd7e36",
          "name": "deleteRun",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRun?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the run, given the run ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38386877-4e01-4b5b-9f12-f2dc6bfb6e24"
            }
          ]
        }
      ]
    },
    {
      "name": "Uploads",
      "item": [
        {
          "id": "3f08e1b4-bedc-4f80-a0a1-569bab3ff73b",
          "name": "deleteUpload",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUpload?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an upload given the upload ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa713db8-35ac-4b4b-b556-b5a3800e5a12"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Settings",
      "item": [
        {
          "id": "bec81bf9-5b61-474b-903f-49599d903fd2",
          "name": "getAccountSettings",
          "request": {
            "url": "http://example.com/api/?Action=GetAccountSettings?accountSettings=accountSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the number of unmetered iOS and/or unmetered Android devices that have been purchased by the account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "443a6201-7fa5-4a83-8b5d-e30e6f4f1f9d"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "4952e122-ab30-4bb3-8ddd-8e94d60fcf2d",
          "name": "getDevice",
          "request": {
            "url": "http://example.com/api/?Action=GetDevice?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a unique device type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e76a2481-9331-4985-8bfa-a5bbe3368e7d"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "24504ebf-8023-423b-95ac-4a59086715da",
          "name": "getJob",
          "request": {
            "url": "http://example.com/api/?Action=GetJob?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3032a7f8-21de-49ea-946b-aac47e5b1ac6"
            }
          ]
        }
      ]
    }
  ]
}