---
name: AWS Device Farm
x-slug: aws-device-farm
description: AWS Device Farm is an app testing service that lets you test and interact
  with your Android, iOS, and web apps on many devices at once, or reproduce issues
  on a device in real time. View video, screenshots, logs, and performance data to
  pinpoint and fix issues before shipping your app.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AWSDeviceFarm.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Uploads
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/aws-device-farm/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Device Farm API Delete Upload
  x-api-slug: aws-device-farm-api
  description: Deletes an upload given the upload ARN.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AWSDeviceFarm.png
  humanURL: https://aws.amazon.com/device-farm/
  baseURL: ://///?Action=DeleteUpload
  tags: Uploads
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/aws-device-farm/actiondeleteupload-get-openapi.md
- name: AWS Device Farm API List Uploads
  x-api-slug: aws-device-farm-api
  description: Gets information about uploads, given an AWS Device Farm project ARN.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AWSDeviceFarm.png
  humanURL: https://aws.amazon.com/device-farm/
  baseURL: ://///?Action=ListUploads
  tags: Uploads
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/aws-device-farm/actionlistuploads-get-openapi.md
- name: AWS Device Farm API
  x-api-slug: aws-device-farm-api
  description: AWS Device Farm is an app testing service that lets you test and interact
    with your Android, iOS, and web apps on many devices at once, or reproduce issues
    on a device in real time. View video, screenshots, logs, and performance data
    to pinpoint and fix issues before shipping your app.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AWSDeviceFarm.png
  humanURL: https://aws.amazon.com/device-farm/
  baseURL: :///
  tags: Uploads
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/aws-device-farm/openapi.md
x-common:
- type: x-blog
  url: https://aws.amazon.com/blogs/mobile/tag/aws-device-farm/
- type: x-concepts
  url: https://docs.aws.amazon.com/devicefarm/latest/developerguide/concepts.html
- type: x-documentation
  url: https://docs.aws.amazon.com/devicefarm/latest/developerguide/api-ref.html
- type: x-documentation
  url: https://docs.aws.amazon.com/devicefarm/latest/developerguide/cli-ref.html
- type: x-limits
  url: https://docs.aws.amazon.com/devicefarm/latest/developerguide/limits.html
- type: x-logging
  url: https://docs.aws.amazon.com/devicefarm/latest/developerguide/cloudtrail.html
- type: x-plugins
  url: https://github.com/awslabs?q=aws-device-farm
- type: x-faq
  url: https://aws.amazon.com/device-farm/faq
- type: x-pricing
  url: https://aws.amazon.com/device-farm/pricing
- type: x-website
  url: https://aws.amazon.com/device-farm/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---