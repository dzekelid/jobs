---
name: HERE
x-slug: here
description: HERE Technologies enables people, enterprises and cities around the world
  to harness the power of location and create innovative solutions that make our lives
  safer and more efficient. We transform information from devices, vehicles, infrastructure
  and...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
x-kinRank: "7"
x-alexaRank: "3011"
tags: Jobs
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/apis.md
specificationVersion: "0.14"
apis:
- name: Batch Geocoder API - Get Job
  x-api-slug: jobspuwwrv32you24y8mnour793chfai36ac-get
  description: "*Request the status of a batch geocoder job*\n\nTo check the status,
    make a request to the `jobs` endpoint  appending the `requestId` and using the
    parameter `action=status `\n  \n\n\n\n* **action**  `enum`\n \\- Type of request
    \ \n\n Valid values are : `cancel`, `runs`, `status`\n\n* **app_code**  `text`\n
    \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the
    client application.    You must include an `app_code` with every request.  \n\n*
    **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the
    authentication of the client application.    You must include an `app_id` with
    every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://batch.geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobspuwwrv32you24y8mnour793chfai36ac-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobspuwwrv32you24y8mnour793chfai36ac-get-openapi.md
- name: Batch Geocoder API - Add Jobs
  x-api-slug: jobs-post
  description: "* Start asynchronously geocoding a large set of addresses in one batch*\n\nSubmit
    an HTTP POST request with `action=run` and attach the input data to the body.
    \n  \n\n\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible behavior
    in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string
    used for the authentication of the client application.    You must include an
    `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_code` with every request.\n\n* **action**  `enum`\n
    \\- Type of request\n\n Valid values are : `cancel`, `run`, `status`\n\n* **mailto**
    \ `text`\n \\- Email address where completion notification is sent.\n\n* **header**
    \ `enum`\n \\- If `true`, a header row is included before the results in the output.
    \ \n\n Valid values are : `false`, `true`\n\n* **indelim**  `text`\n \\- \n\n*
    **outdelim**  `text`\n \\- \n\n* **outcols**  `text`\n \\- \n\n* **outputCombined**
    \ `enum`\n \\- \n\n Valid values are : `true`, `false`"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://batch.geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobs-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobs-post-openapi.md
- name: Batch Geocoder API - Add Jobs
  x-api-slug: jobs-post
  description: "* Start asynchronously geocoding a large set of addresses in one batch*\n\nSubmit
    an HTTP POST request with `action=run` and attach the input data to the body.
    \n  \n\n\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible behavior
    in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string
    used for the authentication of the client application.    You must include an
    `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_code` with every request.\n\n* **action**  `enum`\n
    \\- Type of request\n\n Valid values are : `cancel`, `run`, `status`\n\n* **mailto**
    \ `text`\n \\- Email address where completion notification is sent.\n\n* **header**
    \ `enum`\n \\- If `true`, a header row is included before the results in the output.
    \ \n\n Valid values are : `false`, `true`\n\n* **indelim**  `text`\n \\- \n\n*
    **outdelim**  `text`\n \\- \n\n* **outcols**  `text`\n \\- \n\n* **outputCombined**
    \ `enum`\n \\- \n\n Valid values are : `true`, `false`"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://batch.geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobs-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobs-post-openapi.md
- name: Batch Geocoder API - Add Jobs
  x-api-slug: jobs-post
  description: "* Start asynchronously geocoding a large set of addresses in one batch*\n\nSubmit
    an HTTP POST request with `action=run` and attach the input data to the body.
    \n  \n\n\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible behavior
    in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string
    used for the authentication of the client application.    You must include an
    `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_code` with every request.\n\n* **action**  `enum`\n
    \\- Type of request\n\n Valid values are : `cancel`, `run`, `status`\n\n* **mailto**
    \ `text`\n \\- Email address where completion notification is sent.\n\n* **header**
    \ `enum`\n \\- If `true`, a header row is included before the results in the output.
    \ \n\n Valid values are : `false`, `true`\n\n* **indelim**  `text`\n \\- \n\n*
    **outdelim**  `text`\n \\- \n\n* **outcols**  `text`\n \\- \n\n* **outputCombined**
    \ `enum`\n \\- \n\n Valid values are : `true`, `false`"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://batch.geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobs-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobs-post-openapi.md
- name: Batch Geocoder API - Add Jobs
  x-api-slug: jobs-post
  description: "* Start asynchronously geocoding a large set of addresses in one batch*\n\nSubmit
    an HTTP POST request with `action=run` and attach the input data to the body.
    \n  \n\n\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible behavior
    in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string
    used for the authentication of the client application.    You must include an
    `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_code` with every request.\n\n* **action**  `enum`\n
    \\- Type of request\n\n Valid values are : `cancel`, `run`, `status`\n\n* **mailto**
    \ `text`\n \\- Email address where completion notification is sent.\n\n* **header**
    \ `enum`\n \\- If `true`, a header row is included before the results in the output.
    \ \n\n Valid values are : `false`, `true`\n\n* **indelim**  `text`\n \\- \n\n*
    **outdelim**  `text`\n \\- \n\n* **outcols**  `text`\n \\- \n\n* **outputCombined**
    \ `enum`\n \\- \n\n Valid values are : `true`, `false`"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://batch.geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobs-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobs-post-openapi.md
- name: Batch Geocoder API - Get Job
  x-api-slug: jobspuwwrv32you24y8mnour793chfai36ac-get
  description: "*Request the status of a batch geocoder job*\n\nTo check the status,
    make a request to the `jobs` endpoint  appending the `requestId` and using the
    parameter `action=status `\n  \n\n\n\n* **action**  `enum`\n \\- Type of request
    \ \n\n Valid values are : `cancel`, `runs`, `status`\n\n* **app_code**  `text`\n
    \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the
    client application.    You must include an `app_code` with every request.  \n\n*
    **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the
    authentication of the client application.    You must include an `app_id` with
    every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://batch.geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobspuwwrv32you24y8mnour793chfai36ac-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobspuwwrv32you24y8mnour793chfai36ac-get-openapi.md
- name: Batch Geocoder API - Add Jobs
  x-api-slug: jobs-post
  description: "* Start asynchronously geocoding a large set of addresses in one batch*\n\nSubmit
    an HTTP POST request with `action=run` and attach the input data to the body.
    \n  \n\n\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible behavior
    in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string
    used for the authentication of the client application.    You must include an
    `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_code` with every request.\n\n* **action**  `enum`\n
    \\- Type of request\n\n Valid values are : `cancel`, `run`, `status`\n\n* **mailto**
    \ `text`\n \\- Email address where completion notification is sent.\n\n* **header**
    \ `enum`\n \\- If `true`, a header row is included before the results in the output.
    \ \n\n Valid values are : `false`, `true`\n\n* **indelim**  `text`\n \\- \n\n*
    **outdelim**  `text`\n \\- \n\n* **outcols**  `text`\n \\- \n\n* **outputCombined**
    \ `enum`\n \\- \n\n Valid values are : `true`, `false`"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://batch.geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobs-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobs-post-openapi.md
- name: Batch Geocoder API - Get Job
  x-api-slug: jobspuwwrv32you24y8mnour793chfai36ac-get
  description: "*Request the status of a batch geocoder job*\n\nTo check the status,
    make a request to the `jobs` endpoint  appending the `requestId` and using the
    parameter `action=status `\n  \n\n\n\n* **action**  `enum`\n \\- Type of request
    \ \n\n Valid values are : `cancel`, `runs`, `status`\n\n* **app_code**  `text`\n
    \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the
    client application.    You must include an `app_code` with every request.  \n\n*
    **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the
    authentication of the client application.    You must include an `app_id` with
    every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://batch.geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobspuwwrv32you24y8mnour793chfai36ac-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobspuwwrv32you24y8mnour793chfai36ac-get-openapi.md
- name: Batch Geocoder API - Get Job
  x-api-slug: jobspuwwrv32you24y8mnour793chfai36ac-get
  description: "*Request the status of a batch geocoder job*\n\nTo check the status,
    make a request to the `jobs` endpoint  appending the `requestId` and using the
    parameter `action=status `\n  \n\n\n\n* **action**  `enum`\n \\- Type of request
    \ \n\n Valid values are : `cancel`, `runs`, `status`\n\n* **app_code**  `text`\n
    \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the
    client application.    You must include an `app_code` with every request.  \n\n*
    **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the
    authentication of the client application.    You must include an `app_id` with
    every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://batch.geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobspuwwrv32you24y8mnour793chfai36ac-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/here/jobspuwwrv32you24y8mnour793chfai36ac-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://developer.here.com/blog/feed
- type: x-github
  url: https://github.com/heremaps
- type: x-postman-collection
  url: https://github.com/heremaps/postman-collections
- type: x-api-gallery
  url: http://healthcare.gov.api.gallery.streamdata.io
- type: x-api-stack
  url: http://here.stack.network
- type: x-blog
  url: https://developer.here.com/blog
- type: x-crunchbase
  url: https://crunchbase.com/organization/here-inc
- type: x-developer
  url: https://developer.here.com
- type: x-email
  url: dirk.popp@here.com
- type: x-email
  url: sebastian.kurme@here.com
- type: x-email
  url: jordan.stark@here.com
- type: x-email
  url: amy.stupavsky@here.com
- type: x-email
  url: minna.laub@here.com
- type: x-email
  url: stefanie.sirc@here.com
- type: x-email
  url: rachel.kuta@here.com
- type: x-email
  url: laurel.davis-lyons@here.com
- type: x-email
  url: linda.bradley@here.com
- type: x-email
  url: press@here.com
- type: x-twitter
  url: https://twitter.com/here
- type: x-website
  url: https://here.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---