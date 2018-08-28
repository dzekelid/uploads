---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 0
info:
  title: Dropbox Content Completes an upload initiated by the chunked upload method.
  description: |-
    Completes an upload initiated by the `/chunked_upload` method. Saves a file uploaded via `/chunked_upload` to
    a user's Dropbox.

    `/commit_chunked_upload` is similar to `/files_put`. The main difference is that while `/files_put` takes the
    file contents in the request body, `/commit_chunked_upload` takes a parameter `upload_id`, which is obtained
    when the file contents are uploaded via `/chunked_upload`.
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api-content.dropbox.com
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
      summary: Uploads large files to Dropbox in multiple chunks.
      description: |-
        Uploads large files to Dropbox in multiple chunks. Also has the ability to resume if the upload is interrupted.
        This allows for uploads larger than the `/files_put` maximum of 150 MB.

        Typical usage:
          1. Send a PUT request to `/chunked_upload` with the first chunk of the file without setting `upload_id`, and
          receive an `upload_id` in return.
          2. Repeatedly `PUT` subsequent chunks using the `upload_id` to identify the upload in progress and an `offset`
          representing the number of bytes transferred so far.
          3. After each chunk has been uploaded, the server returns a new offset representing the total amount transferred.
          4. After the last chunk, `POST` to `/commit_chunked_upload` to complete the upload.

        Chunks can be any size up to 150 MB. A typical chunk is 4 MB. Using large chunks will mean fewer calls
        to `/chunked_upload` and faster overall throughput. However, whenever a transfer is interrupted, you will
        have to resume at the beginning of the last chunk, so it is often safer to use smaller chunks.

        If the offset you submit does not match the expected offset on the server, the server will ignore the request
        and respond with a 400 error that includes the current offset. To resume upload, seek to the correct offset
        (in bytes) within the file and then resume uploading from that point.

        A chunked upload can take a maximum of 48 hours before expiring.
      operationId: uploads-large-files-to-dropbox-in-multiple-chunks-also-has-the-ability-to-resume-if-the-upload-is-in
      x-api-path-slug: chunked-upload-put
      parameters:
      - in: body
        name: file_content
        description: A chunk of data from the file being uploaded
        schema:
          $ref: '#/definitions/holder'
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
      - Storage
      - Documents
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