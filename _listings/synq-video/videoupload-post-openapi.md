---
swagger: "2.0"
x-collection-name: SYNQ Video
x-complete: 0
info:
  title: SYNQ Video Return parameters needed for uploading a video file.
  description: |-
    Return parameters needed for uploading a video file to Amazon Simple Storage Service. See http://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-post-example.html as well as the language-specific code-examples.
    #### *Example request*
    ```shell
    curl -s https://api.synq.fm/v1/video/upload \
      -F api_key=${SYNQ_API_KEY} \
      -F video_id=2d81c30ce62f4dfdb501dbca96c7ae56
    ```

    #### *Example response*
    ```json
    {
      "action": "https://synqfm.s3.amazonaws.com/",
      "AWSAccessKeyId": "AKIAIP77Y7MMX3ITZMFA",
      "Content-Type": "video/mp4",
      "Policy": "eyJleHBpcmF0aW9uIiA6ICIyMDE2LTA0LTIyVDE5OjAyOjI2LjE3MloiLCAiY29uZGl0aW9ucyIgOiBbeyJidWNrZXQiIDogInN5bnFmbSJ9LCB7ImFjbCIgOiAicHVibGljLXJlYWQifSwgWyJzdGFydHMtd2l0aCIsICIka2V5IiwgInByb2plY3RzLzZlLzYzLzZlNjNiNzUyYTE4NTRkZGU4ODViNWNjNDcyZWRmNTY5L3VwbG9hZHMvdmlkZW9zLzJkLzgxLzJkODFjMzBjZTYyZjRkZmRiNTAxZGJjYTk2YzdhZTU2Lm1wNCJdLCBbInN0YXJ0cy13aXRoIiwgIiRDb250ZW50LVR5cGUiLCAidmlkZW8vbXA0Il0sIFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLCAwLCAxMDk5NTExNjI3Nzc2XV19",
      "Signature": "ysqDemlKXKr6hKzVFP0hCGgf/cs=",
      "acl": "public-read",
      "key": "projects/6e/63/6e63b752a1854dde885b5cc472edf569/uploads/videos/2d/81/2d81c30ce62f4dfdb501dbca96c7ae56.mp4"
    }
    ```

    To upload the file, you can then make a multipart POST request to the URL in `action`, and for all the other parameters returned, set them as form parameters.

    Given the parameters above, you would upload a file `test.mp4` using cURL like this:

    ```shell
    curl -s https://synqfm.s3.amazonaws.com/ \
      -F AWSAccessKeyId="AKIAIP77Y7MMX3ITZMFA" \
      -F Content-Type="video/mp4" \
      -F Policy="eyJleHBpcmF0aW9uIiA6ICIyMDE2LTA0LTIyVDE5OjAyOjI2LjE3MloiLCAiY29uZGl0aW9ucyIgOiBbeyJidWNrZXQiIDogInN5bnFmbSJ9LCB7ImFjbCIgOiAicHVibGljLXJlYWQifSwgWyJzdGFydHMtd2l0aCIsICIka2V5IiwgInByb2plY3RzLzZlLzYzLzZlNjNiNzUyYTE4NTRkZGU4ODViNWNjNDcyZWRmNTY5L3VwbG9hZHMvdmlkZW9zLzJkLzgxLzJkODFjMzBjZTYyZjRkZmRiNTAxZGJjYTk2YzdhZTU2Lm1wNCJdLCBbInN0YXJ0cy13aXRoIiwgIiRDb250ZW50LVR5cGUiLCAidmlkZW8vbXA0Il0sIFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLCAwLCAxMDk5NTExNjI3Nzc2XV19" \
      -F Signature="ysqDemlKXKr6hKzVFP0hCGgf/cs=" \
      -F acl="public-read" \
      -F key="projects/6e/63/6e63b752a1854dde885b5cc472edf569/uploads/videos/2d/81/2d81c30ce62f4dfdb501dbca96c7ae56.mp4" \
      -F file="@my_video_file.mp4"
    ```
  version: 1.9.1
host: api.synq.fm
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /video/uploader:
    post:
      summary: Return embeddable url to an uploader widget
      description: Returns an embeddable url, that contains an uploader widget that
        allows you to easily upload any mp4. Great way to simplify the uploading process
        for end users.
      operationId: uploader
      x-api-path-slug: videouploader-post
      parameters:
      - in: formData
        name: api_key
      - in: formData
        name: timeout
        description: How long the uploader widget works for
      - in: formData
        name: video_id
        description: The ID of the video you are going to upload into
      responses:
        200:
          description: OK
      tags:
      - Video
      - Uploader
  /video/upload:
    post:
      summary: Return parameters needed for uploading a video file.
      description: |-
        Return parameters needed for uploading a video file to Amazon Simple Storage Service. See http://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-post-example.html as well as the language-specific code-examples.
        #### *Example request*
        ```shell
        curl -s https://api.synq.fm/v1/video/upload \
          -F api_key=${SYNQ_API_KEY} \
          -F video_id=2d81c30ce62f4dfdb501dbca96c7ae56
        ```

        #### *Example response*
        ```json
        {
          "action": "https://synqfm.s3.amazonaws.com/",
          "AWSAccessKeyId": "AKIAIP77Y7MMX3ITZMFA",
          "Content-Type": "video/mp4",
          "Policy": "eyJleHBpcmF0aW9uIiA6ICIyMDE2LTA0LTIyVDE5OjAyOjI2LjE3MloiLCAiY29uZGl0aW9ucyIgOiBbeyJidWNrZXQiIDogInN5bnFmbSJ9LCB7ImFjbCIgOiAicHVibGljLXJlYWQifSwgWyJzdGFydHMtd2l0aCIsICIka2V5IiwgInByb2plY3RzLzZlLzYzLzZlNjNiNzUyYTE4NTRkZGU4ODViNWNjNDcyZWRmNTY5L3VwbG9hZHMvdmlkZW9zLzJkLzgxLzJkODFjMzBjZTYyZjRkZmRiNTAxZGJjYTk2YzdhZTU2Lm1wNCJdLCBbInN0YXJ0cy13aXRoIiwgIiRDb250ZW50LVR5cGUiLCAidmlkZW8vbXA0Il0sIFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLCAwLCAxMDk5NTExNjI3Nzc2XV19",
          "Signature": "ysqDemlKXKr6hKzVFP0hCGgf/cs=",
          "acl": "public-read",
          "key": "projects/6e/63/6e63b752a1854dde885b5cc472edf569/uploads/videos/2d/81/2d81c30ce62f4dfdb501dbca96c7ae56.mp4"
        }
        ```

        To upload the file, you can then make a multipart POST request to the URL in `action`, and for all the other parameters returned, set them as form parameters.

        Given the parameters above, you would upload a file `test.mp4` using cURL like this:

        ```shell
        curl -s https://synqfm.s3.amazonaws.com/ \
          -F AWSAccessKeyId="AKIAIP77Y7MMX3ITZMFA" \
          -F Content-Type="video/mp4" \
          -F Policy="eyJleHBpcmF0aW9uIiA6ICIyMDE2LTA0LTIyVDE5OjAyOjI2LjE3MloiLCAiY29uZGl0aW9ucyIgOiBbeyJidWNrZXQiIDogInN5bnFmbSJ9LCB7ImFjbCIgOiAicHVibGljLXJlYWQifSwgWyJzdGFydHMtd2l0aCIsICIka2V5IiwgInByb2plY3RzLzZlLzYzLzZlNjNiNzUyYTE4NTRkZGU4ODViNWNjNDcyZWRmNTY5L3VwbG9hZHMvdmlkZW9zLzJkLzgxLzJkODFjMzBjZTYyZjRkZmRiNTAxZGJjYTk2YzdhZTU2Lm1wNCJdLCBbInN0YXJ0cy13aXRoIiwgIiRDb250ZW50LVR5cGUiLCAidmlkZW8vbXA0Il0sIFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLCAwLCAxMDk5NTExNjI3Nzc2XV19" \
          -F Signature="ysqDemlKXKr6hKzVFP0hCGgf/cs=" \
          -F acl="public-read" \
          -F key="projects/6e/63/6e63b752a1854dde885b5cc472edf569/uploads/videos/2d/81/2d81c30ce62f4dfdb501dbca96c7ae56.mp4" \
          -F file="@my_video_file.mp4"
        ```
      operationId: upload
      x-api-path-slug: videoupload-post
      parameters:
      - in: formData
        name: api_key
      - in: formData
        name: video_id
        description: The ID of the video you are going to upload into
      responses:
        200:
          description: OK
      tags:
      - Video
      - Upload
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