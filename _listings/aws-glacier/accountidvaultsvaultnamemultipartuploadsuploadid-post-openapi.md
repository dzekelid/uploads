---
swagger: "2.0"
x-collection-name: AWS Glacier
x-complete: 0
info:
  title: Amazon Glacier API Complete  Multipart  Upload
  version: 1.0.0
  description: "DescriptionYou call this multipart upload operation to inform Amazon
    Glacier that all the archive parts have\n\t\t\tbeen uploaded and Amazon Glacier
    can now assemble the archive from the uploaded parts"
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