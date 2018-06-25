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
tags: Jobs
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/aws-glacier/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon Glacier API Describe  Job
  x-api-slug: amazon-glacier-api
  description: "DescriptionThis operation returns information about a job you previously
    initiated, including the job\n\t\t\tinitiation date, the user who initiated the
    job, the job status code/message and the\n\t\t\tAmazon Simple Notification Service
    (Amazon SNS) topic to notify after Amazon Glacier\n\t\t\tcompletes the job. For
    more information about initiating a job, see Initiate Job (POST jobs). \n\t\t\tNoteThis
    operation enables you to check the status of your job. However, it is\n\t\t\t\t\tstrongly
    recommended that you set up an Amazon SNS topic and specify it in your\n\t\t\t\t\tinitiate
    job request so that Amazon Glacier can notify the topic after it completes\n\t\t\t\t\tthe
    job. \n\t\tA job ID will not expire for at least 24 hours after Amazon Glacier
    completes the job. Requests"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: ://///{AccountID}/vaults/{VaultName}/jobs/{JobID}
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/aws-glacier/accountidvaultsvaultnamejobsjobid-get-openapi.md
- name: Amazon Glacier API Get  Job  Output
  x-api-slug: amazon-glacier-api
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
  baseURL: ://///{AccountId}/vaults/{VaultName}/jobs/{JobID}/output
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/aws-glacier/accountidvaultsvaultnamejobsjobidoutput-get-openapi.md
- name: Amazon Glacier API Initiate  Job
  x-api-slug: amazon-glacier-api
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
  baseURL: ://///{AccountId}/vaults/{VaultName}/jobs
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/aws-glacier/accountidvaultsvaultnamejobs-post-openapi.md
- name: Amazon Glacier API List  Jobs
  x-api-slug: amazon-glacier-api
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
  baseURL: ://///{AccountId}/vaults/{VaultName}/jobs
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/aws-glacier/accountidvaultsvaultnamejobs-get-openapi.md
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
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/aws-glacier/openapi.md
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