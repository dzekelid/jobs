---
name: USAJobs API
x-slug: usajobs-api
description: Federal, state, and local government agencies are hiring and have thousands
  of job openings across the country, posted on USAJobs.gov and local government jobs
  sites. This Jobs API allows you to tap into a list of current jobs openings with
  the government. Jobs are searchable by keyword, location, agency, schedule, or any
  combination of these.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/usajobs.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Jobs
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/usajobs-api/apis.md
specificationVersion: "0.14"
apis:
- name: USAJobs API Search Jobs
  x-api-slug: usajobs-api
  description: his Jobs API allows you to tap into a list of current jobs openings
    with the government.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/usajobs.png
  humanURL: https://search.digitalgov.gov/developer/jobs.html
  baseURL: https://api.usa.gov////jobs/search.json
  tags: Jobs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/usajobs-api/jobssearch-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/usajobs-api/jobssearch-json-get-openapi.md
- name: USAJobs API
  x-api-slug: usajobs-api
  description: Federal, state, and local government agencies are hiring and have thousands
    of job openings across the country, posted on USAJobs.gov and local government
    jobs sites. This Jobs API allows you to tap into a list of current jobs openings
    with the government. Jobs are searchable by keyword, location, agency, schedule,
    or any combination of these.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/usajobs.png
  humanURL: https://search.digitalgov.gov/developer/jobs.html
  baseURL: https://api.usa.gov//
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/usajobs-api/openapi.md
x-common:
- type: x-website
  url: https://search.digitalgov.gov/developer/jobs.html
- type: x-terms-of-service
  url: https://www.usa.gov/About/developer-resources/terms-of-service.shtml
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---