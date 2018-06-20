{
  "info": {
    "name": "Transportation Laws and Incentives Get the points of contact for a given jurisdiction.",
    "_postman_id": "6e35a91a-1af4-4592-bc49-73122abb7103",
    "description": "Get the points of contact for a given jurisdiction..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Return",
      "item": [
        {
          "id": "2ea5eaf5-c755-4dc1-970f-1fbbbc581ff4",
          "name": "v1.output_format.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.nrel.gov",
              "path": [
                "api",
                "transportation-incentives-laws",
                "v1.:output_format"
              ],
              "query": [
                {
                  "key": "expired",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "incentive_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "jurisdiction",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "keyword",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "law_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "local",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "poc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "recent",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "regulation_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "technology",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_type",
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
            "description": "Return a full list of laws and incentives that match your query.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82167b6a-42c0-4bb9-a6cc-d07936ec0f83"
            }
          ]
        },
        {
          "id": "484a6d82-f5d3-4466-8b44-6e04d28ee8b7",
          "name": "v1.category_list.output_format.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.nrel.gov",
              "path": [
                "api",
                "transportation-incentives-laws",
                "v1/category-list.:output_format"
              ],
              "query": [
                {
                  "key": "type",
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
            "description": "Return the law categories for a given category type.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "091e91a1-d923-421b-980b-13b4bb655972"
            }
          ]
        }
      ]
    },
    {
      "name": "Points",
      "item": [
        {
          "id": "e9561175-3efb-407e-a253-bc9542a2766b",
          "name": "v1.pocs.output_format.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.nrel.gov",
              "path": [
                "api",
                "transportation-incentives-laws",
                "v1/pocs.:output_format"
              ],
              "query": [
                {
                  "key": "jurisdiction",
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
            "description": "Get the points of contact for a given jurisdiction.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80923f85-d46f-458f-8454-d6880a0c584c"
            }
          ]
        }
      ]
    }
  ]
}