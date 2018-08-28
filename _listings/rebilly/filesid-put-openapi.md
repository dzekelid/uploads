---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Update the File with predefined ID. Note that file can be uploaded
    with POST only.
  description: Update the File with predefined ID
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{id}:
    put:
      summary: Update the File with predefined ID. Note that file can be uploaded
        with POST only.
      description: Update the File with predefined ID
      operationId: files.id.put
      x-api-path-slug: filesid-put
      parameters:
      - in: body
        name: body
        description: File resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - File
      - Predefined
      - ID
      - ""
      - Note
      - That
      - File
      - Can
      - Be
      - Uploaded
      - POST
      - Only
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