swagger: "2.0"
x-collection-name: Framesocket
x-complete: 1
info:
  title: Framesocket
  description: framesocket-is-the-best-way-for-developers-and-content-owners-to-tackle-video-projects-of-any-size-
  version: 1.0.0
host: www.framesocket.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /media/upload.php:
    post:
      summary: Upload Media
      description: Upload Media
      operationId: postMediaUpload.php
      x-api-path-slug: mediaupload-php-post
      parameters:
      - in: query
        name: callback
      - in: query
        name: customid
        description: Text String - Max Length 32 Characters
      - in: query
        name: description
        description: Text String - Limit 1000 Characters
      - in: query
        name: key
        description: Your account username
      - in: query
        name: keywords
        description: Text String - Comma separated by keyword or phrase
      - in: query
        name: media
        description: Must be properly formatted POST data - either an image or a video
      - in: query
        name: secret
        description: Your account API secret
      - in: query
        name: sig
        description: This is an md5 hash of your gatekeeper concatenated with your
          request action
      - in: query
        name: title
        description: Text String - Limit 100 Characters
      responses:
        200:
          description: OK
      tags:
      - Media
      - Upload