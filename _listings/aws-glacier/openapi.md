---
swagger: "2.0"
x-collection-name: AWS Glacier
x-complete: 1
info:
  title: AWS Glacier API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{AccountID}/vaults/{VaultName}/jobs/{JobID}:
    get:
      summary: Describe  Job
      description: "DescriptionThis operation returns information about a job you
        previously initiated, including the job\n\t\t\tinitiation date, the user who
        initiated the job, the job status code/message and the\n\t\t\tAmazon Simple
        Notification Service (Amazon SNS) topic to notify after Amazon Glacier\n\t\t\tcompletes
        the job. For more information about initiating a job, see Initiate Job (POST
        jobs). \n\t\t\tNoteThis operation enables you to check the status of your
        job. However, it is\n\t\t\t\t\tstrongly recommended that you set up an Amazon
        SNS topic and specify it in your\n\t\t\t\t\tinitiate job request so that Amazon
        Glacier can notify the topic after it completes\n\t\t\t\t\tthe job. \n\t\tA
        job ID will not expire for at least 24 hours after Amazon Glacier completes
        the job. Requests"
      operationId: describe Job (GET JobID)
      x-api-path-slug: accountidvaultsvaultnamejobsjobid-get
      parameters:
      - in: query
        name: Action
        description: The job type
        type: string
      - in: query
        name: ArchiveId
        description: For an ArchiveRetrieval job, this is the archive ID requested
          for download
        type: string
      - in: query
        name: ArchiveSHA256TreeHash
        description: The SHA256 tree hash of the entire archive for an archive retrieval
          job
        type: string
      - in: query
        name: ArchiveSizeInBytes
        description: For an ArchiveRetrieval job, this is the size in bytes of the
          archive beingrequested for download
        type: string
      - in: query
        name: Completed
        description: The job status
        type: string
      - in: query
        name: CompletionDate
        description: The UTC time that the job request completed
        type: string
      - in: query
        name: CreationDate
        description: The UTC time that the job was created
        type: string
      - in: query
        name: EndDate
        description: The end of the date range in UTC for vault inventory retrieval
          that includes archives created before this date
        type: string
      - in: query
        name: Format
        description: The output format for the vault inventory list, which is set
          by the  Initiate Job (POST jobs) request  when initiating a job to retrieve
          a vault inventory
        type: string
      - in: query
        name: InventorySizeInBytes
        description: For an InventoryRetrieval job, this is the size in bytes of the
          inventoryrequested for download
        type: string
      - in: query
        name: JobDescription
        description: The job description you provided when you initiated the job
        type: string
      - in: query
        name: JobId
        description: The ID that represents the job in Amazon Glacier
        type: string
      - in: query
        name: Limit
        description: Specifies the maximum number of inventory items returned per
          vault inventory retrieval request
        type: string
      - in: query
        name: Marker
        description: An opaque string that represents where to continue pagination
          of the vault inventoryretrieval results
        type: string
      - in: query
        name: RetrievalByteRange
        description: The retrieved byte range for archive retrieval jobs in the formStartByteValue-EndByteValueIf
          you dont specify a range in the archive retrieval, then the wholearchive
          is retrieved; also StartByteValue equals 0,and EndByteValue equals the size
          of the archiveminus 1
        type: string
      - in: query
        name: SHA256TreeHash
        description: The SHA256 tree hash value for the requested range of an archive
        type: string
      - in: query
        name: SNSTopic
        description: An Amazon Simple Notification Service (Amazon SNS) topic that
          receivesnotification
        type: string
      - in: query
        name: StartDate
        description: The start of the date range in UTC for vault inventory retrieval
          that includes archivescreated on or after this date
        type: string
      - in: query
        name: StatusCode
        description: The status code can be InProgress, Succeeded, orFailed, and indicates
          the status of the job
        type: string
      - in: query
        name: StatusMessage
        description: A friendly message that describes the job status
        type: string
      - in: query
        name: Tier
        description: The retrieval option to use for the archive retrieval
        type: string
      - in: query
        name: VaultARN
        description: The Amazon Resource Name (ARN) of the vault from which the archiveretrieval
          was requested
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /{AccountId}/vaults/{VaultName}/jobs/{JobID}/output:
    get:
      summary: Get  Job  Output
      description: "DescriptionThis operation downloads the output of the job you
        initiated using Initiate Job (POST jobs). Depending\n\t\t\ton the job type
        you specified when you initiated the job, the output will be either the\n\t\t\tcontent
        of an archive or a vault inventory. You can download all the job output or
        download a portion of the output by specifying\n\t\t\ta byte range. For both
        archive and inventory retrieval jobs, you should verify the downloaded \n\t\t\tsize
        against the size returned in the headers from the \n\t\t\tGet Job Output response.For
        archive retrieval jobs, you should also verify that the size is what you expected.
        If\n\t\t\tyou download a portion of the output, the expected size is based
        on the range of bytes\n\t\t\tyou specified. For example, if you specify a
        range of bytes=0-1048575, you should\n\t\t\tverify your download size is 1,048,576
        bytes. If you download an entire archive, the\n\t\t\texpected size is the
        size of the archive when you uploaded it to Amazon Glacier.\n\t\t\tThe expected
        size is also returned in the headers from the \n\t\t\tGet Job Output response.In
        the case of an archive retrieval job, depending on the byte range you\n\t\t\tspecify,
        Amazon Glacier returns the checksum for the portion of the data. To ensure
        the portion you downloaded \n\t\t\tis the correct data, compute the checksum
        on the client, verify that the values match, \n\t\t\tand verify that the size
        is what you expected.A job ID does not expire for at least 24 hours after
        Amazon Glacier completes the job. That\n\t\t\tis, you can download the job
        output within the 24-hour period after Amazon Glacier\n\t\t\tcompletes the
        job.Requests"
      operationId: get Job Output (GET output)
      x-api-path-slug: accountidvaultsvaultnamejobsjobidoutput-get
      parameters:
      - type: string
      - in: query
        name: ArchiveDescription
        description: The description of an archive
        type: string
      - in: query
        name: ArchiveId
        description: The ID of an archive
        type: string
      - in: query
        name: ArchiveList
        description: An array of archive metadata
        type: string
      - in: query
        name: CreationDate
        description: The UTC date and time the archive was created
        type: string
      - in: query
        name: InventoryDate
        description: The UTC date and time of the last inventory for the vault that
          was completed afterchanges to the vault
        type: string
      - in: query
        name: SHA256TreeHash
        description: The tree hash of the archive
        type: string
      - in: query
        name: Size
        description: The size in bytes of the archive
        type: string
      - in: query
        name: VaultARN
        description: The Amazon Resource Name (ARN) resource from which the archiveretrieval
          was requested
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /{AccountId}/vaults/{VaultName}/jobs:
    post:
      summary: Initiate  Job
      description: "Initiate Job (POST jobs)This operation initiates a job of the
        specified type, which can be an archive retrieval or vault inventory retrieval.Initializing
        a Data Retrieval Job Retrieving an archive or a vault inventory are asynchronous
        operations that require you to\n\t\t\tinitiate a job. Retrieval is a two-step
        process:\n\t\t\tInitiate a retrieval job.ImportantA data retrieval policy
        can cause your initiate retrieval job request to fail with a\n\t\t\t\t\t\t\t\tPolicyEnforcedException
        exception. For more information about data\n\t\t\t\t\t\t\tretrieval policies,
        see Amazon Glacier Data Retrieval Policies. For more information about the\n\t\t\t\t\t\t\t\tPolicyEnforcedException
        exception, see Error Responses.After the job completes, download the bytes.
        \n\t\tThe retrieval request is executed asynchronously. When you initiate
        a retrieval job, Amazon Glacier creates a job\n\t\t\tand returns a job ID
        in the response. When Amazon Glacier completes the job, you can get the job
        output (archive or\n\t\t\tinventory data). For information about getting job
        output, see the Get Job Output (GET output) operation. The job must complete
        before you can get its output. To determine when a job is complete, you have
        the\n\t\t\tfollowing options:\n\t\t\tUse an Amazon SNS notification&#8212;
        You can specify an Amazon Simple Notification Service\n\t\t\t\t\t\t(Amazon
        SNS) topic to which Amazon Glacier can post a notification after the job is
        completed. You can specify\n\t\t\t\t\t\tan SNS topic per job request. The
        notification is sent only after Amazon Glacier completes the job. In\n\t\t\t\t\t\taddition
        to specifying an SNS topic per job request, you can configure vault notifications
        for a\n\t\t\t\t\t\tvault so that job notifications are sent for all retrievals.
        For more information, see Set Vault Notification Configuration (PUT\n\t\tnotification-configuration).
        Get job details&#8212; You can make a Describe Job (GET JobID) request to
        obtain job\n\t\t\t\t\t\tstatus information while a job is in progress. However,
        it is more efficient to use an Amazon SNS\n\t\t\t\t\t\tnotification to determine
        when a job is complete.\n\t\t\n\t\t\tNoteThe information you get via notification
        is same that you get by calling Describe Job (GET JobID). \n\t\tIf for a specific
        event, you add both the notification configuration on the vault and also specify
        an SNS\n\t\t\ttopic in your initiate job request, Amazon Glacier sends both
        notifications. For more information, see Set Vault Notification Configuration
        (PUT\n\t\tnotification-configuration)."
      operationId: initiate Job (POST jobs)
      x-api-path-slug: accountidvaultsvaultnamejobs-post
      parameters:
      - type: string
      - in: query
        name: ArchiveId
        description: The ID of the archive that you want to retrieve
        type: string
      - in: query
        name: Description
        description: The optional description for the job
        type: string
      - in: query
        name: EndDate
        description: The end of the date range in UTC for vault inventory retrieval
          that includes archivescreated before this date
        type: string
      - in: query
        name: Format
        description: When initiating a job to retrieve a vault inventory, you can
          optionally add this parameterto your request to specify the output format
        type: string
      - in: query
        name: Limit
        description: The maximum number of inventory items returned per vault inventory
          retrievalrequest
        type: string
      - in: query
        name: Marker
        description: An opaque string that represents where to continue pagination
          of the vault inventoryretrieval results
        type: string
      - in: query
        name: RetrievalByteRange
        description: The byte range to retrieve for an archive retrieval
        type: string
      - in: query
        name: SNSTopic
        description: The Amazon SNS topic ARN where Amazon Glacier sends a notification
          when the job is completed, and theoutput is ready for you to download
        type: string
      - in: query
        name: StartDate
        description: The start of the date range in UTC for vault inventory retrieval
          that includes archivescreated on or after this date
        type: string
      - in: query
        name: Tier
        description: The retrieval option to use for the archive retrieval
        type: string
      - in: query
        name: Type
        description: The job type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
    get:
      summary: List  Jobs
      description: "DescriptionThis operation lists jobs for a vault including jobs
        that are in-progress and jobs that have\n\t\t\trecently finished. \n\t\t\tNoteAmazon
        Glacier retains recently completed jobs for a period before deleting them;
        however,\n\t\t\t\t\tit eventually removes completed jobs. The output of completed
        jobs can be\n\t\t\t\t\tretrieved. Retaining completed jobs for a period of
        time after they have\n\t\t\t\t\tcompleted enables you to get a job output
        in the event you miss the job\n\t\t\t\t\tcompletion notification or your first
        attempt to download it fails. For example,\n\t\t\t\t\tsuppose you start an
        archive retrieval job to download an archive. After the job\n\t\t\t\t\tcompletes,
        you start to download the archive but encounter a network error. In\n\t\t\t\t\tthis
        scenario, you can retry and download the archive while the job exists. \n\t\tTo
        retrieve an archive or retrieve a vault inventory from Amazon Glacier, you
        first initiate\n\t\t\ta job, and after the job completes, you download the
        data. For an archive retrieval, the\n\t\t\toutput is the archive data. For
        an inventory retrieval, it is the inventory list.\n\t\t\tThe List Job operation
        returns a list of these jobs sorted by job initiation\n\t\t\ttime.The List
        Jobs operation supports pagination. You should always check the response\n\t\t\t\tMarker
        field. If there are no more jobs to list, the\n\t\t\t\tMarker field is set
        to null. If there are more jobs to\n\t\t\tlist, the Marker field is set to
        a non-null value, which you can use to\n\t\t\tcontinue the pagination of the
        list. To return a list of jobs that begins at a specific\n\t\t\tjob, set the
        marker request parameter to the Marker value for\n\t\t\tthat job that you
        obtained from a previous List Jobs request.You can set a maximum limit for
        the number of jobs returned in the response by specifying\n\t\t\tthe limit
        parameter in the request. The default limit is 1000. The number\n\t\t\tof
        jobs returned might be fewer than the limit but the number of returned jobs
        never\n\t\t\texceeds the limit.Additionally, you can filter the jobs list
        returned by specifying the optional\n\t\t\tstatuscode parameter or completed
        parameter, or both. Using\n\t\t\tthe statuscode parameter, you can specify
        to return only jobs that match\n\t\t\teither the InProgress, Succeeded, or
        Failed status.\n\t\t\tUsing the completed parameter, you can specify to return
        only jobs that were\n\t\t\tcompleted (true) or jobs that were not completed\n\t\t\t(false).Requests"
      operationId: list Jobs (GET jobs)
      x-api-path-slug: accountidvaultsvaultnamejobs-get
      parameters:
      - in: query
        name: Action
        description: For archive retrieval jobs, this value is ArchiveRetrieval
        type: string
      - in: query
        name: ArchiveId
        description: The ID of the archive that was requested in an archive retrieval
        type: string
      - in: query
        name: ArchiveSHA256TreeHash
        description: The SHA256 tree hash of the entire archive for an archive retrieval
        type: string
      - in: query
        name: ArchiveSizeInBytes
        description: The size of the archive for which the archive retrieval job requestwas
          initiated
        type: string
      - in: query
        name: Completed
        description: true if the job is completed; false otherwise
        type: string
      - in: query
        name: CompletionDate
        description: The Universal Coordinated Time (UTC) date when the job completed
        type: string
      - in: query
        name: CreationDate
        description: The Universal Coordinated Time (UTC) date the job started
        type: string
      - in: query
        name: EndDate
        description: The end of the date range in UTC for vault inventory retrieval
          that includes archives created before this date
        type: string
      - in: query
        name: Format
        description: The output format for the vault inventory list, which is set
          by the  Initiate Job (POST jobs) request  when initiating a job to retrieve
          a vault inventory
        type: string
      - in: query
        name: InventorySizeInBytes
        description: The size of the inventory associated with an inventory retrieval
          job request
        type: string
      - in: query
        name: JobDescription
        description: A description of the job
        type: string
      - in: query
        name: JobId
        description: The ID that represents the job in Amazon Glacier
        type: string
      - in: query
        name: JobList
        description: An array of job objects
        type: string
      - in: query
        name: Limit
        description: Specifies the maximum number of inventory items returned per
          vault inventory retrievalrequest
        type: string
      - in: query
        name: Marker
        description: An opaque string that represents where to continue pagination
          of the results
        type: string
      - in: query
        name: Marker (InventoryRetrievalParameters)
        description: An opaque string that represents where to continue pagination
          of the vault inventoryretrieval results
        type: string
      - in: query
        name: RetrievalByteRange
        description: The retrieved byte range for archive retrieval jobs in the formStartByteValue-EndByteValueIf
          no range was specified in the archive retrieval, then the wholearchive is
          retrieved and StartByteValue equals 0and EndByteValue equals the size of
          the archiveminus 1
        type: string
      - in: query
        name: SHA256TreeHash
        description: The SHA256 tree hash value for the requested range of an archive
        type: string
      - in: query
        name: SNSTopic
        description: The Amazon Resource Name (ARN) that represents an Amazon SNS
          topic where notification ofjob completion or failure is sent, if notification
          was configured in thejob initiation (Initiate Job (POST jobs))
        type: string
      - in: query
        name: StartDate
        description: The start of the date range in UTC for vault inventory retrieval
          that includes archivescreated on or after this date
        type: string
      - in: query
        name: StatusCode
        description: The job status code
        type: string
      - in: query
        name: StatusMessage
        description: The job status message
        type: string
      - in: query
        name: Tier
        description: The retrieval option to use for the archive retrieval
        type: string
      - in: query
        name: VaultARN
        description: The Amazon Resource Name (ARN) of the vault of which the job
          is asubresource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
---