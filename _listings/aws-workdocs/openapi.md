swagger: "2.0"
x-collection-name: AWS WorkDocs
x-complete: 1
info:
  title: AWS WorkDocs API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AbortDocumentVersionUpload:
    get:
      summary: Abort Document Version Upload
      description: Aborts the upload of the specified document version that was previously
        initiated by.
      operationId: abortDocumentVersionUpload
      x-api-path-slug: actionabortdocumentversionupload-get
      parameters:
      - in: query
        name: DocumentId
        description: The ID of the document
        type: string
      - in: query
        name: VersionId
        description: The ID of the version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Documents
  /?Action=InitiateDocumentVersionUpload:
    get:
      summary: Initiate Document Version Upload
      description: Creates a new document object and version object.
      operationId: initiateDocumentVersionUpload
      x-api-path-slug: actioninitiatedocumentversionupload-get
      parameters:
      - in: query
        name: ContentType
        description: The content type of the document
        type: string
      - in: query
        name: DocumentSizeInBytes
        description: The size of the document, in bytes
        type: string
      - in: query
        name: Id
        description: The ID of the document
        type: string
      - in: query
        name: Name
        description: The name of the document
        type: string
      - in: query
        name: ParentFolderId
        description: The ID of the parent folder
        type: string
      responses:
        200:
          description: OK
      tags:
      - Documents