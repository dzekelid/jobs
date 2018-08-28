---
name: Pay Run
x-slug: pay-run
description: PayRun.io is a RESTful payroll and auto enrolment API built by developers
  for developers. It is a 100% compliant solution hosted in our own private cloud,
  providing realtime payroll calculations and regulatory reporting to HMRC.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
x-kinRank: "7"
x-alexaRank: "0"
tags: Jobs
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/pay-run/apis.md
specificationVersion: "0.14"
apis:
- name: Pay Run.IO Get all DPS jobs
  x-api-slug: pay-run-io
  description: Gets all the DPS jobs
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Jobs/Dps
  tags: DPJobs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/pay-run/jobsdps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/pay-run/jobsdps-get-openapi.md
- name: Pay Run.IO Get all PayRun jobs
  x-api-slug: pay-run-io
  description: Gets all the pay run jobs
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Jobs/PayRuns
  tags: PayRun,Jobs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/pay-run/jobspayruns-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/pay-run/jobspayruns-get-openapi.md
- name: Pay Run.IO Get all RTI jobs
  x-api-slug: pay-run-io
  description: Gets all the RTI jobs
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Jobs/Rti
  tags: RTI,Jobs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/pay-run/jobsrti-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/pay-run/jobsrti-get-openapi.md
- name: Pay Run.IO
  x-api-slug: pay-run-io
  description: PayRun.io is a RESTful payroll and auto enrolment API built by developers
    for developers. It is a 100% compliant solution hosted in our own private cloud,
    providing realtime payroll calculations and regulatory reporting to HMRC.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/pay-run/openapi.md
x-common:
- type: x-website
  url: http://www.payrun.io
- type: x-documentation
  url: https://developer.payrun.io/docs/home/index.html
- type: x-twitter
  url: https://twitter.com/PayRun_io
- type: x-website
  url: http://api.test.payrun.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---