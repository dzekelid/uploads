---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Upload User Profile Image
  description: "Returns the extension profile image.\nApp Permission\nEditExtensions\nUser
    Permission\nEditUserInfo\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call
    this API endpoint, application needs to have [EditExtensions] permission"
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/glip/files:
    post:
      summary: Upload File
      description: |-
        Posts a file.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Heavy
      operationId: createGlipFile
      x-api-path-slug: restapiv1-0glipfiles-post
      parameters:
      - in: formData
        name: body
        description: The file to upload
      - in: query
        name: groupId
        description: Internal identifier of a group to which the post with attachement
          will be added to
      - in: formData
        name: name
        description: Name of a file attached
      responses:
        200:
          description: OK
      tags:
      - Upload
      - File
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/profile-image:
    post:
      summary: Upload User Profile Image
      description: "Returns the extension profile image.\nApp Permission\nEditExtensions\nUser
        Permission\nEditUserInfo\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n
        \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [EditExtensions]
        permission"
      operationId: uploadImageByPostForm
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidprofileimage-post
      parameters:
      - in: path
        name: accountId
      - in: path
        name: extensionId
      - in: formData
        name: image
      responses:
        200:
          description: OK
      tags:
      - Upload
      - User
      - Profile
      - Image
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