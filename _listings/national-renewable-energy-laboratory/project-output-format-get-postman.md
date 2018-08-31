{
  "info": {
    "name": "High Performance Building Database Get Projects",
    "_postman_id": "aa87bf13-9b4d-4d80-8ef6-82bd0e8fbfa5",
    "description": "Get Projects",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "7b8c2fd6-a179-4a80-8297-db0ba52d93c3",
          "name": "getProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.nrel.gov",
              "path": [
                "api",
                "building-case-studies",
                "project.:output_format"
              ],
              "query": [
                {
                  "key": "city",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "portal",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "province",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "region",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "search",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "output_format",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Projects"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83271e16-c6b9-4bdb-afdc-4631acc81d72"
            }
          ]
        }
      ]
    }
  ]
}