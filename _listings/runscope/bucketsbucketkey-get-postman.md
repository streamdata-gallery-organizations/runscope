{
  "info": {
    "name": "Runscope Get Buckets Bucketkey",
    "_postman_id": "4a29044f-14ca-4c62-b609-02ffb8c92a64",
    "description": "Returns a single bucket resource.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "buckets",
      "item": [
        {
          "id": "861d5137-7669-45be-a212-da0ec518384a",
          "name": "buckets.bucketKey.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.runscope.com",
              "path": [
                "buckets/:bucketKey"
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
            "description": "Returns a single bucket resource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce2b7ade-549c-4221-9a8d-980f39a1791e"
            }
          ]
        }
      ]
    }
  ]
}