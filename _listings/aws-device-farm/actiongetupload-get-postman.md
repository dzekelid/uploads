{
  "info": {
    "name": "AWS Device Farm API Get Upload",
    "_postman_id": "d4e9b87e-27b7-4cc0-b143-28e97f9f2139",
    "description": "Gets information about an upload.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device Pool",
      "item": [
        {
          "id": "726e9a99-1fa8-4009-b7e1-59d6512f1ebd",
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
              "id": "5191a3bd-df6f-4abc-ae7f-cf0c36d3b326"
            }
          ]
        },
        {
          "id": "8dbe8146-a099-4dd5-be8f-ddded488179e",
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
              "id": "7fcddc1b-ae6d-4763-8cb6-a965613e2688"
            }
          ]
        },
        {
          "id": "02bc5769-5d6f-4701-98d9-33ae6a8daf14",
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
              "id": "72010fd7-fba9-4927-a04f-e5611e698c55"
            }
          ]
        },
        {
          "id": "a35239c3-a513-409b-bf21-2319ee67bc53",
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
              "id": "02b1f46f-6798-43d5-8c31-a6a1145fc0b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Project",
      "item": [
        {
          "id": "a5d04a08-143f-45e0-8237-d7e492aad376",
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
              "id": "608185df-5353-4e67-8967-70caa42010df"
            }
          ]
        }
      ]
    },
    {
      "name": "Remote Access Sessions",
      "item": [
        {
          "id": "e9964918-d470-4846-a00d-1324637da023",
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
              "id": "2af20cae-d12d-4531-aaee-2414ff2e3555"
            }
          ]
        },
        {
          "id": "a84858a2-c631-4281-a5ce-3cef851d5896",
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
              "id": "172c283d-7900-420f-9b26-ed4b8fcdb3f7"
            }
          ]
        },
        {
          "id": "cdf42248-760c-418c-a963-7e4289034952",
          "name": "getRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=GetRemoteAccessSession?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a link to a currently running remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "742fb699-8a78-4e21-8700-17055d1fe2fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "683cc4f8-af03-4ac3-aba3-22b788407156",
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
              "id": "b68418bc-2c08-4d9a-ac28-5c4cdaac5516"
            }
          ]
        },
        {
          "id": "e6f8090b-daa8-4f67-bd1a-0d74ceb0f936",
          "name": "getUpload",
          "request": {
            "url": "http://example.com/api/?Action=GetUpload?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about an upload."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8be254b6-a59c-4713-bd45-2963724df2cf"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "40322b36-89bc-4844-8b90-c4209632201e",
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
              "id": "ba5f125a-4070-4214-aa55-27b925846dfa"
            }
          ]
        },
        {
          "id": "dfb6f776-1db1-47cd-ba76-3a8664860491",
          "name": "getProject",
          "request": {
            "url": "http://example.com/api/?Action=GetProject?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90dba237-0664-40f0-a396-20502dae0928"
            }
          ]
        }
      ]
    },
    {
      "name": "Runs",
      "item": [
        {
          "id": "25fb4d44-af8c-4191-ac4b-2b8bfabf77fb",
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
              "id": "5d17d653-99fb-41aa-8409-9204507bd13e"
            }
          ]
        },
        {
          "id": "919a7a67-dd92-4164-890c-d2715f1fef0f",
          "name": "getRun",
          "request": {
            "url": "http://example.com/api/?Action=GetRun?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e1abcd6-46b1-4f12-a95f-1d38a00d1443"
            }
          ]
        }
      ]
    },
    {
      "name": "Uploads",
      "item": [
        {
          "id": "38c5e356-d512-4d51-a5eb-dbd13a747413",
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
              "id": "3820d6f3-1bab-4b02-b529-772a94a850bc"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Settings",
      "item": [
        {
          "id": "635feb8b-8258-44cd-a917-081e7251fea1",
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
              "id": "71abb25e-173d-4211-bdad-9e507beec8b0"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "10092a7f-3a88-412c-87d9-c738f7fe41f0",
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
              "id": "58ed1a07-30ed-451b-87f5-edbd17b547ac"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "0115ade3-00bc-4bea-a057-027a6dd94c5d",
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
              "id": "89c0834f-6682-4953-b139-1f6804011a15"
            }
          ]
        }
      ]
    },
    {
      "name": "Offering Status",
      "item": [
        {
          "id": "1dfdcab4-69d0-422f-a8d4-005d6b9a8130",
          "name": "getOfferingStatus",
          "request": {
            "url": "http://example.com/api/?Action=GetOfferingStatus?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the current status and future status of all offerings purchased by an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e632814-427c-4647-a4ab-bedeb0a210ce"
            }
          ]
        }
      ]
    },
    {
      "name": "Suites",
      "item": [
        {
          "id": "7eb359d5-68d0-4302-a44c-da4fcdf8d2b8",
          "name": "getSuite",
          "request": {
            "url": "http://example.com/api/?Action=GetSuite?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a suite."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b558713-2b04-42f8-aed6-18b009245ece"
            }
          ]
        }
      ]
    },
    {
      "name": "Tests",
      "item": [
        {
          "id": "c694fe47-6c90-4b5f-ba3a-c81c0ad603ab",
          "name": "getTest",
          "request": {
            "url": "http://example.com/api/?Action=GetTest?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a test."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "372d9497-6d7e-4fd4-b040-b25b83c744de"
            }
          ]
        }
      ]
    }
  ]
}