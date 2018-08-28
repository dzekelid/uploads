---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr People Get Upload Status
  description: Returns information for the calling user related to photo uploads.
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