{
  "info": {
    "name": "Transportation Laws and Incentives Return the law categories for a given category type.",
    "_postman_id": "18335947-dbfb-41b6-80d9-7eef568f9eea",
    "description": "Return the law categories for a given category type..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Return",
      "item": [
        {
          "id": "828bd281-d2df-48dc-bb4a-fdf2e72e8555",
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
              "id": "dd2f4907-2281-43fa-8ad6-9c566dda003f"
            }
          ]
        }
      ]
    }
  ]
}