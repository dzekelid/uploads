---
swagger: "2.0"
x-collection-name: AWS EC2 Container Registry Service
x-complete: 0
info:
  title: AWS EC2 Container Registry API Complete Layer Upload
  version: 1.0.0
  description: Inform Amazon ECR that the image layer upload for a specified registry,
    repository name, and upload ID, has completed.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UploadLayerPart:
    get:
      summary: Upload Layer Part
      description: Uploads an image layer part to Amazon ECR.
      operationId: uploadLayerPart
      x-api-path-slug: actionuploadlayerpart-get
      responses:
        200:
          description: OK
      tags:
      - Layer Parts
  /?Action=CompleteLayerUpload:
    get:
      summary: Complete Layer Upload
      description: Inform Amazon ECR that the image layer upload for a specified registry,
        repository name, and upload ID, has completed.
      operationId: completeLayerUpload
      x-api-path-slug: actioncompletelayerupload-get
      responses:
        200:
          description: OK
      tags:
      - Layer Upload
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