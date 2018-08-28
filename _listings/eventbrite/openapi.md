swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 1
info:
  title: Eventbrite
  description: create-manage--promote-events--add-eventmanagement-features-to-your-site--show-the-world-what-exciting-things-are-happening-around-them-
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