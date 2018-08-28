---
swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 0
info:
  title: AWS Device Farm API Get Upload
  version: 1.0.0
  description: Gets information about an upload.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteUpload:
    get:
      summary: Delete Upload
      description: Deletes an upload given the upload ARN.
      operationId: deleteUpload
      x-api-path-slug: actiondeleteupload-get
      parameters:
      - in: query
        name: arn
        description: Represents the Amazon Resource Name (ARN) of the Device Farm
          upload you wish to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Uploads
  /?Action=ListUploads:
    get:
      summary: List Uploads
      description: Gets information about uploads, given an AWS Device Farm project
        ARN.
      operationId: listUploads
      x-api-path-slug: actionlistuploads-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the project for which you want
          to list uploads
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Uploads
  /?Action=CreateUpload:
    get:
      summary: Create Upload
      description: Uploads an app or test scripts.
      operationId: createUpload
      x-api-path-slug: actioncreateupload-get
      parameters:
      - in: query
        name: contentType
        description: The uploads content type (for example, application/octet-stream)
        type: string
      - in: query
        name: name
        description: The uploads file name
        type: string
      - in: query
        name: projectArn
        description: The ARN of the project for the upload
        type: string
      - in: query
        name: type
        description: The uploads upload type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload
  /?Action=GetUpload:
    get:
      summary: Get Upload
      description: Gets information about an upload.
      operationId: getUpload
      x-api-path-slug: actiongetupload-get
      parameters:
      - in: query
        name: arn
        description: The uploads ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---