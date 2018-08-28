swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/sidekiq/job_stats:
    get:
      summary: Get Sekiq Job Stats
      description: Get the Sidekiq job statistics
      operationId: getV3SidekiqJobStats
      x-api-path-slug: v3sidekiqjob-stats-get
      responses:
        200:
          description: OK
      tags:
      - Sekiq
      - Job
      - Stats