swagger: "2.0"
x-collection-name: Ge.tt
x-complete: 1
info:
  title: Ge.tt  REST API
  description: the-ge-tt-api-allows-you-to-use-ge-tt-in-your-own-applications--we-believe-that-our-users-should-be-able-to-access-their-files-and-share-their-content-in-their-platform-of-choice--by-using-the-api-developers-are-able-to-easily-put-their-own-content-or-the-content-of-their-users-online--at-the-same-time-they-are-able-to-use-ge-tts-unique-realtime-file-sharing-technology-where-files-are-available-before-they-are-even-uploaded-
  termsOfService: http://ge.tt/terms
  version: "1"
host: open.ge.tt
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /1/files/{sharename}/{fileid}/upload:
    get:
      summary: Files  Upload
      description: Get upload urls to the file. This returns a new PUT and POST url
        for you to upload the file to.nOBS You can also choose to use the put- or
        posturl that you were previously given to override the file.
      operationId: get1FilesSharenameFileUpload
      x-api-path-slug: 1filessharenamefileidupload-get
      parameters:
      - in: query
        name: accesstoken
      - in: path
        name: fileid
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Files
      - Sharename
      - Fileid
      - Upload