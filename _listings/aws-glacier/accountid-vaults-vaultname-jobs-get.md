---
swagger: "2.0"
info:
  title: Amazon Glacier API List  Jobs
  version: 1.0.0
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
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{AccountId}/vaults/{VaultName}/jobs:
    get:
      summary: List  Jobs
      description: "DescriptionThis operation lists jobs for a vault including jobs
        that are in-progress and jobs that have\n\t\t\trecently finished"
      operationId: list Jobs (GET jobs)
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
        description: "The size of the archive for which the archive retrieval job
          request\t\t\t\t\t\t\twas initiated"
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
        description: "The end of the date range in UTC for vault inventory retrieval
          that includes \t\t\t\t\t\t\tarchives created before this date"
        type: string
      - in: query
        name: Format
        description: "The output format for the vault inventory list, which is set
          by the  \t\t\t\t\t\t\tInitiate Job (POST jobs) request  \t\t\t\t\t\t\twhen
          initiating a job to retrieve a vault inventory"
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
        description: "Specifies the maximum number of inventory items returned per
          vault inventory retrieval\t\t\t\t\t\t\trequest"
        type: string
      - in: query
        name: Marker
        description: An opaque string that represents where to continue pagination
          of the results
        type: string
      - in: query
        name: Marker (InventoryRetrievalParameters)
        description: "An opaque string that represents where to continue pagination
          of the vault inventory\t\t\t\t\t\t\tretrieval results"
        type: string
      - in: query
        name: RetrievalByteRange
        description: "The retrieved byte range for archive retrieval jobs in the form\t\t\t\t\t\t\t\tStartByteValue-EndByteValue\t\t\t\t\t\t\tIf
          no range was specified in the archive retrieval, then the whole\t\t\t\t\t\t\tarchive
          is retrieved and StartByteValue equals 0\t\t\t\t\t\t\tand EndByteValue equals
          the size of the archive\t\t\t\t\t\t\tminus 1"
        type: string
      - in: query
        name: SHA256TreeHash
        description: The SHA256 tree hash value for the requested range of an archive
        type: string
      - in: query
        name: SNSTopic
        description: "The Amazon Resource Name (ARN) that represents an Amazon SNS
          topic where notification of\t\t\t\t\t\t\tjob completion or failure is sent,
          if notification was configured in the\t\t\t\t\t\t\tjob initiation (Initiate
          Job (POST jobs))"
        type: string
      - in: query
        name: StartDate
        description: "The start of the date range in UTC for vault inventory retrieval
          that includes archives\t\t\t\t\t\t\tcreated on or after this date"
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
        description: "The Amazon Resource Name (ARN) of the vault of which the job
          is a\t\t\t\t\t\t\tsubresource"
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