---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Post Projects Uploads
  version: 1.0.0
  description: Post projects uploads.
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/uploads:
    post:
      summary: Post Projects Uploads
      description: Post projects uploads.
      operationId: postV3ProjectsIdUploads
      x-api-path-slug: v3projectsiduploads-post
      parameters:
      - in: formData
        name: file
        description: The file to be uploaded
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Uploads
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