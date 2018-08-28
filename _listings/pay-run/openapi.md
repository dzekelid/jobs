---
swagger: "2.0"
x-collection-name: Pay Run
x-complete: 1
info:
  title: Pay Run.IO
  description: open-scableable-transparent-payroll-api-
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
  /Jobs/Dps:
    get:
      summary: Get all DPS jobs
      description: Gets all the DPS jobs
      operationId: GetDpsJobs
      x-api-path-slug: jobsdps-get
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
      - DPJobs
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
---