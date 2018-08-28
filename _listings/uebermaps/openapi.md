swagger: "2.0"
x-collection-name: uebermaps
x-complete: 1
info:
  title: uebermaps
  description: enable-people-to-store-spots-on-public-and-private-maps
  termsOfService: https://uebermaps.com/terms/
  contact:
    name: uebermaps API Team
  version: "2.0"
host: uebermaps.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /maps/{id}/attachments:
    post:
      summary: Upload map attachment
      description: Upload map attachment. Wrap attachment parameters in [attachment]
      operationId: maps.id.attachments.post
      x-api-path-slug: mapsidattachments-post
      parameters:
      - in: path
        name: id
        description: Map id
      - in: body
        name: image
        description: Base64 encoded image
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Upload
      - Map
      - Attachment
  /spots/{id}/attachments:
    post:
      summary: Upload spot attachment
      description: Upload spot attachment. Wrap attachment parameters in [attachment]
      operationId: spots.id.attachments.post
      x-api-path-slug: spotsidattachments-post
      parameters:
      - in: path
        name: id
        description: Spot id
      - in: body
        name: image
        description: Base64 encoded image
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Upload
      - Spot
      - Attachment