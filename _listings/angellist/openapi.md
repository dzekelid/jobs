swagger: "2.0"
x-collection-name: AngelList
x-complete: 1
info:
  title: AngelList
  description: the-angellist-api-provides-developers-with-a-restful-interface-to-the-angellist-data-set--for-more-information-read-the-oauth-faq-
  termsOfService: https://angel.co/terms
  contact:
    name: AngelList
    url: https://angel.co/api
    email: api@angel.co
  version: v1
host: api.angel.co
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /jobs:
    get:
      summary: Get Jobs
      description: Get jobs.
      operationId: jobs
      x-api-path-slug: jobs-get
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Jobs
  /jobs/{job_id}:
    get:
      summary: Get Job
      description: Get job.
      operationId: job
      x-api-path-slug: jobsjob-id-get
      parameters:
      - in: path
        name: job_id
        description: The id for the job
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Jobs