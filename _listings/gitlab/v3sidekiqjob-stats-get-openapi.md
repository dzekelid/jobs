---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Get Sekiq Job Stats
  version: 1.0.0
  description: Get the Sidekiq job statistics
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