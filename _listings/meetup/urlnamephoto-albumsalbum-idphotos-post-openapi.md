---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Album Photo Upload
  description: Support for uploading new Album photos
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2/group_photo:
    post:
      summary: Group Photo Upload
      description: Uploads a new Meetup Group photo. To change other Group settings
        use the [Group Edit](/meetup_api/docs/:urlname/#edit) endpoint
      operationId: groups
      x-api-path-slug: 2group-photo-post
      parameters:
      - in: query
        name: await
        description: If true, this ensures a response will not be returned until the
          upload is accessible
        type: string
      - in: query
        name: group_id
        description: Group ID for the target group
        type: string
      - in: query
        name: group_urlname
        description: Group urlname
        type: string
      - in: query
        name: main
        description: Set to true to have this photo become the groups main photo
        type: string
      - in: query
        name: photo
        description: The photo, encoded as multipart/form-data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
  /2/member_photo:
    post:
      summary: Member Photo Upload
      description: Uploads a photo to be associated with a Member
      operationId: members
      x-api-path-slug: 2member-photo-post
      parameters:
      - in: query
        name: await
        description: If true, this ensures a response will not be returned until the
          upload is accessible
        type: string
      - in: query
        name: main
        description: Set to true to have this photo become the members main profile
          photo
        type: string
      - in: query
        name: photo
        description: The photo, encoded as multipart/form-data
        type: string
      - in: query
        name: sync_matching_photo
        description: When set to true and main is set to true, this will replace all
          group profile photos matching the current photo with the provided replacement
        type: string
      - in: query
        name: sync_photo
        description: When set to true, this parameter will sync all of the group profile
          photos for the member with the provided photo_id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
      - Member
  /2/photo:
    post:
      summary: Event Photo Upload
      description: Uploads a photo for a given event
      operationId: photos
      x-api-path-slug: 2photo-post
      parameters:
      - in: query
        name: await
        description: If true, this ensures a response will not be returned until the
          upload is accessible
        type: string
      - in: query
        name: caption
        description: Caption for the photo
        type: string
      - in: query
        name: event_id
        description: Identifier of an event
        type: string
      - in: query
        name: photo
        description: The photo, encoded as multipart/form-data
        type: string
      - in: query
        name: photo_album_id
        description: Identifier of an existing photo album, which may be an event
          or group album
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/events/:event_id/photos:
    post:
      summary: Event Photo Upload
      description: Support for uploading new Event photos
      operationId: photos
      x-api-path-slug: urlnameeventsevent-idphotos-post
      parameters:
      - in: query
        name: await
        description: Optional boolean parameter that will defer a requests a response
          until confirmation that photo is immediately displayable is received
        type: string
      - in: query
        name: caption
        description: Caption for display
        type: string
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      - in: query
        name: photo
        description: Photo upload data, encoded as multipart/form-data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/photo_albums/:album_id/photos:
    post:
      summary: Album Photo Upload
      description: Support for uploading new Album photos
      operationId: photos
      x-api-path-slug: urlnamephoto-albumsalbum-idphotos-post
      parameters:
      - in: query
        name: await
        description: Optional boolean parameter that will defer a requests a response
          until confirmation that photo is immediately displayable is received
        type: string
      - in: query
        name: caption
        description: Caption for display
        type: string
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      - in: query
        name: photo
        description: Photo upload data, encoded as multipart/form-data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
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