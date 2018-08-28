swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/drive/items/{parent-id}:/{filename}:/content:
    put:
      summary: Upload Or Replace The Contents Of A Drive Item
      description: Upload or replace the contents of a driveItem The simple upload
        API allows you to provide the contents of a new file or update the contents
        of an existing file in a single API call. This method only supports files
        up to 4MB in size.
      operationId: UploadOrReplaceTheContentsOfADriveItem
      x-api-path-slug: medriveitemsparentidfilenamecontent-put
      parameters:
      - in: path
        name: filename
        type: string
      - in: path
        name: parent-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Or
      - ReplaceContents
      - OfDrive
      - Item
  /me/drive/root:/{parent-path}/{filename}:/content:
    put:
      summary: Upload Or Replace The Contents Of A Drive Item
      description: Upload or replace the contents of a driveItem The simple upload
        API allows you to provide the contents of a new file or update the contents
        of an existing file in a single API call. This method only supports files
        up to 4MB in size.
      operationId: UploadOrReplaceTheContentsOfADriveItem
      x-api-path-slug: medriverootparentpathfilenamecontent-put
      parameters:
      - in: path
        name: filename
        type: string
      - in: path
        name: parent-path
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Or
      - ReplaceContents
      - OfDrive
      - Item
  /me/drive/items/{parent-id}/children/{filename}/content:
    put:
      summary: Upload Or Replace The Contents Of A Drive Item
      description: Upload or replace the contents of a driveItem The simple upload
        API allows you to provide the contents of a new file or update the contents
        of an existing file in a single API call. This method only supports files
        up to 4MB in size.
      operationId: UploadOrReplaceTheContentsOfADriveItem
      x-api-path-slug: medriveitemsparentidchildrenfilenamecontent-put
      parameters:
      - in: path
        name: filename
        type: string
      - in: path
        name: parent-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Or
      - ReplaceContents
      - OfDrive
      - Item
  /groups/{id}/drive/items/{parent-id}/children/{filename}/content:
    put:
      summary: Upload Or Replace The Contents Of A Drive Item
      description: Upload or replace the contents of a driveItem The simple upload
        API allows you to provide the contents of a new file or update the contents
        of an existing file in a single API call. This method only supports files
        up to 4MB in size.
      operationId: UploadOrReplaceTheContentsOfADriveItem
      x-api-path-slug: groupsiddriveitemsparentidchildrenfilenamecontent-put
      parameters:
      - in: path
        name: filename
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: parent-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Or
      - ReplaceContents
      - OfDrive
      - Item