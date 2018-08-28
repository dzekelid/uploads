swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
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