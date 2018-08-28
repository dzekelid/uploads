---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Upload an attachment
  version: 1.0.0
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
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