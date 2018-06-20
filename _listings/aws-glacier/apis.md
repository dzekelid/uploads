---
name: AWS Glacier
x-slug: aws-glacier
description: Amazon Glacier is a secure, durable, and extremely low-cost cloud storage
  service for data archiving and long-term backup. Customers can reliably store large
  or small amounts of data for as little as $0.004 per gigabyte per month, a significant
  savings compared to on-premises solutions. To keep costs low yet suitable for varying
  retrieval needs, Amazon Glacier provides three options for access to archives, from
  a few minutes to several hours.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Uploads
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/aws-glacier/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon Glacier API Abort  Multipart  Upload
  x-api-slug: amazon-glacier-api
  description: "DescriptionThis multipart upload operation aborts a multipart upload
    identified by the upload\n\t\t\tID"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: ://///{AccountId}/vaults/{VaultName}/multipart-uploads/{uploadID}
  tags: Multipart Uploads
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/aws-glacier/accountidvaultsvaultnamemultipartuploadsuploadid-delete-openapi.md
- name: Amazon Glacier API Complete  Multipart  Upload
  x-api-slug: amazon-glacier-api
  description: "DescriptionYou call this multipart upload operation to inform Amazon
    Glacier that all the archive parts have\n\t\t\tbeen uploaded and Amazon Glacier
    can now assemble the archive from the uploaded parts"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: ://///{AccountId}/vaults/{VaultName}/multipart-uploads/{uploadID}
  tags: Multipart Uploads
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/aws-glacier/accountidvaultsvaultnamemultipartuploadsuploadid-post-openapi.md
- name: Amazon Glacier API List  Multipart  Uploads
  x-api-slug: amazon-glacier-api
  description: DescriptionThis multipart upload operation lists in-progress multipart
    uploads for the specified vault
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: ://///{AccountId}/vaults/{VaultName}/multipart-uploads
  tags: Multipart Uploads
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/aws-glacier/accountidvaultsvaultnamemultipartuploads-get-openapi.md
- name: Amazon Glacier API
  x-api-slug: amazon-glacier-api
  description: Amazon Glacier is a secure, durable, and extremely low-cost cloud storage
    service for data archiving and long-term backup. Customers can reliably store
    large or small amounts of data for as little as $0.004 per gigabyte per month,
    a significant savings compared to on-premises solutions. To keep costs low yet
    suitable for varying retrieval needs, Amazon Glacier provides three options for
    access to archives, from a few minutes to several hours.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: :///
  tags: Uploads
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/aws-glacier/openapi.md
x-common:
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/Amazon-Glacier/
- type: x-documentation
  url: http://docs.aws.amazon.com/amazonglacier/latest/dev/amazon-glacier-api.html
- type: x-faq
  url: https://aws.amazon.com/glacier/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=140
- type: x-getting-started
  url: https://aws.amazon.com/glacier/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/glacier/pricing/
- type: x-website
  url: https://aws.amazon.com/glacier/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---