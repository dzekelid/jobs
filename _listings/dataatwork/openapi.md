---
swagger: "2.0"
x-collection-name: DataAtWork
x-complete: 1
info:
  title: Open Skills API
  description: a-complete-and-standard-data-store-for-canonical-and-emerging-skills-knowledge-abilities-tools-technolgies-and-how-they-relate-to-jobs-
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
---