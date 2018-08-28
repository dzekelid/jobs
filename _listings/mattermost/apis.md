---
name: Mattermost
x-slug: mattermost
description: Open source, private cloud Slack-alternative, Workplace messaging for
  web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
  configurable, and scalable from teams to the enterprise.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
x-kinRank: "8"
x-alexaRank: "95684"
tags: Jobs
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/mattermost/apis.md
specificationVersion: "0.14"
apis:
- name: Mattermost API Get the jobs.
  x-api-slug: mattermost-api
  description: |-
    Get a page of jobs. Use the query parameters to modify the behaviour of this endpoint.
    __Minimum server version: 4.1__
    ##### Permissions
    Must have `manage_jobs` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//jobs
  tags: Jobs.
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/mattermost/jobs-get-openapi.md
- name: Mattermost API Get the jobs of the given type.
  x-api-slug: mattermost-api
  description: |-
    Get a page of jobs of the given type. Use the query parameters to modify the behaviour of this endpoint.
    __Minimum server version: 4.1__
    ##### Permissions
    Must have `manage_jobs` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//jobs/type/{type}
  tags: Jobs,Of,Given,Type.
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/mattermost/jobstypetype-get-openapi.md
- name: Mattermost API
  x-api-slug: mattermost-api
  description: Open source, private cloud Slack-alternative, Workplace messaging for
    web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
    configurable, and scalable from teams to the enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/mattermost/openapi.md
x-common:
- type: x-blog
  url: https://about.mattermost.com/blog/
- type: x-blog-rss
  url: https://about.mattermost.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/mattermost
- type: x-developer
  url: https://api.mattermost.com/
- type: x-github
  url: https://github.com/mattermost
- type: x-pricing
  url: https://about.mattermost.com/pricing/
- type: x-security
  url: https://docs.mattermost.com/overview/security.html
- type: x-twitter
  url: https://twitter.com/mattermosthq
- type: x-website
  url: https://mattermost.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---