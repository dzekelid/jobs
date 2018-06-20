---
swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 0
info:
  title: AWS Device Farm API Get Job
  version: 1.0.0
  description: Gets information about a job.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetJob:
    get:
      summary: Get Job
      description: Gets information about a job.
      operationId: getJob
      x-api-path-slug: actiongetjob-get
      parameters:
      - in: query
        name: arn
        description: The jobs ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
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