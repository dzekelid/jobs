---
swagger: "2.0"
x-collection-name: Google Cloud Dataproc
x-complete: 0
info:
  title: Google Cloud Dataproc API Submit Job
  description: Submits a job to a cluster.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: dataproc.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/projects/{projectId}/regions/{region}/jobs:
    get:
      summary: Get Region Jobs
      description: Lists regions/{region}/jobs in a project.
      operationId: dataproc.projects.regions.jobs.list
      x-api-path-slug: v1projectsprojectidregionsregionjobs-get
      parameters:
      - in: query
        name: clusterName
        description: Optional If set, the returned jobs list includes only jobs that
          were submitted to the named cluster
      - in: query
        name: filter
        description: Optional A filter constraining the jobs to list
      - in: query
        name: jobStateMatcher
        description: Optional Specifies enumerated categories of jobs to list (default
          = match ALL jobs)
      - in: query
        name: pageSize
        description: Optional The number of results to return in each response
      - in: query
        name: pageToken
        description: Optional The page token, returned by a previous call, to request
          the next page of results
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          job belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1/projects/{projectId}/regions/{region}/jobs/{jobId}:
    delete:
      summary: Delete Job
      description: Deletes the job from the project. If the job is active, the delete
        fails, and the response returns FAILED_PRECONDITION.
      operationId: dataproc.projects.regions.jobs.delete
      x-api-path-slug: v1projectsprojectidregionsregionjobsjobid-delete
      parameters:
      - in: path
        name: jobId
        description: Required The job ID
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          job belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Job
    get:
      summary: Get Job
      description: Gets the resource representation for a job in a project.
      operationId: dataproc.projects.regions.jobs.get
      x-api-path-slug: v1projectsprojectidregionsregionjobsjobid-get
      parameters:
      - in: path
        name: jobId
        description: Required The job ID
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          job belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Job
    patch:
      summary: Update Job
      description: Updates a job in a project.
      operationId: dataproc.projects.regions.jobs.patch
      x-api-path-slug: v1projectsprojectidregionsregionjobsjobid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: jobId
        description: Required The job ID
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          job belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      - in: query
        name: updateMask
        description: Required Specifies the path, relative to Job, of the field to
          update
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1/projects/{projectId}/regions/{region}/jobs/{jobId}:cancel:
    post:
      summary: Cancel Job
      description: Starts a job cancellation request. To access the job resource after
        cancellation, call regions/{region}/jobs.list or regions/{region}/jobs.get.
      operationId: dataproc.projects.regions.jobs.cancel
      x-api-path-slug: v1projectsprojectidregionsregionjobsjobidcancel-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: jobId
        description: Required The job ID
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          job belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1/projects/{projectId}/regions/{region}/jobs:submit:
    post:
      summary: Submit Job
      description: Submits a job to a cluster.
      operationId: dataproc.projects.regions.jobs.submit
      x-api-path-slug: v1projectsprojectidregionsregionjobssubmit-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          job belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Job
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