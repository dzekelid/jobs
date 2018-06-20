---
name: YouTube
x-slug: youtube
description: YouTube allows billions of people to discover, watch and share originally-created
  videos. YouTube provides a forum for people to connect, inform, and inspire others
  across the globe and acts as a distribution platform for original content creators
  and advertisers large and small.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Jobs
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/youtube/apis.md
specificationVersion: "0.14"
apis:
- name: Youtube Get Jobs
  x-api-slug: youtube
  description: Lists jobs.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//v1/jobs
  tags: V1, Jobs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/youtube/v1jobs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/youtube/v1jobs-get-openapi.md
- name: Youtube Add Jobs
  x-api-slug: youtube
  description: Creates a job and returns it.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//v1/jobs
  tags: V1, Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/youtube/v1jobs-post-openapi.md
- name: Youtube Delete Jobs Job
  x-api-slug: youtube
  description: Delete v1 jobs job
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//v1/jobs/{jobId}
  tags: V1, Jobs, Job
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/youtube/v1jobsjobid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/youtube/v1jobsjobid-delete-openapi.md
- name: Youtube Get Jobs Job
  x-api-slug: youtube
  description: Get v1 jobs job
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//v1/jobs/{jobId}
  tags: V1, Jobs, Job
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/youtube/v1jobsjobid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/youtube/v1jobsjobid-get-openapi.md
- name: Youtube Get Jobs Job Reports
  x-api-slug: youtube
  description: |-
    Lists reports created by a specific job.
    Returns NOT_FOUND if the job does not exist.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//v1/jobs/{jobId}/reports
  tags: V1, Jobs, Job, Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/youtube/v1jobsjobidreports-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/youtube/v1jobsjobidreports-get-openapi.md
- name: Youtube Get Jobs Job Reports Report
  x-api-slug: youtube
  description: Gets the metadata of a specific report.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//v1/jobs/{jobId}/reports/{reportId}
  tags: V1, Jobs, Job, Reports, Report
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/youtube/v1jobsjobidreportsreportid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/youtube/v1jobsjobidreportsreportid-get-openapi.md
- name: Youtube
  x-api-slug: youtube
  description: YouTube allows billions of people to discover, watch and share originally-created
    videos. YouTube provides a forum for people to connect, inform, and inspire others
    across the globe and acts as a distribution platform for original content creators
    and advertisers large and small.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/youtube/openapi.md
x-common:
- type: x-articles
  url: https://developers.google.com/youtube/articles/
- type: x-authentication
  url: https://developers.google.com/youtube/v3/guides/authentication
- type: x-blog
  url: https://youtube-eng.googleblog.com/
- type: x-blog-rss
  url: https://youtube-eng.googleblog.com/feeds/posts/default?alt=rss
- type: x-branding
  url: https://developers.google.com/youtube/branding_guidelines
- type: x-bug-report
  url: https://code.google.com/p/gdata-issues/issues/entry
- type: x-bug-report
  url: https://code.google.com/p/gdata-issues/issues/list?q=label:API-YouTube
- type: x-buttons
  url: https://developers.google.com/youtube/youtube_subscribe_button
- type: x-deprecation-policy
  url: https://developers.google.com/youtube/youtube-api-list
- type: x-developer
  url: https://developers.google.com/youtube/
- type: x-getting-started
  url: https://developers.google.com/youtube/v3/getting-started
- type: x-github
  url: https://github.com/youtube
- type: x-github
  url: https://github.com/youtube/
- type: x-terms-of-service
  url: https://developers.google.com/youtube/terms
- type: x-training
  url: https://developers.google.com/youtube/training/
- type: x-twitter
  url: https://twitter.com/YouTubeDev
- type: x-website
  url: https://www.youtube.com/
- type: x-widgets
  url: https://developers.google.com/youtube/youtube_upload_widget
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---