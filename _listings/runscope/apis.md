---
name: Runscope
x-slug: runscope
description: API performance monitoring. Everything is going to be 200 OK
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
x-kinRank: "9"
x-alexaRank: "125183"
tags: Runscope
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/apis.md
specificationVersion: "0.14"
apis:
- name: Runscope Get Account
  x-api-slug: runscope
  description: Account Resource
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////account
  tags: Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/account-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/account-get-openapi.md
- name: Runscope Get Buckets
  x-api-slug: runscope
  description: Returns a list of buckets.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets
  tags: Buckets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/buckets-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/buckets-get-openapi.md
- name: Runscope Add Buckets
  x-api-slug: runscope
  description: Create a new bucket
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets
  tags: Buckets
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/buckets-post-openapi.md
- name: Runscope Delete Buckets Bucketkey
  x-api-slug: runscope
  description: Delete a single bucket resource.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}
  tags: Buckets, Bucketkey
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkey-delete-openapi.md
- name: Runscope Get Buckets Bucketkey
  x-api-slug: runscope
  description: Returns a single bucket resource.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}
  tags: Buckets, Bucketkey
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkey-get-openapi.md
- name: Runscope Get Buckets Environments
  x-api-slug: runscope
  description: Returns list of shared environments for a specified bucket.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/environments
  tags: Buckets, Environments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyenvironments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyenvironments-get-openapi.md
- name: Runscope Add Buckets Environments
  x-api-slug: runscope
  description: Create new shared environment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/environments
  tags: Buckets, Environments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyenvironments-post-openapi.md
- name: Runscope Put Buckets Environments
  x-api-slug: runscope
  description: Update the details of a shared environment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/environments/{environmentId}
  tags: Buckets, Environments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyenvironmentsenvironmentid-put-openapi.md
- name: Runscope Get Buckets Errors
  x-api-slug: runscope
  description: Retrieve a list of error messages in a bucket
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/errors
  tags: Buckets, Errors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyerrors-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyerrors-get-openapi.md
- name: Runscope Delete Buckets Messages
  x-api-slug: runscope
  description: Clear a bucket (remove all messages).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/messages
  tags: Buckets, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeymessages-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeymessages-delete-openapi.md
- name: Runscope Get Buckets Messages
  x-api-slug: runscope
  description: Retrieve a list of messages in a bucket
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/messages
  tags: Buckets, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeymessages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeymessages-get-openapi.md
- name: Runscope Add Buckets Messages
  x-api-slug: runscope
  description: Create a message
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/messages
  tags: Buckets, Messages
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeymessages-post-openapi.md
- name: Runscope Get Buckets Messages Message
  x-api-slug: runscope
  description: Retrieve the details for a single message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/messages/{messageId}
  tags: Buckets, Messages, Message
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeymessagesmessageid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeymessagesmessageid-get-openapi.md
- name: Runscope Get Buckets Tests
  x-api-slug: runscope
  description: Returns a list of tests.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/tests
  tags: Buckets, Tests
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeytests-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeytests-get-openapi.md
- name: Runscope Add Buckets Tests
  x-api-slug: runscope
  description: Create a test.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/tests
  tags: Buckets, Tests
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeytests-post-openapi.md
- name: Runscope Delete Buckets Tests
  x-api-slug: runscope
  description: Delete a test, including all steps, schedules, test-specific environments
    and results.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/tests/{testId}
  tags: Buckets, Tests
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestid-delete-openapi.md
- name: Runscope Get Buckets Tests
  x-api-slug: runscope
  description: Retrieve the details of a given test by ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/tests/{testId}
  tags: Buckets, Tests
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestid-get-openapi.md
- name: Runscope Put Buckets Tests
  x-api-slug: runscope
  description: Modify a test's name, description, default environment and its steps.
    To modify other individual properties of a test, make requests to the steps, environments,
    and schedules subresources of the test.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/tests/{testId}
  tags: Buckets, Tests
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestid-put-openapi.md
- name: Runscope Get Buckets Tests Environments
  x-api-slug: runscope
  description: Return details of the test's environments (only those that belong to
    the specified test)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/tests/{testId}/environments
  tags: Buckets, Tests, Environments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestidenvironments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestidenvironments-get-openapi.md
- name: Runscope Add Buckets Tests Environments
  x-api-slug: runscope
  description: Create new test environment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/tests/{testId}/environments
  tags: Buckets, Tests, Environments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestidenvironments-post-openapi.md
- name: Runscope Put Buckets Tests Environments
  x-api-slug: runscope
  description: Update the details of a test environment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/tests/{testId}/environments/{environmentId}
  tags: Buckets, Tests, Environments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestidenvironmentsenvironmentid-put-openapi.md
- name: Runscope Get Buckets Tests Metrics
  x-api-slug: runscope
  description: Return details of the test metrics for the specified timeframe.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/tests/{testId}/metrics
  tags: Buckets, Tests, Metrics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestidmetrics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestidmetrics-get-openapi.md
- name: Runscope Get Buckets Tests Steps
  x-api-slug: runscope
  description: List test steps for a test.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/tests/{testId}/steps
  tags: Buckets, Tests, Steps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestidsteps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestidsteps-get-openapi.md
- name: Runscope Add Buckets Tests Steps
  x-api-slug: runscope
  description: Add new test step.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/tests/{testId}/steps
  tags: Buckets, Tests, Steps
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestidsteps-post-openapi.md
- name: Runscope Delete Buckets Tests Steps
  x-api-slug: runscope
  description: Delete a step from a test.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/tests/{testId}/steps/{stepId}
  tags: Buckets, Tests, Steps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestidstepsstepid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestidstepsstepid-delete-openapi.md
- name: Runscope Put Buckets Tests Steps
  x-api-slug: runscope
  description: Update the details of a single test step.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////buckets/{bucketKey}/tests/{testId}/steps/{stepId}
  tags: Buckets, Tests, Steps
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/bucketsbucketkeyteststestidstepsstepid-put-openapi.md
- name: Runscope Get Teams Agents
  x-api-slug: runscope
  description: Team agents list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////teams/{teamId}/agents
  tags: Teams, Agents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/teamsteamidagents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/teamsteamidagents-get-openapi.md
- name: Runscope Get Teams Integrations
  x-api-slug: runscope
  description: Team integrations list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////teams/{teamId}/integrations
  tags: Teams, Integrations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/teamsteamidintegrations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/teamsteamidintegrations-get-openapi.md
- name: Runscope Get Teams People
  x-api-slug: runscope
  description: Teams Resource
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com////teams/{teamId}/people
  tags: Teams, People
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/teamsteamidpeople-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/teamsteamidpeople-get-openapi.md
- name: Runscope
  x-api-slug: runscope
  description: API performance monitoring. Everything is going to be 200 OK
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1752-runscope.jpg
  humanURL: http://runscope.com
  baseURL: https://api.runscope.com//
  tags: Runscope
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/runscope/master/_listings/runscope/openapi.md
x-common:
- type: x-base-url
  url: https://api.runscope.com
- type: x-blog
  url: http://blog.runscope.com/
- type: x-blog-rss
  url: http://blog.runscope.com/posts?format=rss
- type: x-crunchbase
  url: https://crunchbase.com/organization/runscope
- type: x-crunchbase
  url: http://www.crunchbase.com/company/runscope
- type: x-developer
  url: https://www.runscope.com/docs/api
- type: x-email
  url: sales@runscope.com
- type: x-email
  url: press@runscope.com
- type: x-email
  url: help@runscope.com
- type: x-email
  url: dmca@runscope.com
- type: x-github
  url: https://github.com/Runscope
- type: x-openapi-spec--authoritative
  url: https://raw.githubusercontent.com/Runscope/runscope-api-examples/master/schemas/runscope-swagger.json
- type: x-pricing
  url: https://www.runscope.com/pricing-and-plans
- type: x-privacy
  url: https://www.runscope.com/privacy
- type: x-status
  url: http://status.runscope.com/
- type: x-support
  url: https://www.runscope.com/support
- type: x-terms-of-service
  url: https://www.runscope.com/terms
- type: x-twitter
  url: https://twitter.com/Runscope
- type: x-website
  url: http://runscope.com
- type: x-website
  url: https://www.runscope.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---