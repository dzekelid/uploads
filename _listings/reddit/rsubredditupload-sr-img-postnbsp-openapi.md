---
swagger: "2.0"
x-collection-name: Reddit
x-complete: 0
info:
  title: Reddit Add Subreddit Upload Sr Img
  description: |-
    Add or replace a subreddit image, custom header logo, custom mobile
    icon, or custom mobile banner.
  version: 1.0.0
host: www.reddit.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/subreddit/emoji_asset_upload_s3.json:
    post&nbsp;:
      summary: Add Subreddit Emoji Asset Upload S3.json
      description: |-
        Acquire and return an upload lease to s3 temp bucket. The return value
        of this function is a json object containing credentials for uploading
        assets to S3 bucket, S3 url for upload request and the key to use for
        uploading. Using this lease the client will upload the emoji image to
        S3 temp bucket (included as part of the S3 URL).
      operationId: post&nbsp;V1SubredditEmojiAssetUploadS3.json
      x-api-path-slug: v1subredditemoji-asset-upload-s3-json-postnbsp
      parameters:
      - in: query
        name: filepath
        description: name and extension of the image file e
        type: string
      - in: query
        name: mimetype
        description: mime type of the image e
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subreddit
      - Emoji
      - Asset
      - Upload
      - S3.json
  '{/r/subreddit}/upload_sr_img':
    post&nbsp;:
      summary: Add Subreddit Upload Sr Img
      description: |-
        Add or replace a subreddit image, custom header logo, custom mobile
        icon, or custom mobile banner.
      operationId: post&nbsp;RSubredditUploadSrImg
      x-api-path-slug: rsubredditupload-sr-img-postnbsp
      parameters:
      - in: query
        name: file
        description: file upload with maximum size of 500 KiB
        type: string
      - in: query
        name: formid
        description: (optional) can be ignored
        type: string
      - in: query
        name: header
        description: an integer between 0 and 1
        type: string
      - in: query
        name: img_type
        description: 'one of png or jpg (default: png)'
        type: string
      - in: query
        name: name
        description: a valid subreddit image name
        type: string
      - in: query
        name: uh / X-Modhash header
        description: a modhash
        type: string
      - in: query
        name: upload_type
        description: one of (img, header, icon, banner)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subreddit
      - Upload
      - Sr
      - Img
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