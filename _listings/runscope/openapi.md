---
swagger: "2.0"
x-collection-name: Runscope
x-complete: 1
info:
  title: Runscope
  description: manage-runscope-programmatically-
  version: 1.0.0
host: api.runscope.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    get:
      summary: Get Account
      description: Account Resource
      operationId: account.get
      x-api-path-slug: account-get
      responses:
        200:
          description: OK
      tags:
      - Account
  /buckets:
    get:
      summary: Get Buckets
      description: Returns a list of buckets.
      operationId: buckets.get
      x-api-path-slug: buckets-get
      responses:
        200:
          description: OK
      tags:
      - Buckets
    post:
      summary: Add Buckets
      description: Create a new bucket
      operationId: buckets.post
      x-api-path-slug: buckets-post
      parameters:
      - in: body
        name: NewBucket
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Buckets
  /buckets/{bucketKey}:
    delete:
      summary: Delete Buckets Bucketkey
      description: Delete a single bucket resource.
      operationId: buckets.bucketKey.delete
      x-api-path-slug: bucketsbucketkey-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Bucketkey
    get:
      summary: Get Buckets Bucketkey
      description: Returns a single bucket resource.
      operationId: buckets.bucketKey.get
      x-api-path-slug: bucketsbucketkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Bucketkey
  /buckets/{bucketKey}/environments:
    get:
      summary: Get Buckets Environments
      description: Returns list of shared environments for a specified bucket.
      operationId: buckets.bucketKey.environments.get
      x-api-path-slug: bucketsbucketkeyenvironments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Environments
    post:
      summary: Add Buckets Environments
      description: Create new shared environment.
      operationId: buckets.bucketKey.environments.post
      x-api-path-slug: bucketsbucketkeyenvironments-post
      parameters:
      - in: body
        name: NewEnvironment
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Environments
  /buckets/{bucketKey}/environments/{environmentId}:
    put:
      summary: Put Buckets Environments
      description: Update the details of a shared environment.
      operationId: buckets.bucketKey.environments.environmentId.put
      x-api-path-slug: bucketsbucketkeyenvironmentsenvironmentid-put
      parameters:
      - in: body
        name: ModifiedEnvironment
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Environments
  /buckets/{bucketKey}/errors:
    get:
      summary: Get Buckets Errors
      description: Retrieve a list of error messages in a bucket
      operationId: buckets.bucketKey.errors.get
      x-api-path-slug: bucketsbucketkeyerrors-get
      parameters:
      - in: query
        name: before
        description: Only return messages before the given Unix timestamp
      - in: query
        name: count
        description: Maxiumum number of messages to return
      - in: query
        name: No Name
      - in: query
        name: since
        description: Only return messages after the given Unix timestamp
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Errors
  /buckets/{bucketKey}/messages:
    delete:
      summary: Delete Buckets Messages
      description: Clear a bucket (remove all messages).
      operationId: buckets.bucketKey.messages.delete
      x-api-path-slug: bucketsbucketkeymessages-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Messages
    get:
      summary: Get Buckets Messages
      description: Retrieve a list of messages in a bucket
      operationId: buckets.bucketKey.messages.get
      x-api-path-slug: bucketsbucketkeymessages-get
      parameters:
      - in: query
        name: before
        description: Only return messages before the given Unix timestamp
      - in: query
        name: count
        description: Maxiumum number of messages to return
      - in: query
        name: No Name
      - in: query
        name: since
        description: Only return messages after the given Unix timestamp
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Messages
    post:
      summary: Add Buckets Messages
      description: Create a message
      operationId: buckets.bucketKey.messages.post
      x-api-path-slug: bucketsbucketkeymessages-post
      parameters:
      - in: body
        name: NewMessage
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Messages
  /buckets/{bucketKey}/messages/{messageId}:
    get:
      summary: Get Buckets Messages Message
      description: Retrieve the details for a single message.
      operationId: buckets.bucketKey.messages.messageId.get
      x-api-path-slug: bucketsbucketkeymessagesmessageid-get
      parameters:
      - in: path
        name: messageId
        description: The unique identifier for this message
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Messages
      - Message
  /buckets/{bucketKey}/tests:
    get:
      summary: Get Buckets Tests
      description: Returns a list of tests.
      operationId: buckets.bucketKey.tests.get
      x-api-path-slug: bucketsbucketkeytests-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
    post:
      summary: Add Buckets Tests
      description: Create a test.
      operationId: buckets.bucketKey.tests.post
      x-api-path-slug: bucketsbucketkeytests-post
      parameters:
      - in: body
        name: NewTest
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
  /buckets/{bucketKey}/tests/{testId}:
    delete:
      summary: Delete Buckets Tests
      description: Delete a test, including all steps, schedules, test-specific environments
        and results.
      operationId: buckets.bucketKey.tests.testId.delete
      x-api-path-slug: bucketsbucketkeyteststestid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
    get:
      summary: Get Buckets Tests
      description: Retrieve the details of a given test by ID.
      operationId: buckets.bucketKey.tests.testId.get
      x-api-path-slug: bucketsbucketkeyteststestid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
    put:
      summary: Put Buckets Tests
      description: Modify a test's name, description, default environment and its
        steps. To modify other individual properties of a test, make requests to the
        steps, environments, and schedules subresources of the test.
      operationId: buckets.bucketKey.tests.testId.put
      x-api-path-slug: bucketsbucketkeyteststestid-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
  /buckets/{bucketKey}/tests/{testId}/environments:
    get:
      summary: Get Buckets Tests Environments
      description: Return details of the test's environments (only those that belong
        to the specified test)
      operationId: buckets.bucketKey.tests.testId.environments.get
      x-api-path-slug: bucketsbucketkeyteststestidenvironments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Environments
    post:
      summary: Add Buckets Tests Environments
      description: Create new test environment.
      operationId: buckets.bucketKey.tests.testId.environments.post
      x-api-path-slug: bucketsbucketkeyteststestidenvironments-post
      parameters:
      - in: body
        name: NewEnvironment
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Environments
  /buckets/{bucketKey}/tests/{testId}/environments/{environmentId}:
    put:
      summary: Put Buckets Tests Environments
      description: Update the details of a test environment.
      operationId: buckets.bucketKey.tests.testId.environments.environmentId.put
      x-api-path-slug: bucketsbucketkeyteststestidenvironmentsenvironmentid-put
      parameters:
      - in: body
        name: ModifiedEnvironment
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Environments
  /buckets/{bucketKey}/tests/{testId}/metrics:
    get:
      summary: Get Buckets Tests Metrics
      description: Return details of the test metrics for the specified timeframe.
      operationId: buckets.bucketKey.tests.testId.metrics.get
      x-api-path-slug: bucketsbucketkeyteststestidmetrics-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Metrics
  /buckets/{bucketKey}/tests/{testId}/steps:
    get:
      summary: Get Buckets Tests Steps
      description: List test steps for a test.
      operationId: buckets.bucketKey.tests.testId.steps.get
      x-api-path-slug: bucketsbucketkeyteststestidsteps-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Steps
    post:
      summary: Add Buckets Tests Steps
      description: Add new test step.
      operationId: buckets.bucketKey.tests.testId.steps.post
      x-api-path-slug: bucketsbucketkeyteststestidsteps-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: TestStep
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Steps
  /buckets/{bucketKey}/tests/{testId}/steps/{stepId}:
    delete:
      summary: Delete Buckets Tests Steps
      description: Delete a step from a test.
      operationId: buckets.bucketKey.tests.testId.steps.stepId.delete
      x-api-path-slug: bucketsbucketkeyteststestidstepsstepid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Steps
    put:
      summary: Put Buckets Tests Steps
      description: Update the details of a single test step.
      operationId: buckets.bucketKey.tests.testId.steps.stepId.put
      x-api-path-slug: bucketsbucketkeyteststestidstepsstepid-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: TestStep
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Steps
  /teams/{teamId}/agents:
    get:
      summary: Get Teams Agents
      description: Team agents list
      operationId: teams.teamId.agents.get
      x-api-path-slug: teamsteamidagents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Agents
  /teams/{teamId}/integrations:
    get:
      summary: Get Teams Integrations
      description: Team integrations list
      operationId: teams.teamId.integrations.get
      x-api-path-slug: teamsteamidintegrations-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Integrations
  /teams/{teamId}/people:
    get:
      summary: Get Teams People
      description: Teams Resource
      operationId: teams.teamId.people.get
      x-api-path-slug: teamsteamidpeople-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Teams
      - People
---