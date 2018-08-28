swagger: "2.0"
x-collection-name: Spreaker
x-complete: 1
info:
  title: Spreaker API
  version: v1
host: api.spreaker.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/{user_id}/images:
    post:
      summary: Upload An Image
      description: Upload An Image
      operationId: postUserUserImages
      x-api-path-slug: useruser-idimages-post
      parameters:
      - in: body
        name: Filedata
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Upload
      - Image