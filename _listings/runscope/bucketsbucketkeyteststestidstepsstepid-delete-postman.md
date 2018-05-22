{
  "info": {
    "name": "Runscope Delete Buckets Tests Steps",
    "_postman_id": "0470e3ea-b05b-42d0-9722-807bd57e8659",
    "description": "Delete a step from a test.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "buckets",
      "item": [
        {
          "id": "c4f11673-df8f-4f65-b9ab-27e47d7567c0",
          "name": "buckets.bucketKey.tests.testId.steps.stepId.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.runscope.com",
              "path": [
                "buckets/:bucketKey/tests/:testId/steps/:stepId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "bucketKey",
                  "value": "bucketKey",
                  "type": "string"
                },
                {
                  "id": "testId",
                  "value": "testId",
                  "type": "string"
                },
                {
                  "id": "stepId",
                  "value": "stepId",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a step from a test"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5f30688-d943-46ef-a21a-bfbc90107748"
            }
          ]
        }
      ]
    }
  ]
}