swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 1
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddUploadBuffer:
    get:
      summary: Add Upload Buffer
      description: Configures one or more gateway local disks as upload buffer for
        a specified gateway.
      operationId: addUploadBuffer
      x-api-path-slug: actionadduploadbuffer-get
      parameters:
      - in: query
        name: DiskIds
        description: 'Type: array of Strings'
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload Buffer
  /?Action=DescribeUploadBuffer:
    get:
      summary: Describe Upload Buffer
      description: Returns information about the upload buffer of a gateway.
      operationId: describeUploadBuffer
      x-api-path-slug: actiondescribeuploadbuffer-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload Buffer