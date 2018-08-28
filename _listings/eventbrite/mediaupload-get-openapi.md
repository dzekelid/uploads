---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Get Media Upload
  description: See Media Uploads.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /media/upload/:
    get:
      summary: Get Media Upload
      description: See Media Uploads.
      operationId: getMediaUpload
      x-api-path-slug: mediaupload-get
      parameters:
      - in: query
        name: type
        description: 'The type of image to upload (Valid choices are: image-event-logo,
          image-event-logo-preserve-quality, image-event-view-from-seat, image-organizer-logo,
          image-user-photo, or image-structured-content)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Media
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