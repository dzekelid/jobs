---
swagger: "2.0"
info:
  title: Amazon Glacier API Initiate  Job
  version: 1.0.0
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
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{AccountId}/vaults/{VaultName}/jobs:
    post:
      summary: Initiate  Job
      description: Initiate Job (POST jobs)This operation initiates a job of the specified
        type, which can be an archive retrieval or vault inventory retrieval
      operationId: initiate Job (POST jobs)
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
        description: "The end of the date range in UTC for vault inventory retrieval
          that includes archives\t\t\t\t\t\t\tcreated before this date"
        type: string
      - in: query
        name: Format
        description: "When initiating a job to retrieve a vault inventory, you can
          optionally add this parameter\t\t\t\t\t\t\tto your request to specify the
          output format"
        type: string
      - in: query
        name: Limit
        description: "The maximum number of inventory items returned per vault inventory
          retrieval\t\t\t\t\t\t\trequest"
        type: string
      - in: query
        name: Marker
        description: "An opaque string that represents where to continue pagination
          of the vault inventory\t\t\t\t\t\t\tretrieval results"
        type: string
      - in: query
        name: RetrievalByteRange
        description: The byte range to retrieve for an archive retrieval
        type: string
      - in: query
        name: SNSTopic
        description: "The Amazon SNS topic ARN where Amazon Glacier sends a notification
          when the job is completed, and the\t\t\t\t\t\t\toutput is ready for you
          to download"
        type: string
      - in: query
        name: StartDate
        description: "The start of the date range in UTC for vault inventory retrieval
          that includes archives\t\t\t\t\t\t\tcreated on or after this date"
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
      - jobs
definitions: []
x-collection-name: AWS Glacier
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