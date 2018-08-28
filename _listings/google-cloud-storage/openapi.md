swagger: "2.0"
x-collection-name: Google Cloud Storage
x-complete: 1
info:
  title: Google Cloud Storage
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/transferJobs:
    get:
      summary: Get Transfer Jobs
      description: Lists transfer jobs.
      operationId: storagetransfer.transferJobs.list
      x-api-path-slug: v1transferjobs-get
      parameters:
      - in: query
        name: filter
        description: A list of query parameters specified as JSON text in the form
          of {`project_id`:my_project_id, `job_names`:[jobid1,jobid2,
      - in: query
        name: pageSize
        description: The list page size
      - in: query
        name: pageToken
        description: The list page token
      responses:
        200:
          description: OK
      tags:
      - Job
    post:
      summary: Create Transfer Jobs
      description: Creates a transfer job that runs periodically.
      operationId: storagetransfer.transferJobs.create
      x-api-path-slug: v1transferjobs-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1/{jobName}:
    get:
      summary: Get Transfer Jobs
      description: Gets a transfer job.
      operationId: storagetransfer.transferJobs.get
      x-api-path-slug: v1jobname-get
      parameters:
      - in: path
        name: jobName
        description: The job to get
      - in: query
        name: projectId
        description: The ID of the Google Developers Console project that owns the
          job
      responses:
        200:
          description: OK
      tags:
      - Job
    patch:
      summary: Update Transfer Jobs
      description: Updates a transfer job. Updating a job's transfer spec does not
        affect transfer operations that are running already. Updating the scheduling
        of a job is not allowed.
      operationId: storagetransfer.transferJobs.patch
      x-api-path-slug: v1jobname-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: jobName
        description: The name of job to update
      responses:
        200:
          description: OK
      tags:
      - Job