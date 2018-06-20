---
name: DataAtWork
x-slug: dataatwork
description: ""
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
  Shot 2016-10-12 at 11.19.25 PM.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Jobs
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/dataatwork/apis.md
specificationVersion: "0.14"
apis:
- name: Open Skills API Jobs Associated with a Job
  x-api-slug: open-skills-api
  description: Retrieves a collection of jobs associated with a specified job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//jobs/{id}/related_jobs
  tags: Jobs, Associated, Job
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/dataatwork/jobsidrelated-jobs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/dataatwork/jobsidrelated-jobs-get-openapi.md
- name: Open Skills API Jobs Associated with a Skill
  x-api-slug: open-skills-api
  description: Retrieves a collection of jobs associated with a specified skill.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//skills/{id}/related_jobs
  tags: Jobs, Associated, Skill
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/dataatwork/skillsidrelated-jobs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/dataatwork/skillsidrelated-jobs-get-openapi.md
- name: Open Skills API
  x-api-slug: open-skills-api
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/dataatwork/openapi.md
x-common:
- type: x-developer
  url: http://api.dataatwork.org/v1/spec/
- type: x-website
  url: http://www.dataatwork.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---