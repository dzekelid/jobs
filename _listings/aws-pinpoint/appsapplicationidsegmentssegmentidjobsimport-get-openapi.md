---
swagger: "2.0"
x-collection-name: AWS Pinpoint
x-complete: 0
info:
  title: AWS Pinpoint API Import Job List by Segment
  version: 1.0.0
  description: Use the GET method to request information about the import jobs for
    a segment.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps/application-id/jobs/import:
    get:
      summary: Import Job List
      description: Use the GET method to request information about your import jobs.
      operationId: importJobList
      x-api-path-slug: appsapplicationidjobsimport-get
      responses:
        200:
          description: OK
      tags:
      - Import Job
    post:
      summary: Update Import Job List
      description: Use the POST method to create or update an import job.
      operationId: updateImportJobList
      x-api-path-slug: appsapplicationidjobsimport-post
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Import Job
  /apps/application-id/jobs/import/{job-id}:
    get:
      summary: Import Job Instance
      description: Use the GET method to request information about an import job.
      operationId: importJobInstance
      x-api-path-slug: appsapplicationidjobsimportjobid-get
      parameters:
      - in: path
        name: job-id
        description: The job id
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Import Job
  /apps/application-id/segments/segment-id/jobs/import:
    get:
      summary: Import Job List by Segment
      description: Use the GET method to request information about the import jobs
        for a segment.
      operationId: importJobListbySegment
      x-api-path-slug: appsapplicationidsegmentssegmentidjobsimport-get
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Import Job
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