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
- name: Amazon Glacier API Initiate  Job
  description: "Initiate Job (POST jobs)This operation initiates a job of the specified
    type, which can be an archive retrieval or vault inventory retrieval.Initializing
    a Data Retrieval Job Retrieving an archive or a vault inventory are asynchronous
    operations that require you to\n\t\t\tinitiate a job. Retrieval is a two-step
    process:\n\t\t\tInitiate a retrieval job.ImportantA data retrieval policy can
    cause your initiate retrieval job request to fail with a\n\t\t\t\t\t\t\t\tPolicyEnforcedException
    exception. For more information about data\n\t\t\t\t\t\t\tretrieval policies,
    see Amazon Glacier Data Retrieval Policies. For more information about the\n\t\t\t\t\t\t\t\tPolicyEnforcedException
    exception, see Error Responses.After the job completes, download the bytes. \n\t\tThe
    retrieval request is executed asynchronously. When you initiate a retrieval job,
    Amazon Glacier creates a job\n\t\t\tand returns a job ID in the response. When
    Amazon Glacier completes the job, you can get the job output (archive or\n\t\t\tinventory
    data). For information about getting job output, see the Get Job Output (GET output)
    operation. The job must complete before you can get its output. To determine when
    a job is complete, you have the\n\t\t\tfollowing options:\n\t\t\tUse an Amazon
    SNS notification&#8212; You can specify an Amazon Simple Notification Service\n\t\t\t\t\t\t(Amazon
    SNS) topic to which Amazon Glacier can post a notification after the job is completed.
    You can specify\n\t\t\t\t\t\tan SNS topic per job request. The notification is
    sent only after Amazon Glacier completes the job. In\n\t\t\t\t\t\taddition to
    specifying an SNS topic per job request, you can configure vault notifications
    for a\n\t\t\t\t\t\tvault so that job notifications are sent for all retrievals.
    For more information, see Set Vault Notification Configuration (PUT\n\t\tnotification-configuration).
    Get job details&#8212; You can make a Describe Job (GET JobID) request to obtain
    job\n\t\t\t\t\t\tstatus information while a job is in progress. However, it is
    more efficient to use an Amazon SNS\n\t\t\t\t\t\tnotification to determine when
    a job is complete.\n\t\t\n\t\t\tNoteThe information you get via notification is
    same that you get by calling Describe Job (GET JobID). \n\t\tIf for a specific
    event, you add both the notification configuration on the vault and also specify
    an SNS\n\t\t\ttopic in your initiate job request, Amazon Glacier sends both notifications.
    For more information, see Set Vault Notification Configuration (PUT\n\t\tnotification-configuration)."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: http:://{host}//
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/aws-glacier/accountid-vaults-vaultname-jobs-post.md
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