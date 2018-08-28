---
swagger: "2.0"
x-collection-name: AWS Snowball
x-complete: 0
info:
  title: AWS Snowball API Describe Job
  version: 1.0.0
  description: |-
    Returns information about a specific job including shipping information, job status,
          and other important metadata.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CancelJob:
    get:
      summary: Cancel Job
      description: Cancels the specified job.
      operationId: cancelJob
      x-api-path-slug: actioncanceljob-get
      parameters:
      - in: query
        name: JobId
        description: The 39-character job ID for the job that you want to cancel,
          for example        JID123e4567-e89b-12d3-a456-426655440000
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /?Action=CreateJob:
    get:
      summary: Create Job
      description: |-
        Creates a job to import or export data between Amazon S3 and your on-premises data
              center.
      operationId: createJob
      x-api-path-slug: actioncreatejob-get
      parameters:
      - in: query
        name: AddressId
        description: The ID for the address that you want the Snowball shipped to
        type: string
      - in: query
        name: ClusterId
        description: The ID of a cluster
        type: string
      - in: query
        name: Description
        description: Defines an optional description of this specific job, for example
          Important        Photos 2016-08-11
        type: string
      - in: query
        name: JobType
        description: Defines the type of job that youre creating
        type: string
      - in: query
        name: KmsKeyARN
        description: The KmsKeyARN that you want to associate with this job
        type: string
      - in: query
        name: Notification
        description: Defines the Amazon Simple Notification Service (Amazon SNS) notification
          settings for      this job
        type: string
      - in: query
        name: Resources
        description: Defines the Amazon S3 buckets associated with this job
        type: string
      - in: query
        name: RoleARN
        description: The RoleARN that you want to associate with this job
        type: string
      - in: query
        name: ShippingOption
        description: The shipping speed for this job
        type: string
      - in: query
        name: SnowballCapacityPreference
        description: If your job is being created in one of the US regions, you have
          the option of      specifying what size Snowball youd like for this job
        type: string
      - in: query
        name: SnowballType
        description: The type of AWS Snowball appliance to use for this job
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /?Action=DescribeJob:
    get:
      summary: Describe Job
      description: |-
        Returns information about a specific job including shipping information, job status,
              and other important metadata.
      operationId: describeJob
      x-api-path-slug: actiondescribejob-get
      parameters:
      - in: query
        name: JobId
        description: The automatically generated ID for a job, for example        JID123e4567-e89b-12d3-a456-426655440000
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /?Action=GetJobUnlockCode:
    get:
      summary: Get Job Unlock Code
      description: Returns the UnlockCode code value for the specified job.
      operationId: getJobUnlockCode
      x-api-path-slug: actiongetjobunlockcode-get
      parameters:
      - in: query
        name: JobId
        description: The ID for the job that you want to get the UnlockCode value
          for, for      example JID123e4567-e89b-12d3-a456-426655440000
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /?Action=ListJobs:
    get:
      summary: List Jobs
      description: Returns an array of JobListEntry objects of the specified length.
      operationId: listJobs
      x-api-path-slug: actionlistjobs-get
      parameters:
      - in: query
        name: MaxResults
        description: The number of JobListEntry objects to return
        type: string
      - in: query
        name: NextToken
        description: HTTP requests are stateless
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /?Action=UpdateJob:
    get:
      summary: Update Job
      description: |-
        While a job's JobState value is New, you can update some of
              the information associated with a job.
      operationId: updateJob
      x-api-path-slug: actionupdatejob-get
      parameters:
      - in: query
        name: AddressId
        description: The ID of the updated Address object
        type: string
      - in: query
        name: Description
        description: The updated description of this jobs JobMetadata object
        type: string
      - in: query
        name: JobId
        description: The job ID of the job that you want to update, for example        JID123e4567-e89b-12d3-a456-426655440000
        type: string
      - in: query
        name: Notification
        description: The new or updated Notification object
        type: string
      - in: query
        name: Resources
        description: The updated S3Resource object (for a single Amazon S3 bucket
          or key      range), or the updated JobResource object (for multiple buckets
          or key      ranges)
        type: string
      - in: query
        name: RoleARN
        description: The new role Amazon Resource Name (ARN) that you want to associate
          with this job
        type: string
      - in: query
        name: ShippingOption
        description: The updated shipping option value of this jobs ShippingDetails      object
        type: string
      - in: query
        name: SnowballCapacityPreference
        description: The updated SnowballCapacityPreference of this jobs JobMetadata
          object
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /?Action=ListClusterJobs:
    get:
      summary: List Cluster Jobs
      description: Returns an array of JobListEntry objects of the specified length.
      operationId: listClusterJobs
      x-api-path-slug: actionlistclusterjobs-get
      parameters:
      - in: query
        name: ClusterId
        description: The 39-character ID for the cluster that you want to list, for
          example        CID123e4567-e89b-12d3-a456-426655440000
        type: string
      - in: query
        name: MaxResults
        description: The number of JobListEntry objects to return
        type: string
      - in: query
        name: NextToken
        description: HTTP requests are stateless
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Jobs
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