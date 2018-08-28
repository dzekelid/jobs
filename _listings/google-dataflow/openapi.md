swagger: "2.0"
x-collection-name: Google Dataflow
x-complete: 1
info:
  title: Google Dataflow
  description: manages-google-cloud-dataflow-projects-on-google-cloud-platform-
  contact:
    name: Google
    url: https://google.com
  version: v1b3
host: dataflow.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1b3/projects/{projectId}/jobs:
    get:
      summary: Get Project Jobs
      description: List the jobs of a project.
      operationId: dataflow.projects.jobs.list
      x-api-path-slug: v1b3projectsprojectidjobs-get
      parameters:
      - in: query
        name: filter
        description: The kind of filter to use
      - in: query
        name: location
        description: The location that contains this job
      - in: query
        name: pageSize
        description: If there are many jobs, limit response to at most this many
      - in: query
        name: pageToken
        description: Set this to the next_page_token field of a previous responseto
          request additional results in a long list
      - in: path
        name: projectId
        description: The project which owns the jobs
      - in: query
        name: view
        description: Level of information requested in response
      responses:
        200:
          description: OK
      tags:
      - Job
    post:
      summary: Create Project Job
      description: Creates a Cloud Dataflow job.
      operationId: dataflow.projects.jobs.create
      x-api-path-slug: v1b3projectsprojectidjobs-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: location
        description: The location that contains this job
      - in: path
        name: projectId
        description: The ID of the Cloud Platform project that the job belongs to
      - in: query
        name: replaceJobId
        description: Deprecated
      - in: query
        name: view
        description: The level of information requested in response
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1b3/projects/{projectId}/jobs/{jobId}:
    get:
      summary: Get Project Job
      description: Gets the state of the specified Cloud Dataflow job.
      operationId: dataflow.projects.jobs.get
      x-api-path-slug: v1b3projectsprojectidjobsjobid-get
      parameters:
      - in: path
        name: jobId
        description: The job ID
      - in: query
        name: location
        description: The location that contains this job
      - in: path
        name: projectId
        description: The ID of the Cloud Platform project that the job belongs to
      - in: query
        name: view
        description: The level of information requested in response
      responses:
        200:
          description: OK
      tags:
      - Job
    put:
      summary: Update Project Job
      description: Updates the state of an existing Cloud Dataflow job.
      operationId: dataflow.projects.jobs.update
      x-api-path-slug: v1b3projectsprojectidjobsjobid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: jobId
        description: The job ID
      - in: query
        name: location
        description: The location that contains this job
      - in: path
        name: projectId
        description: The ID of the Cloud Platform project that the job belongs to
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1b3/projects/{projectId}/jobs/{jobId}/messages:
    get:
      summary: Get Job Status
      description: Request the job status.
      operationId: dataflow.projects.jobs.messages.list
      x-api-path-slug: v1b3projectsprojectidjobsjobidmessages-get
      parameters:
      - in: query
        name: endTime
        description: Return only messages with timestamps < end_time
      - in: path
        name: jobId
        description: The job to get messages about
      - in: query
        name: location
        description: The location which contains the job specified by job_id
      - in: query
        name: minimumImportance
        description: Filter to only get messages with importance >= level
      - in: query
        name: pageSize
        description: If specified, determines the maximum number of messages toreturn
      - in: query
        name: pageToken
        description: If supplied, this should be the value of next_page_token returnedby
          an earlier call
      - in: path
        name: projectId
        description: A project id
      - in: query
        name: startTime
        description: If specified, return only messages with timestamps >= start_time
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1b3/projects/{projectId}/jobs/{jobId}/metrics:
    get:
      summary: Get Job Metrics
      description: Request the job status.
      operationId: dataflow.projects.jobs.getMetrics
      x-api-path-slug: v1b3projectsprojectidjobsjobidmetrics-get
      parameters:
      - in: path
        name: jobId
        description: The job to get messages for
      - in: query
        name: location
        description: The location which contains the job specified by job_id
      - in: path
        name: projectId
        description: A project id
      - in: query
        name: startTime
        description: Return only metric data that has changed since this time
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1b3/projects/{projectId}/locations/{location}/jobs:
    get:
      summary: Get Project Jobs for Location
      description: List the jobs of a project.
      operationId: dataflow.projects.locations.jobs.list
      x-api-path-slug: v1b3projectsprojectidlocationslocationjobs-get
      parameters:
      - in: query
        name: filter
        description: The kind of filter to use
      - in: path
        name: location
        description: The location that contains this job
      - in: query
        name: pageSize
        description: If there are many jobs, limit response to at most this many
      - in: query
        name: pageToken
        description: Set this to the next_page_token field of a previous responseto
          request additional results in a long list
      - in: path
        name: projectId
        description: The project which owns the jobs
      - in: query
        name: view
        description: Level of information requested in response
      responses:
        200:
          description: OK
      tags:
      - Job
    post:
      summary: Create Project Job for Location
      description: Creates a Cloud Dataflow job.
      operationId: dataflow.projects.locations.jobs.create
      x-api-path-slug: v1b3projectsprojectidlocationslocationjobs-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location
        description: The location that contains this job
      - in: path
        name: projectId
        description: The ID of the Cloud Platform project that the job belongs to
      - in: query
        name: replaceJobId
        description: Deprecated
      - in: query
        name: view
        description: The level of information requested in response
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1b3/projects/{projectId}/locations/{location}/jobs/{jobId}:
    get:
      summary: Get State of Project Job for Location
      description: Gets the state of the specified Cloud Dataflow job.
      operationId: dataflow.projects.locations.jobs.get
      x-api-path-slug: v1b3projectsprojectidlocationslocationjobsjobid-get
      parameters:
      - in: path
        name: jobId
        description: The job ID
      - in: path
        name: location
        description: The location that contains this job
      - in: path
        name: projectId
        description: The ID of the Cloud Platform project that the job belongs to
      - in: query
        name: view
        description: The level of information requested in response
      responses:
        200:
          description: OK
      tags:
      - Job
    put:
      summary: Get State of Project Job for Location
      description: Updates the state of an existing Cloud Dataflow job.
      operationId: dataflow.projects.locations.jobs.update
      x-api-path-slug: v1b3projectsprojectidlocationslocationjobsjobid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: jobId
        description: The job ID
      - in: path
        name: location
        description: The location that contains this job
      - in: path
        name: projectId
        description: The ID of the Cloud Platform project that the job belongs to
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1b3/projects/{projectId}/locations/{location}/jobs/{jobId}/messages:
    get:
      summary: Get Job Status
      description: Request the job status.
      operationId: dataflow.projects.locations.jobs.messages.list
      x-api-path-slug: v1b3projectsprojectidlocationslocationjobsjobidmessages-get
      parameters:
      - in: query
        name: endTime
        description: Return only messages with timestamps < end_time
      - in: path
        name: jobId
        description: The job to get messages about
      - in: path
        name: location
        description: The location which contains the job specified by job_id
      - in: query
        name: minimumImportance
        description: Filter to only get messages with importance >= level
      - in: query
        name: pageSize
        description: If specified, determines the maximum number of messages toreturn
      - in: query
        name: pageToken
        description: If supplied, this should be the value of next_page_token returnedby
          an earlier call
      - in: path
        name: projectId
        description: A project id
      - in: query
        name: startTime
        description: If specified, return only messages with timestamps >= start_time
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1b3/projects/{projectId}/locations/{location}/jobs/{jobId}/metrics:
    get:
      summary: Get Job Status
      description: Request the job status.
      operationId: dataflow.projects.locations.jobs.getMetrics
      x-api-path-slug: v1b3projectsprojectidlocationslocationjobsjobidmetrics-get
      parameters:
      - in: path
        name: jobId
        description: The job to get messages for
      - in: path
        name: location
        description: The location which contains the job specified by job_id
      - in: path
        name: projectId
        description: A project id
      - in: query
        name: startTime
        description: Return only metric data that has changed since this time
      responses:
        200:
          description: OK
      tags:
      - Job