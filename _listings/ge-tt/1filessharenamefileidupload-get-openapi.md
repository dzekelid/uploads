---
swagger: "2.0"
x-collection-name: Ge.tt
x-complete: 0
info:
  title: Ge.tt  REST API Files  Upload
  description: Get upload urls to the file. This returns a new PUT and POST url for
    you to upload the file to.nOBS You can also choose to use the put- or posturl
    that you were previously given to override the file.
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