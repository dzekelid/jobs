---
name: AppVeyor CI
x-slug: appveyor-ci
description: We provide continuous integration tools for Windows developers. The service
  is offered for free to open-source projects, we offer subscriptions for private
  projects and AppVeyor Enterprise installations on customer premises.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
x-kinRank: "7"
x-alexaRank: "35479"
tags: Jobs
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/appveyor-ci/apis.md
specificationVersion: "0.14"
apis:
- name: App Veyor Get Buildjobs Jobid Artifacts
  x-api-slug: app-veyor
  description: Get buildjobs jobid artifacts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api//buildjobs/{jobId}/artifacts
  tags: Builds,Jobs,,Artifacts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/appveyor-ci/buildjobsjobidartifacts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/appveyor-ci/buildjobsjobidartifacts-get-openapi.md
- name: App Veyor Parameters Buildjobs Jobid Artifacts
  x-api-slug: app-veyor
  description: Parameters buildjobs jobid artifacts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api//buildjobs/{jobId}/artifacts
  tags: Builds,Jobs,,Artifacts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/appveyor-ci/buildjobsjobidartifacts-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/appveyor-ci/buildjobsjobidartifacts-parameters-openapi.md
- name: App Veyor Get Buildjobs Jobid Artifacts Artifactfilename
  x-api-slug: app-veyor
  description: Get buildjobs jobid artifacts artifactfilename.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api//buildjobs/{jobId}/artifacts/{artifactFileName}
  tags: Builds,Jobs,,Artifacts,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/appveyor-ci/buildjobsjobidartifactsartifactfilename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/appveyor-ci/buildjobsjobidartifactsartifactfilename-get-openapi.md
- name: App Veyor Parameters Buildjobs Jobid Artifacts Artifactfilename
  x-api-slug: app-veyor
  description: Parameters buildjobs jobid artifacts artifactfilename.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api//buildjobs/{jobId}/artifacts/{artifactFileName}
  tags: Builds,Jobs,,Artifacts,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/appveyor-ci/buildjobsjobidartifactsartifactfilename-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/appveyor-ci/buildjobsjobidartifactsartifactfilename-parameters-openapi.md
- name: App Veyor Get Buildjobs Jobid Log
  x-api-slug: app-veyor
  description: Get buildjobs jobid log.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api//buildjobs/{jobId}/log
  tags: Builds,Jobs,,Log
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/appveyor-ci/buildjobsjobidlog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/appveyor-ci/buildjobsjobidlog-get-openapi.md
- name: App Veyor Parameters Buildjobs Jobid Log
  x-api-slug: app-veyor
  description: Parameters buildjobs jobid log.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api//buildjobs/{jobId}/log
  tags: Builds,Jobs,,Log
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/appveyor-ci/buildjobsjobidlog-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/appveyor-ci/buildjobsjobidlog-parameters-openapi.md
- name: App Veyor
  x-api-slug: app-veyor
  description: We provide continuous integration tools for Windows developers. The
    service is offered for free to open-source projects, we offer subscriptions for
    private projects and AppVeyor Enterprise installations on customer premises.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/appveyor-ci/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/appveyor-systems-inc
- type: x-documentation
  url: https://www.appveyor.com/docs/
- type: x-email
  url: jobs@appveyor.com
- type: x-email
  url: team@appveyor.com
- type: x-email
  url: privacy@appveyor.com
- type: x-twitter
  url: https://twitter.com/appveyor
- type: x-website
  url: http://appveyor.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---