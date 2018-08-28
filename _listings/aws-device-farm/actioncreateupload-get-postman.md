{
  "info": {
    "name": "AWS Device Farm API Create Upload",
    "_postman_id": "870363b0-8faf-4c71-acfb-805886245779",
    "description": "Uploads an app or test scripts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device Pool",
      "item": [
        {
          "id": "de5d6671-569b-446a-b98f-052adf784ca5",
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
              "id": "99104771-f2f4-4001-8d0a-e85d6eb853d8"
            }
          ]
        }
      ]
    },
    {
      "name": "Project",
      "item": [
        {
          "id": "8f19d9fc-0834-4e37-a366-e4da0d4732fa",
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
              "id": "d6e5216f-2f63-424c-8c56-ec2f90881111"
            }
          ]
        }
      ]
    },
    {
      "name": "Remote Access Sessions",
      "item": [
        {
          "id": "31d47e70-5494-4036-98fb-b24c58759d3a",
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
              "id": "306847bf-e5bd-4eb3-aa53-6e171d7b17a8"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "c4a6b442-f104-4ee6-a9ce-74005f6fca43",
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
              "id": "e5f37669-8a5d-4340-bb38-2426995625df"
            }
          ]
        }
      ]
    }
  ]
}