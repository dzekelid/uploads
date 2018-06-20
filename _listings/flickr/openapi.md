---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 1
info:
  title: Flickr
  description: explore-upload-and-organize-photos-on-flickr
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.people.getUploadStatus:
    get:
      summary: People Get Upload Status
      description: Returns information for the calling user related to photo uploads.
      operationId: getRestMethodFlickr.people.getuploadstatus
      x-api-path-slug: restmethodflickr-people-getuploadstatus-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - People
      - GetUploadStatus
---