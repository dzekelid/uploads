---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Add API Kycdocumentupload
  version: 1.0.0
  description: Add api kycdocumentupload.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/CheckDocumentsToUpload:
    get:
      summary: Get API Checkdocumentstoupload
      description: Get api checkdocumentstoupload.
      operationId: ApiCheckDocumentsToUploadGet
      x-api-path-slug: apicheckdocumentstoupload-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Checkdocumentstoupload
  /api/KycDocumentUpload:
    post:
      summary: Add API Kycdocumentupload
      description: Add api kycdocumentupload.
      operationId: ApiKycDocumentUploadPost
      x-api-path-slug: apikycdocumentupload-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: idType
      - in: formfile
        name: photo
      - in: query
        name: type
      - in: formfile
        name: userFile
      responses:
        200:
          description: OK
      tags:
      - Kycdocumentupload
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