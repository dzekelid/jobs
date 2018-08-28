---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 0
info:
  title: Pay Run.IO Delete the pay run job
  description: Deletes the the payrun job
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Jobs/PayRuns:
    get:
      summary: Get all PayRun jobs
      description: Gets all the pay run jobs
      operationId: GetPayRunJobs
      x-api-path-slug: jobspayruns-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - PayRun
      - Jobs
    post:
      summary: Create new PayRun job
      description: Creates the new pay run job to the queue and returns the job info
      operationId: PostNewPayRunJob
      x-api-path-slug: jobspayruns-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: PayRunJobInstruction
        description: The pay run job instruction object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - PayRun
      - Job
  /Jobs/Rti:
    get:
      summary: Get all RTI jobs
      description: Gets all the RTI jobs
      operationId: GetRtiJobs
      x-api-path-slug: jobsrti-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Jobs
    post:
      summary: Create new RTI job
      description: Creates the new RTI job to the queue and returns the job info
      operationId: PostNewRtiJob
      x-api-path-slug: jobsrti-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: RtiJobInstruction
        description: The the RTI job instruction object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - RTI
      - Job
  /Jobs/PayRuns/{JobId}:
    delete:
      summary: Delete the pay run job
      description: Deletes the the payrun job
      operationId: DeletePayRunJob
      x-api-path-slug: jobspayrunsjobid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
  /Jobs/PayRuns/{JobId}/Info:
    get:
      summary: Get the pay run job information
      description: Return the the payrun job information
      operationId: GetPayRunJobInfo
      x-api-path-slug: jobspayrunsjobidinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Information
  /Jobs/PayRuns/{JobId}/Progress:
    get:
      summary: Get the pay run job progress
      description: Return the the payrun job progress
      operationId: GetPayRunJobProgress
      x-api-path-slug: jobspayrunsjobidprogress-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Progress
  /Jobs/PayRuns/{JobId}/Status:
    get:
      summary: Get the pay run job status
      description: Return the the payrun job status
      operationId: GetPayRunJobStatus
      x-api-path-slug: jobspayrunsjobidstatus-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Status
  /Jobs/Rti/{JobId}:
    delete:
      summary: Delete the RTI job
      description: Deletes the the RTI job
      operationId: DeleteRtiJob
      x-api-path-slug: jobsrtijobid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Job
  /Jobs/Rti/{JobId}/Info:
    get:
      summary: Get the RTI job information
      description: Return the the RTI job information
      operationId: GetRtiJobInfo
      x-api-path-slug: jobsrtijobidinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Job
      - Information
  /Jobs/Rti/{JobId}/Progress:
    get:
      summary: Get the RTI job progress
      description: Return the the RTI job progress
      operationId: GetRtiJobProgress
      x-api-path-slug: jobsrtijobidprogress-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Job
      - Progress
  /Jobs/Rti/{JobId}/Status:
    get:
      summary: Get the RTI job status
      description: Return the the RTI job status
      operationId: GetRtiJobStatus
      x-api-path-slug: jobsrtijobidstatus-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Job
      - Status
  /Templates/jobinfo:
    get:
      summary: Gets the job info template
      description: Return the job info data object template
      operationId: GetJobInfoTemplate
      x-api-path-slug: templatesjobinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Job
      - Info
      - Template
  /Templates/payrunjob:
    get:
      summary: Gets the pay run job template
      description: Return the pay run job data object template
      operationId: GetPayRunJobTemplate
      x-api-path-slug: templatespayrunjob-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Template
  /Templates/payrunjobinstruction:
    get:
      summary: Gets the pay run job instruction template
      description: Return the pay run job instruction data object template
      operationId: GetPayRunJobInstructionTemplate
      x-api-path-slug: templatespayrunjobinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Instruction
      - Template
  /Templates/rtijob:
    get:
      summary: Gets the rti job template
      description: Return the rti job data object template
      operationId: GetRtiJobTemplate
      x-api-path-slug: templatesrtijob-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Job
      - Template
  /Templates/rtijobinstruction:
    get:
      summary: Gets the rti job instruction template
      description: Return the rti job instruction data object template
      operationId: GetRtiJobInstructionTemplate
      x-api-path-slug: templatesrtijobinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Job
      - Instruction
      - Template
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