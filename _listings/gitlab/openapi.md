swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
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