swagger: "2.0"
x-collection-name: SAP
x-complete: 1
info:
  title: SAP Translation Hub
  description: to-provide-users-of-software-in-a-global-market-with-texts-in-their-own-language-translations-are-required--sap-translation-hub-enables-you-to-draw-on-saps-translation-experience-across-multiple-products-and-languages-to-propose-translations-for-short-texts-
  contact:
    name: SAP Translation Hub team
    email: translationhub@sap.com
  version: 1.0.0
host: sandbox.api.sap.com
basePath: /translationhub/api/v1
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