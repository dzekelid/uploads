swagger: "2.0"
x-collection-name: AWS EC2 Container Registry Service
x-complete: 1
info:
  title: AWS EC2 Container Registry API
  version: 1.0.0
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
  /?Action=InitiateLayerUpload:
    get:
      summary: Initiate Layer Upload
      description: Notify Amazon ECR that you intend to upload an image layer.
      operationId: initiateLayerUpload
      x-api-path-slug: actioninitiatelayerupload-get
      responses:
        200:
          description: OK
      tags:
      - Layer Upload