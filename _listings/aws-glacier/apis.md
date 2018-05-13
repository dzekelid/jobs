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
- name: Amazon Glacier API List  Jobs
  description: "DescriptionThis operation lists jobs for a vault including jobs that
    are in-progress and jobs that have\n\t\t\trecently finished. \n\t\t\tNoteAmazon
    Glacier retains recently completed jobs for a period before deleting them; however,\n\t\t\t\t\tit
    eventually removes completed jobs. The output of completed jobs can be\n\t\t\t\t\tretrieved.
    Retaining completed jobs for a period of time after they have\n\t\t\t\t\tcompleted
    enables you to get a job output in the event you miss the job\n\t\t\t\t\tcompletion
    notification or your first attempt to download it fails. For example,\n\t\t\t\t\tsuppose
    you start an archive retrieval job to download an archive. After the job\n\t\t\t\t\tcompletes,
    you start to download the archive but encounter a network error. In\n\t\t\t\t\tthis
    scenario, you can retry and download the archive while the job exists. \n\t\tTo
    retrieve an archive or retrieve a vault inventory from Amazon Glacier, you first
    initiate\n\t\t\ta job, and after the job completes, you download the data. For
    an archive retrieval, the\n\t\t\toutput is the archive data. For an inventory
    retrieval, it is the inventory list.\n\t\t\tThe List Job operation returns a list
    of these jobs sorted by job initiation\n\t\t\ttime.The List Jobs operation supports
    pagination. You should always check the response\n\t\t\t\tMarker field. If there
    are no more jobs to list, the\n\t\t\t\tMarker field is set to null. If there are
    more jobs to\n\t\t\tlist, the Marker field is set to a non-null value, which you
    can use to\n\t\t\tcontinue the pagination of the list. To return a list of jobs
    that begins at a specific\n\t\t\tjob, set the marker request parameter to the
    Marker value for\n\t\t\tthat job that you obtained from a previous List Jobs request.You
    can set a maximum limit for the number of jobs returned in the response by specifying\n\t\t\tthe
    limit parameter in the request. The default limit is 1000. The number\n\t\t\tof
    jobs returned might be fewer than the limit but the number of returned jobs never\n\t\t\texceeds
    the limit.Additionally, you can filter the jobs list returned by specifying the
    optional\n\t\t\tstatuscode parameter or completed parameter, or both. Using\n\t\t\tthe
    statuscode parameter, you can specify to return only jobs that match\n\t\t\teither
    the InProgress, Succeeded, or Failed status.\n\t\t\tUsing the completed parameter,
    you can specify to return only jobs that were\n\t\t\tcompleted (true) or jobs
    that were not completed\n\t\t\t(false).Requests"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: http:://{host}//
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/aws-glacier/accountid-vaults-vaultname-jobs-get.md
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