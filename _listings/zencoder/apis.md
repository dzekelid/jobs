---
name: Zencoder
x-slug: zencoder
description: Audio and video encoding/transcoding software as a service. Convert videos
  online into web and mobile formats using our cloud encoding API.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/282-zencoder.jpg
x-kinRank: "8"
x-alexaRank: "596400"
tags: Jobs
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/apis.md
specificationVersion: "0.14"
apis:
- name: Zencoder API List Jobs
  x-api-slug: zencoder-api
  description: A list of jobs can be obtained by sending an HTTP GET request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/282-zencoder.jpg
  humanURL: http://zencoder.com/
  baseURL: https://app.zencoder.com//api/v2//jobs
  tags: Jobs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/jobs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/jobs-get-openapi.md
- name: Zencoder API Create a Job
  x-api-slug: zencoder-api
  description: Encoding jobs are created by sending an HTTP POST request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/282-zencoder.jpg
  humanURL: http://zencoder.com/
  baseURL: https://app.zencoder.com//api/v2//jobs
  tags: Jobs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/jobs-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/jobs-post-openapi.md
- name: Zencoder API Get Job Details
  x-api-slug: zencoder-api
  description: Get Job Details
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/282-zencoder.jpg
  humanURL: http://zencoder.com/
  baseURL: https://app.zencoder.com//api/v2//jobs/{job_id}
  tags: Jobs,Job,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/jobsjob-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/jobsjob-id-get-openapi.md
- name: Zencoder API Cancel a Job
  x-api-slug: zencoder-api
  description: If you wish to cancel a job that has not yet finished processing you
    may send a request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/282-zencoder.jpg
  humanURL: http://zencoder.com/
  baseURL: https://app.zencoder.com//api/v2//jobs/{job_id}/cancel
  tags: Jobs,Job,Id,Cancel
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/jobsjob-idcancel-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/jobsjob-idcancel-put-openapi.md
- name: Zencoder API Finish a LIve Job
  x-api-slug: zencoder-api
  description: Finishes the input on a Live streaming job.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/282-zencoder.jpg
  humanURL: http://zencoder.com/
  baseURL: https://app.zencoder.com//api/v2//jobs/{job_id}/finish
  tags: Jobs,Job,Id,Finish
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/jobsjob-idfinish-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/jobsjob-idfinish-put-openapi.md
- name: Zencoder API Job Progress
  x-api-slug: zencoder-api
  description: 'The return will contain one or more of the following keys: state,
    input, outputs, and progress.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/282-zencoder.jpg
  humanURL: http://zencoder.com/
  baseURL: https://app.zencoder.com//api/v2//jobs/{job_id}/progress
  tags: Jobs,Job,Id,Progress
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/jobsjob-idprogress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/jobsjob-idprogress-get-openapi.md
- name: Zencoder API Resubmit a Job
  x-api-slug: zencoder-api
  description: If a job has failed processing you may request that it be attempted
    again.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/282-zencoder.jpg
  humanURL: http://zencoder.com/
  baseURL: https://app.zencoder.com//api/v2//jobs/{job_id}/resubmit
  tags: Jobs,Job,Id,Resubmit
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/jobsjob-idresubmit-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/jobsjob-idresubmit-put-openapi.md
- name: Zencoder API
  x-api-slug: zencoder-api
  description: Zencoders Video Encoding API allows you to seamlessly integrate your
    application with Zencoders extremely fast and scalable encoding platform. Our
    RESTful API is extensively documented with easy-to-use guides and detailed descriptions,
    as well as thoroughly tested code libraries and code examples for every encoding
    setting. Backed by an uptime SLA and live support with real encoding engineers,
    integrating with Zencoder couldnt be easier.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/282-zencoder.jpg
  humanURL: http://zencoder.com/
  baseURL: https://app.zencoder.com//api/v2
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/zencoder/openapi.md
x-common:
- type: x-base
  url: https://app.zencoder.com/api/
- type: x-blog
  url: http://blog.zencoder.com/
- type: x-blog-rss
  url: http://blog.zencoder.com/feed/
- type: x-contact-form
  url: https://zencoder.com/en/sales
- type: x-crunchbase
  url: http://www.crunchbase.com/company/zencoder
- type: x-crunchbase
  url: https://crunchbase.com/organization/zencoder
- type: x-developer
  url: http://zencoder.com/api/
- type: x-email
  url: privacy@zencoder.com
- type: x-error-codes
  url: https://app.zencoder.com/docs/errors
- type: x-facebook
  url: http://www.facebook.com/zencoderinc
- type: x-faq
  url: https://app.zencoder.com/docs/faq
- type: x-getting-started
  url: https://app.zencoder.com/docs/guides/getting-started
- type: x-github
  url: https://github.com/zencoder
- type: x-pricing
  url: https://zencoder.com/en/file-transcoding/pricing#basic
- type: x-pricing
  url: https://zencoder.com/en/live-transcoding/pricing
- type: x-privacy
  url: http://zencoder.com/privacy
- type: x-selfservice-registration
  url: https://app.zencoder.com/signup
- type: x-terms-of-service
  url: http://zencoder.com/terms
- type: x-twitter
  url: https://twitter.com/zencoderinc
- type: x-website
  url: http://zencoder.com/
- type: x-website
  url: http://zencoder.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---