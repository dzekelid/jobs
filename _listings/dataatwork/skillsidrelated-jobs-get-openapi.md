---
swagger: "2.0"
x-collection-name: DataAtWork
x-complete: 0
info:
  title: Open Skills API Jobs Associated with a Skill
  description: Retrieves a collection of jobs associated with a specified skill.
  contact:
    name: Work Data Initiative
    url: http://www.dataatwork.org
  version: "1.0"
host: api.dataatwork.org
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /jobs/{id}/related_jobs:
    get:
      summary: Jobs Associated with a Job
      description: Retrieves a collection of jobs associated with a specified job.
      operationId: retrieves-a-collection-of-jobs-associated-with-a-specified-job
      x-api-path-slug: jobsidrelated-jobs-get
      parameters:
      - in: path
        name: id
        description: The UUID of the job to retrieve related jobs for
      responses:
        200:
          description: OK
      tags:
      - Jobs
      - Associated
      - Job
  /skills/{id}/related_jobs:
    get:
      summary: Jobs Associated with a Skill
      description: Retrieves a collection of jobs associated with a specified skill.
      operationId: retrieves-a-collection-of-jobs-associated-with-a-specified-skill
      x-api-path-slug: skillsidrelated-jobs-get
      parameters:
      - in: path
        name: id
        description: The UUID of the skill to retrieve jobs for
      responses:
        200:
          description: OK
      tags:
      - Jobs
      - Associated
      - Skill
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