swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox Notify Appendix API v1
  description: the-dropbox-notify--is-a-part-of-dropbox-core-ap-with-a-separate-endpoint-for-notification-call-
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api-notify.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /chunked_upload:
    put:
      summary: Chunked Upload
      description: /chunked_upload
      operationId: chunked-upload
      x-api-path-slug: chunked-upload-put
      parameters:
      - in: query
        name: offset
        description: The byte offset of this chunk, relative to the beginning of the
          full file
      - in: query
        name: upload_id
        description: The unique ID of the in-progress upload on the server
      responses:
        200:
          description: OK
      tags:
      - Chunked
      - Upload
  /commit_chunked_upload/{root}/{path}:
    post:
      summary: Completes an upload initiated by the chunked upload method.
      description: |-
        Completes an upload initiated by the `/chunked_upload` method. Saves a file uploaded via `/chunked_upload` to
        a user's Dropbox.

        `/commit_chunked_upload` is similar to `/files_put`. The main difference is that while `/files_put` takes the
        file contents in the request body, `/commit_chunked_upload` takes a parameter `upload_id`, which is obtained
        when the file contents are uploaded via `/chunked_upload`.
      operationId: completes-an-upload-initiated-by-the-chunked-upload-method-saves-a-file-uploaded-via-chunked-upload-
      x-api-path-slug: commit-chunked-uploadrootpath-post
      parameters:
      - in: query
        name: autorename
        description: This value, either `true` (default) or `false`, determines what
          happens when there is a conflict
      - in: query
        name: locale
        description: The metadata returned on successful upload will have its `size`
          field translated based on the given locale
      - in: query
        name: overwrite
        description: This value, either `true` (default) or `false`, determines whether
          an existing file will be overwritten bythis upload
      - in: query
        name: parent_rev
        description: If present, this parameter specifies the revision of the file
          youre editing
      - in: path
        name: path
        description: The full path to the file you want to write to
      - in: path
        name: root
        description: 'Root folder: `auto` - automatically determines the appropriate
          root folder using your apps permissionlevel (recommended); `sandbox` - the
          codename for app folder level; `dropbox` - full dropbox access'
      - in: query
        name: upload_id
        description: Used to identify the chunked upload session youd like to commit
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Commit
      - Chunked
      - Upload
      - Root
      - Path