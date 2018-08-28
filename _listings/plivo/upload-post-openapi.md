---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Post Upload
  description: Allows an application to upload the photo file.nnNote that this endpoint
    is at the upload.500px.com domain, not the api.500px.com domain.
  version: 1.0.0
host: /account
basePath: https://codenvy.com/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /photos/upload:
    post:
      summary: Post Photos Upload
      description: This is a new photo upload endpoint. It is currently in beta.nCreate
        a new photo on behalf of the user and upload a file.nfile parameter is passed
        in multipart/form-data, other parameters are passed as query parametrs or
        multipart/form-data.
      operationId: this-is-a-new-photo-upload-endpoint-it-is-currently-in-betacreate-a-new-photo-on-behalf-of-the-user-
      x-api-path-slug: photosupload-post
      parameters:
      - in: query
        name: aperture
        description: Aperture value
      - in: query
        name: camera
        description: Make and model of the camera
      - in: query
        name: category
        description: A numerical ID for the Category of the photo
      - in: query
        name: description
        description: Description for the photo
      - in: query
        name: file (required)  - Photo filename in JPG/JPEG, passed along with multipart/form-data.
      - in: query
        name: focal_length
        description: Focal length in millimetres, a string representing an integer
          value
      - in: query
        name: iso
        description: ISO value
      - in: query
        name: latitude
        description: Latitude, in decimal format
      - in: query
        name: lens
        description: Lens used to make this photo
      - in: query
        name: longitude
        description: Longitude, in decimal format
      - in: query
        name: name
        description: Title of the photo
      - in: query
        name: privacy
        description: Whether to hide the photo from the user profile on the website
      - in: query
        name: shutter_speed
        description: Shutter speed in seconds, represented by string containing a
          rational expression if the value is 1sec
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Upload
  /upload:
    post:
      summary: Post Upload
      description: Allows an application to upload the photo file.nnNote that this
        endpoint is at the upload.500px.com domain, not the api.500px.com domain.
      operationId: allows-an-application-to-upload-the-photo-filenote-that-this-endpoint-is-at-the-upload500pxcom-domai
      x-api-path-slug: upload-post
      parameters:
      - in: query
        name: file
        description: The multipart HTTP upload
      - in: query
        name: photo_id
        description: The ID of the photo the file is being uploaded for
      responses:
        200:
          description: OK
      tags:
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