---
name: AWS Glacier
description: Amazon Glacier is a secure, durable, and extremely low-cost cloud storage
  service for data archiving and long-term backup. Customers can reliably store large
  or small amounts of data for as little as $0.004 per gigabyte per month, a significant
  savings compared to on-premises solutions. To keep costs low yet suitable for varying
  retrieval needs, Amazon Glacier provides three options for access to archives, from
  a few minutes to several hours.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Storage
- Stack Network
- Amazon Web Services
created: "2018-03-23"
modified: "2018-03-23"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/aws-glacier/apis.yaml
specificationVersion: "0.14"
apis:
- name: Amazon Glacier API
  description: Amazon Glacier is a secure, durable, and extremely low-cost cloud storage
    service for data archiving and long-term backup
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: ""
  baseURL: :///
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/aws-glacier/accountid-vaults-vaultname-jobs-get.md
- name: Amazon Glacier API Get  Job  Output
  description: "DescriptionThis operation downloads the output of the job you initiated
    using Initiate Job (POST jobs). Depending\n\t\t\ton the job type you specified
    when you initiated the job, the output will be either the\n\t\t\tcontent of an
    archive or a vault inventory. You can download all the job output or download
    a portion of the output by specifying\n\t\t\ta byte range. For both archive and
    inventory retrieval jobs, you should verify the downloaded \n\t\t\tsize against
    the size returned in the headers from the \n\t\t\tGet Job Output response.For
    archive retrieval jobs, you should also verify that the size is what you expected.
    If\n\t\t\tyou download a portion of the output, the expected size is based on
    the range of bytes\n\t\t\tyou specified. For example, if you specify a range of
    bytes=0-1048575, you should\n\t\t\tverify your download size is 1,048,576 bytes.
    If you download an entire archive, the\n\t\t\texpected size is the size of the
    archive when you uploaded it to Amazon Glacier.\n\t\t\tThe expected size is also
    returned in the headers from the \n\t\t\tGet Job Output response.In the case of
    an archive retrieval job, depending on the byte range you\n\t\t\tspecify, Amazon
    Glacier returns the checksum for the portion of the data. To ensure the portion
    you downloaded \n\t\t\tis the correct data, compute the checksum on the client,
    verify that the values match, \n\t\t\tand verify that the size is what you expected.A
    job ID does not expire for at least 24 hours after Amazon Glacier completes the
    job. That\n\t\t\tis, you can download the job output within the 24-hour period
    after Amazon Glacier\n\t\t\tcompletes the job.Requests"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: http:://{host}//
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/aws-glacier/accountid-vaults-vaultname-jobs-jobid-output-get.md
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