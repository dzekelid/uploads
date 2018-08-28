---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Upload a layout document
  description: Uploads a layout document to storage. The storage key (i.e. file path)
    must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/contacts/{contactId}/document:
    post:
      summary: Upload a document to contact directory
      description: Upload a document to contact directory.
      operationId: postRestAccountsContactsContactDocument
      x-api-path-slug: restaccountscontactscontactiddocument-post
      parameters:
      - in: path
        name: contactId
      - in: query
        name: key
        description: The storage key for the file to upload
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Document
      - To
      - Contact
      - Directory
  /rest/categories/{categoryId}/documents:
    post:
      summary: Upload category documents
      description: Uploads documents to a category. The ID of the category must be
        specified.
      operationId: postRestCategoriesCategoryDocuments
      x-api-path-slug: restcategoriescategoryiddocuments-post
      parameters:
      - in: body
        name: /rest/categories/{categoryId}/documents
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryId
      - in: query
        name: directoryId
        description: The directory ID
      - in: query
        name: displayDate
        description: The date displayed on the document
      - in: query
        name: documents
        description: The array with the category documents
      - in: query
        name: number
        description: The document number
      - in: query
        name: numberWithPrefix
        description: Number with prefix
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Category
      - Documents
  /rest/items/{id}/images/upload:
    post:
      summary: Upload a new image
      description: Uploads an image. The item ID must be specified.
      operationId: postRestItemsImagesUpload
      x-api-path-slug: restitemsidimagesupload-post
      parameters:
      - in: body
        name: /rest/items/{id}/images/upload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Upload
      - New
      - Image
  /rest/orders/{orderId}/documents/{type}:
    post:
      summary: Upload order documents
      description: Uploads order documents. The ID of the order and the document type
        must be specified.
      operationId: postRestOrdersOrderDocumentsType
      x-api-path-slug: restordersorderiddocumentstype-post
      parameters:
      - in: body
        name: /rest/orders/{orderId}/documents/{type}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Order
      - Documents
  /rest/storage/frontend/file:
    post:
      summary: Upload a single file to frontend storage.
      description: If file is an image, generate a thumbnail and store dimensions
        in metadata.
      operationId: postRestStorageFrontendFile
      x-api-path-slug: reststoragefrontendfile-post
      parameters:
      - in: query
        name: key
        description: The key for the uploaded object
      - in: query
        name: maxAge
        description: Number of seconds until the content of the file expires
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Single
      - File
      - To
      - Frontend
      - Storage
  /rest/storage/layout:
    post:
      summary: Upload a layout document
      description: Uploads a layout document to storage. The storage key (i.e. file
        path) must be specified.
      operationId: postRestStorageLayout
      x-api-path-slug: reststoragelayout-post
      parameters:
      - in: query
        name: key
        description: The storage key for the layout document to upload
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Layout
      - Document
  /rest/storage/plugins/inbox:
    post:
      summary: Upload a file to the inbox
      description: Uploads a file to the inbox. The storage key (i.e. file path) must
        be specified.
      operationId: postRestStoragePluginsInbox
      x-api-path-slug: reststoragepluginsinbox-post
      parameters:
      - in: query
        name: key
        description: The storage key for the file to upload
      responses:
        200:
          description: OK
      tags:
      - Upload
      - File
      - To
      - Inbox
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