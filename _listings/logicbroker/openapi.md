swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 1
info:
  title: CommerceAPI
  version: 1.0.0
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Attachments:
    post:
      summary: Upload an attachment
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Attachment_Upload
      x-api-path-slug: apiv1attachments-post
      parameters:
      - in: body
        name: data
        description: XML/JSON data to attach (webhooks)
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: description
        description: Attachment description
      - in: formData
        name: file
        description: File to attach
      - in: query
        name: logicbrokerKey
        description: Logicbroker key to attach
      - in: query
        name: notify
        description: If true, create an activty event
      - in: query
        name: receiverId
        description: Receiver account number
      - in: query
        name: type
        description: Attachment type (json, xml, csv, txt, pdf, png)
      - in: query
        name: url
        description: URL of file to attach
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Attachment