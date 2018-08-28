---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 0
info:
  title: AWS Cognito API Create User Import Job
  version: 1.0.0
  description: Creates the user import job.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListUserImportJobs:
    get:
      summary: List User Import Jobs
      description: Lists the user import jobs.
      operationId: listUserImportJobs
      x-api-path-slug: actionlistuserimportjobs-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of import jobs you want the request to return
        type: string
      - in: query
        name: PaginationToken
        description: An identifier that was returned from the previous call to ListUserImportJobs,
          which            can be used to return the next set of import jobs in the
          list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Imports
  /?Action=CreateUserImportJob:
    get:
      summary: Create User Import Job
      description: Creates the user import job.
      operationId: createUserImportJob
      x-api-path-slug: actioncreateuserimportjob-get
      parameters:
      - in: query
        name: CloudWatchLogsRoleArn
        description: The role ARN for the Amazon CloudWatch Logging role for the user
          import            job
        type: string
      - in: query
        name: JobName
        description: The job name for the user import job
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Imports
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