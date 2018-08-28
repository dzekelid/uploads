---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Store avatar
  description: Creates an avatar for a given entity, for the given entity ID and type
    of entity. For example, you can create an avatar for an issue type, given the
    issue type Id. Uploading an avatar is supported for different types of entities
    across the Jira products. However, it is supported for the "project" and "issuetype"
    entity types for all Jira products. The uploaded image will be cropped according
    to the crop parameters listed below. If no crop parameters are specified, the
    image will be cropped to a square. The square will originate at the top left of
    the image and the length of each side will be set to the smaller of the height
    or width of the image.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/universal_avatar/type/{type}/owner/{entityId}:
    post:
      summary: Store avatar
      description: Creates an avatar for a given entity, for the given entity ID and
        type of entity. For example, you can create an avatar for an issue type, given
        the issue type Id. Uploading an avatar is supported for different types of
        entities across the Jira products. However, it is supported for the "project"
        and "issuetype" entity types for all Jira products. The uploaded image will
        be cropped according to the crop parameters listed below. If no crop parameters
        are specified, the image will be cropped to a square. The square will originate
        at the top left of the image and the length of each side will be set to the
        smaller of the height or width of the image.
      operationId: com.atlassian.jira.rest.v2.issue.UniversalAvatarResource.storeAvatar_post
      x-api-path-slug: api2universal-avatartypetypeownerentityid-post
      parameters:
      - in: path
        name: entityId
        description: The Id of the entity that you want to update the avatar of
      - in: query
        name: size
        description: (optional) The length of each side of the crop region
      - in: path
        name: type
        description: The type of the entity that you want to update the avatar of
      - in: query
        name: x
        description: (optional) The X coordinate of the top-left corner of the crop
          region
      - in: query
        name: "y"
        description: (optional) The Y coordinate of the top-left corner of the crop
          region
      responses:
        200:
          description: OK
      tags:
      - Store
      - Avatar
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