swagger: "2.0"
x-collection-name: Strava
x-complete: 1
info:
  title: Strava API v3
  description: strava-api
  version: 1.0.0
host: www.strava.com
basePath: /api/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /uploads:
    post:
      summary: Upload Activity
      description: Uploads a new data file to create an activity from.
      operationId: createUpload
      x-api-path-slug: uploads-post
      parameters:
      - in: formData
        name: commute
        description: Whether the resulting activity should be tagged as a commute
      - in: formData
        name: data_type
        description: The format of the uploaded file
      - in: formData
        name: description
        description: The desired description of the resulting activity
      - in: formData
        name: external_id
        description: The desired external identifier of the resulting activity
      - in: formData
        name: file
        description: The uploaded file
      - in: formData
        name: name
        description: The desired name of the resulting activity
      - in: formData
        name: private
        description: Whether the resulting activity should be private
      - in: formData
        name: trainer
        description: Whether the resulting activity should be marked as having been
          performed on a trainer
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Upload
      - Activity
  /uploads/{uploadId}:
    get:
      summary: Get Upload
      description: Returns an upload for a given identifier.
      operationId: getUploadById
      x-api-path-slug: uploadsuploadid-get
      parameters:
      - in: path
        name: uploadId
        description: The identifier of the upload
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Upload