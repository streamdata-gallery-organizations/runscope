{
  "info": {
    "name": "Runscope Get Buckets Tests",
    "_postman_id": "10f9d03f-4009-4402-b073-90c37ca7ef29",
    "description": "Returns a list of tests.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "buckets",
      "item": [
        {
          "id": "aff5ebe3-c06a-4419-8e22-69db4c61d666",
          "name": "buckets.bucketKey.tests.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.runscope.com",
              "path": [
                "buckets/:bucketKey/tests"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of tests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6df12bf-e513-4100-b3da-797a68006b3c"
            }
          ]
        }
      ]
    }
  ]
}