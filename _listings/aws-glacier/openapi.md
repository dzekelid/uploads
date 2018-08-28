---
swagger: "2.0"
x-collection-name: AWS Glacier
x-complete: 1
info:
  title: AWS Glacier API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{AccountId}/vaults/{VaultName}/multipart-uploads/{uploadID}:
    delete:
      summary: Abort  Multipart  Upload
      description: "DescriptionThis multipart upload operation aborts a multipart
        upload identified by the upload\n\t\t\tID"
      operationId: abort Multipart Upload (DELETE uploadID)
      x-api-path-slug: accountidvaultsvaultnamemultipartuploadsuploadid-delete
      responses:
        200:
          description: OK
      tags:
      - Multipart Uploads
    post:
      summary: Complete  Multipart  Upload
      description: "DescriptionYou call this multipart upload operation to inform
        Amazon Glacier that all the archive parts have\n\t\t\tbeen uploaded and Amazon
        Glacier can now assemble the archive from the uploaded parts"
      operationId: complete Multipart Upload (POST uploadID)
      x-api-path-slug: accountidvaultsvaultnamemultipartuploadsuploadid-post
      parameters:
      - type: string
      responses:
        200:
          description: OK
      tags:
      - Multipart Uploads
  /{AccountId}/vaults/{VaultName}/multipart-uploads:
    get:
      summary: List  Multipart  Uploads
      description: DescriptionThis multipart upload operation lists in-progress multipart
        uploads for the specified vault
      operationId: list Multipart Uploads (GET multipart-uploads)
      x-api-path-slug: accountidvaultsvaultnamemultipartuploads-get
      parameters:
      - in: query
        name: ArchiveDescription
        description: The description of the archive that was specified in the Initiate
          Multipart Uploadrequest
        type: string
      - in: query
        name: CreationDate
        description: The UTC time that the multipart upload was initiated
        type: string
      - in: query
        name: Marker
        description: An opaque string that represents where to continue pagination
          of the results
        type: string
      - in: query
        name: MultipartUploadId
        description: The ID of the multipart upload
        type: string
      - in: query
        name: PartSizeInBytes
        description: The part size specified in the Initiate Multipart Upload (POSTmultipart-uploads)
          request
        type: string
      - in: query
        name: UploadsList
        description: A list of metadata about multipart upload objects
        type: string
      - in: query
        name: VaultARN
        description: The Amazon Resource Name (ARN) of the vault that contains the
          archive
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multipart Uploads
---