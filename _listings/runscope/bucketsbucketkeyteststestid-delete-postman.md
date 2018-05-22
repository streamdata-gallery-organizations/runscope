{
  "info": {
    "name": "Runscope Delete Buckets Tests",
    "_postman_id": "57ca8f31-5175-4220-bc02-c72240749fa6",
    "description": "Delete a test, including all steps, schedules, test-specific environments and results.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "buckets",
      "item": [
        {
          "id": "f5b3e7ac-df63-4b53-adc3-c38f1bfe140f",
          "name": "buckets.bucketKey.tests.testId.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.runscope.com",
              "path": [
                "buckets/:bucketKey/tests/:testId"
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
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a test, including all steps, schedules, test-specific environments and results"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c52c3a4f-3523-4c69-9d69-b9ebb32102b4"
            }
          ]
        }
      ]
    }
  ]
}