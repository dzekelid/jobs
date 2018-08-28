---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Delete Workers Jobs
  description: Delete a single scheduled job
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /harvest/source/{ident}/jobs/:
    get:
      summary: Get Harvest Source Ent Jobs
      description: List all jobs for a given source
      operationId: getHarvestSourceEntJobs
      x-api-path-slug: harvestsourceidentjobs-get
      parameters:
      - in: path
        name: ident
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
      - Jobs
  /workers/jobs/:
    get:
      summary: Get Workers Jobs
      description: List all scheduled jobs
      operationId: getWorkersJobs
      x-api-path-slug: workersjobs-get
      responses:
        200:
          description: OK
      tags:
      - Workers
      - Jobs
    post:
      summary: Add Workers Jobs
      description: Create a new scheduled job
      operationId: postWorkersJobs
      x-api-path-slug: workersjobs-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Workers
      - Jobs
  /workers/jobs/schedulables:
    get:
      summary: Get Workers Jobs Schedulables
      description: List all schedulable jobs
      operationId: getWorkersJobsSchedulables
      x-api-path-slug: workersjobsschedulables-get
      responses:
        200:
          description: OK
      tags:
      - Workers
      - Jobs
      - Schedulables
  /workers/jobs/{id}:
    delete:
      summary: Delete Workers Jobs
      description: Delete a single scheduled job
      operationId: deleteWorkersJobs
      x-api-path-slug: workersjobsid-delete
      parameters:
      - in: path
        name: id
        description: A job ID
      responses:
        200:
          description: OK
      tags:
      - Workers
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