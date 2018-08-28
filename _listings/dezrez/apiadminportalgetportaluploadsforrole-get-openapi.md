---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get all the live portal uploads associated with a property marketing
    role
  version: 1.0.0
  description: Get all the live portal uploads associated with a property marketing
    role.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/branding/{id}/uploadandattachdocument:
    put:
      summary: Uploads and attaches a document to a brand.
      description: Uploads and attaches a document to a brand..
      operationId: Branding_UploadAndAttachDocumentByidBydocumentDetails
      x-api-path-slug: apibrandingiduploadandattachdocument-put
      parameters:
      - in: body
        name: documentDetails
        description: Details of the file
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Attaches
      - Document
      - To
      - Brand
  /api/branding/{id}/uploadandattachdocumenttodefault:
    put:
      summary: Uploads and attaches a document to a brand.
      description: Uploads and attaches a document to a brand..
      operationId: Branding_UploadAndAttachDocumentToDefaultBrandBydocumentDetailsByid
      x-api-path-slug: apibrandingiduploadandattachdocumenttodefault-put
      parameters:
      - in: body
        name: documentDetails
        description: Details of the file
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Attaches
      - Document
      - To
      - Brand
  /api/documentgeneration/createlettertemplate:
    post:
      summary: Uploads a new letter template
      description: Uploads a new letter template.
      operationId: DocumentGeneration_CreateLetterTemplateByletterTemplate
      x-api-path-slug: apidocumentgenerationcreatelettertemplate-post
      parameters:
      - in: body
        name: letterTemplate
        description: The letter template
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - New
      - Letter
      - Template
  /api/documentgeneration/createheadertemplate/{brandId}:
    post:
      summary: Uploads a new header template
      description: Uploads a new header template.
      operationId: DocumentGeneration_CreateHeaderTemplateBybrandIdByletterTemplate
      x-api-path-slug: apidocumentgenerationcreateheadertemplatebrandid-post
      parameters:
      - in: path
        name: brandId
        description: Brand Id for this header
      - in: body
        name: letterTemplate
        description: The letter template
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - New
      - Header
      - Template
  /api/group/{id}/uploadandattachdocument:
    post:
      summary: Uploads a new document and attaches it to the specified group.
      description: Uploads a new document and attaches it to the specified group..
      operationId: Group_UploadAndAttachDocumentByidBydocumentDetails
      x-api-path-slug: apigroupiduploadandattachdocument-post
      parameters:
      - in: body
        name: documentDetails
        description: The document details
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The identifier
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - New
      - Document
      - Attaches
      - It
      - To
      - Specified
      - Group
  /api/progression/lettings/{roleId}/inventory/uploaddocument:
    post:
      summary: Uploads an inventory document for a tenant role
      description: Uploads an inventory document for a tenant role.
      operationId: LettingsProgression_UploadAndAttachInventoryDocumentByroleIdBydocumentSaveCommand
      x-api-path-slug: apiprogressionlettingsroleidinventoryuploaddocument-post
      parameters:
      - in: body
        name: documentSaveCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
        description: Tenant role id
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Inventory
      - Documenta
      - Tenant
      - Role
  /api/admin/portal/getportaluploadsforrole:
    get:
      summary: Get all the live portal uploads associated with a property marketing
        role
      description: Get all the live portal uploads associated with a property marketing
        role.
      operationId: Portal_GetLivePortalInformationRecordsForRoleByroleId
      x-api-path-slug: apiadminportalgetportaluploadsforrole-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Live
      - Portal
      - Uploads
      - Associated
      - Property
      - Marketing
      - Role
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