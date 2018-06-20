---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost API Reference
  description: -api-v4-is-stable-with-the-mattermost-server-4-0-release--api-v3-was-deprecated-on-january-16th-2018-and-scheduled-for-removal-in-mattermost-v5-0--details-heretagapiv3deprecation--looking-for-the-api-v3-reference-it-has-moved-herehttpsapi-mattermost-comv3-
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /jobs:
    get:
      summary: Get the jobs.
      description: |-
        Get a page of jobs. Use the query parameters to modify the behaviour of this endpoint.
        __Minimum server version: 4.1__
        ##### Permissions
        Must have `manage_jobs` permission.
      operationId: get-a-page-of-jobs-use-the-query-parameters-to-modify-the-behaviour-of-this-endpoint-minimum-server-
      x-api-path-slug: jobs-get
      parameters:
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of jobs per page
      responses:
        200:
          description: OK
      tags:
      - Jobs.
  /jobs/type/{type}:
    get:
      summary: Get the jobs of the given type.
      description: |-
        Get a page of jobs of the given type. Use the query parameters to modify the behaviour of this endpoint.
        __Minimum server version: 4.1__
        ##### Permissions
        Must have `manage_jobs` permission.
      operationId: get-a-page-of-jobs-of-the-given-type-use-the-query-parameters-to-modify-the-behaviour-of-this-endpoi
      x-api-path-slug: jobstypetype-get
      parameters:
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of jobs per page
      - in: path
        name: type
        description: Job type
      responses:
        200:
          description: OK
      tags:
      - Jobs
      - Of
      - Given
      - Type.
---