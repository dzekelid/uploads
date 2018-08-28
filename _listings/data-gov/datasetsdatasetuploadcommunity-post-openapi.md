---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Add Datasets Dataset Upload Community
  description: Upload a new community resource
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /datasets/community_resources/{community}/upload/:
    post:
      summary: Add Datasets Community Resources Community Upload
      description: Update the file related to a given community resource
      operationId: postDatasetsCommunityResourcesCommunityUpload
      x-api-path-slug: datasetscommunity-resourcescommunityupload-post
      parameters:
      - in: path
        name: community
        description: The community resource unique identifier
      - in: query
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
      - Community
      - Upload
  /datasets/{dataset}/resources/{rid}/upload/:
    post:
      summary: Add Datasets Dataset Resources R Upload
      description: Upload a file related to a given resource on a given dataset
      operationId: postDatasetsDatasetResourcesRUpload
      x-api-path-slug: datasetsdatasetresourcesridupload-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: path
        name: rid
        description: The resource unique identifier
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Resources
      - R
      - Upload
  /datasets/{dataset}/upload/:
    post:
      summary: Add Datasets Dataset Upload
      description: Upload a new dataset resource
      operationId: postDatasetsDatasetUpload
      x-api-path-slug: datasetsdatasetupload-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Upload
  /datasets/{dataset}/upload/community/:
    post:
      summary: Add Datasets Dataset Upload Community
      description: Upload a new community resource
      operationId: postDatasetsDatasetUploadCommunity
      x-api-path-slug: datasetsdatasetuploadcommunity-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Upload
      - Community
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