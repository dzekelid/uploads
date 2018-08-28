---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Manufacturing Network Partner APIs Uploads a file
  description: Uploads a file to a collaboration room.
  version: 1.0.0
host: hostname
basePath: /dim/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /documents/collaborationRooms/{collaborationRoomId}/upload:
    post:
      summary: Uploads a file
      description: Uploads a file to a collaboration room.
      operationId: uploads-a-file-to-a-collaboration-room
      x-api-path-slug: documentscollaborationroomscollaborationroomidupload-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: formData
        name: fileUpload
        description: A file to be uploaded
      - in: formData
        name: originFileDisplay
        description: Indicates if a file is visible to all participants in the collaboration
          room (public) or to the uploader only (private)
      responses:
        200:
          description: Successful response
      tags:
      - Uploads
      - File
  /documents/organizations/{organizationId}/TEMP/upload:
    post:
      summary: Uploads a file to the temp folder
      description: Uploads a file to the temp folder for an organization.
      operationId: uploads-a-file-to-the-temp-folder-for-an-organization
      x-api-path-slug: documentsorganizationsorganizationidtempupload-post
      parameters:
      - in: formData
        name: fileUpload
        description: A file to be uploaded
      - in: path
        name: organizationId
        description: The ID of an organization
      responses:
        200:
          description: Successful response
      tags:
      - Uploads
      - File
      - To
      - Temp
      - Folder
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