---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Allows you to upload a document and attach it directly to a property.
  version: 1.0.0
  description: Allows you to upload a document and attach it directly to a property..
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
  /api/roomdescription/{id}/uploadandattachdocumenttoroom:
    put:
      summary: Uploads and attaches a document to room description room - the new
        document is appended to the current list.
      description: Uploads and attaches a document to room description room - the
        new document is appended to the current list..
      operationId: RoomDescription_UploadAndAttachDocumentToRoomByidByroomIdBydocumentDetails
      x-api-path-slug: apiroomdescriptioniduploadandattachdocumenttoroom-put
      parameters:
      - in: body
        name: documentDetails
        description: Details about the document
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The room description Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roomId
        description: The roomId
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Attaches
      - Document
      - To
      - Room
      - Description
      - Room
      - '-'
      - New
      - Document
      - Is
      - Appended
      - To
      - Current
      - List
  /api/branding/{id}/uploaddocumentcustomisation:
    put:
      summary: Upload the data to customise a Brand Document.
      description: Upload the data to customise a brand document..
      operationId: Branding_UploadDocumentCustomisationByidBycustomisationSaveData
      x-api-path-slug: apibrandingiduploaddocumentcustomisation-put
      parameters:
      - in: body
        name: customisationSaveData
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: BrandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Data
      - To
      - Customise
      - Brand
      - Document
  /api/branding/uploadsmstemplate:
    post:
      summary: Upload the data to create a SMS Document Template for a Brand.
      description: Upload the data to create a sms document template for a brand..
      operationId: Branding_UploadSMSTemplateBybrandTemplateSaveDataContract
      x-api-path-slug: apibrandinguploadsmstemplate-post
      parameters:
      - in: body
        name: brandTemplateSaveDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Data
      - To
      - Create
      - SMS
      - Document
      - Templatea
      - Brand
  /api/branding/uploademailtemplate:
    post:
      summary: Upload the data to create a Email Document Template for a Brand.
      description: Upload the data to create a email document template for a brand..
      operationId: Branding_UploadEmailTemplateBybrandTemplateSaveDataContract
      x-api-path-slug: apibrandinguploademailtemplate-post
      parameters:
      - in: body
        name: brandTemplateSaveDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Data
      - To
      - Create
      - Email
      - Document
      - Templatea
      - Brand
  /api/branding/htmladvert/{brandId}:
    post:
      summary: Upload the a html advert for a brand.
      description: Upload the a html advert for a brand..
      operationId: Branding_UpdateHtmlAdvertBybrandIdBybrandHtmlAdvertDataContract
      x-api-path-slug: apibrandinghtmladvertbrandid-post
      parameters:
      - in: body
        name: brandHtmlAdvertDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Html
      - Adverta
      - Brand
  /api/branding/htmladverts/{brandId}:
    get:
      summary: Upload the a html advert for a brand.
      description: Upload the a html advert for a brand..
      operationId: Branding_HtmlAdvertsBybrandId
      x-api-path-slug: apibrandinghtmladvertsbrandid-get
      parameters:
      - in: path
        name: brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Html
      - Adverta
      - Brand
  /api/progression/lettings/uploadandattachtenantdocument:
    post:
      summary: Allows you to upload a document and attach it directly to a tenant.
      description: Allows you to upload a document and attach it directly to a tenant..
      operationId: LettingsProgression_UploadAndAttachTenantDocumentBytenantInfoIdBydocumentDetailsContract
      x-api-path-slug: apiprogressionlettingsuploadandattachtenantdocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenantInfoId
        description: The tenant Id
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Tenant
  /api/progression/lettings/uploadandattachlandlorddocument:
    post:
      summary: Allows you to upload a document and attach it directly to a tenant.
      description: Allows you to upload a document and attach it directly to a tenant..
      operationId: LettingsProgression_UploadAndAttachLandlordDocumentBylandlordInfoIdBydocumentDetailsContract
      x-api-path-slug: apiprogressionlettingsuploadandattachlandlorddocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: landlordInfoId
        description: The tenant Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Tenant
  /api/progression/lettings/uploadandattachguarantorgroupdocument:
    post:
      summary: Allows you to upload a lettings document and attach it directly to
        a guarantor group.
      description: Allows you to upload a lettings document and attach it directly
        to a guarantor group..
      operationId: LettingsProgression_UploadAndAttachGurantorGroupDocumentByguarantorGroupIdBytenancyIdBydocumentDetai
      x-api-path-slug: apiprogressionlettingsuploadandattachguarantorgroupdocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: guarantorGroupId
        description: The guarantor group Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenancyId
        description: The tenancy Id
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Lettings
      - Document
      - Attach
      - It
      - Directly
      - To
      - Guarantor
      - Group
  /api/progression/lettings/uploadandattachguarantordocument:
    post:
      summary: Allows you to upload a document and attach it directly to a guarantor.
      description: Allows you to upload a document and attach it directly to a guarantor..
      operationId: LettingsProgression_UploadAndAttachGuarantorDocumentByguarantorIdBydocumentDetailsContract
      x-api-path-slug: apiprogressionlettingsuploadandattachguarantordocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: guarantorId
        description: The guarantor Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Guarantor
  /api/progression/lettings/uploadandattachguarantorreferencedocument:
    post:
      summary: Allows you to upload a document and attach it directly to a guarantor.
      description: Allows you to upload a document and attach it directly to a guarantor..
      operationId: LettingsProgression_UploadAndAttachGuarantorReferenceDocumentByguarantorIdByreferenceIdBydocumentDet
      x-api-path-slug: apiprogressionlettingsuploadandattachguarantorreferencedocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: guarantorId
        description: The guarantor Id
      - in: query
        name: referenceId
        description: The reference Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Guarantor
  /api/progression/lettings/uploadandattachrighttorentdocument:
    post:
      summary: Allows you to upload a document and attach it directly to a r ight
        to rent.
      description: Allows you to upload a document and attach it directly to a r ight
        to rent..
      operationId: LettingsProgression_UploadAndAttachRightToRentDocumentBytenantInfoIdBydocumentDetailsContract
      x-api-path-slug: apiprogressionlettingsuploadandattachrighttorentdocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenantInfoId
        description: The tenant info Id
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - R
      - Ight
      - To
      - Rent
  /api/progression/lettings/uploadandattachtenantreferencedocument:
    post:
      summary: Allows you to upload a document and attach it directly to a guarantor.
      description: Allows you to upload a document and attach it directly to a guarantor..
      operationId: LettingsProgression_UploadAndAttachTenantReferenceDocumentBytenantInfoIdByreferenceIdBytenantRoleIdB
      x-api-path-slug: apiprogressionlettingsuploadandattachtenantreferencedocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: referenceId
        description: The reference Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenantInfoId
        description: The tenantInfoId Id
      - in: query
        name: tenantRoleId
        description: The reference Id
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Guarantor
  /api/milestone/{id}/uploadandattachdocument:
    post:
      summary: Allows you to upload a document and attach it directly to a milestone.
      description: Allows you to upload a document and attach it directly to a milestone..
      operationId: Milestone_UploadAndAttachDocumentByidBydocumentDetailsContract
      x-api-path-slug: apimilestoneiduploadandattachdocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        description: Document save command
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The milestone Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Milestone
  /api/negotiator/my/preferences/emailsignature:
    post:
      summary: Allows you to upload a document for use as email signature
      description: Allows you to upload a document for use as email signature.
      operationId: Negotiator_UploadEmailSignatureBydocumentDetailsContract
      x-api-path-slug: apinegotiatormypreferencesemailsignature-post
      parameters:
      - in: body
        name: documentDetailsContract
        description: Document details
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Documentuse
      - As
      - Email
      - Signature
  /api/property/{id}/uploadandattachdocument:
    post:
      summary: Allows you to upload a document and attach it directly to a property.
      description: Allows you to upload a document and attach it directly to a property..
      operationId: Property_UploadAndAttachDocumentByidBydocumentDetailsContract
      x-api-path-slug: apipropertyiduploadandattachdocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        description: Details o
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Property
  /api/property/uploadandattachcertificatedocument:
    post:
      summary: Allows you to upload a document and attach it directly to a guarantor.
      description: Allows you to upload a document and attach it directly to a guarantor..
      operationId: Property_UploadAndAttachCertificateDocumentBycertificateIdBydocumentDetailsContract
      x-api-path-slug: apipropertyuploadandattachcertificatedocument-post
      parameters:
      - in: query
        name: certificateId
        description: The Certificate Id
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Guarantor
  /api/role/{id}/uploadandattachdocument:
    post:
      summary: Allows you to upload a document and attach it directly to a role.
      description: Allows you to upload a document and attach it directly to a role..
      operationId: Role_UploadAndAttachDocumentByidBydocumentDetailsContract
      x-api-path-slug: apiroleiduploadandattachdocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The role Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
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