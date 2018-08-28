swagger: "2.0"
x-collection-name: EhrScape
x-complete: 1
info:
  title: EhrScape Terminology APIs
  description: validates-and-resolves-terminology-codes
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: rest.ehrscape.com
basePath: /terminology-adapter/rest
paths:
  /guide/upload:
    post:
      summary: Uploads new guide definition.
      description: Uploads new guide definition..
      operationId: uploadGuide
      x-api-path-slug: guideupload-post
      parameters:
      - in: form
        name: guide
        description: Base64 encoded guide definition
      responses:
        200:
          description: OK
      tags:
      - Guide
      - Upload