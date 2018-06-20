---
swagger: "2.0"
x-collection-name: National Renewable Energy Laboratory
x-complete: 0
info:
  title: Transportation Laws and Incentives Fetch the details of a specific law given
    the law's ID.
  description: Fetch the details of a specific law given the law's id..
  version: 0.1.0
host: developer.nrel.gov
basePath: /api/transportation-incentives-laws
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1.{output_format}:
    get:
      summary: Return a full list of laws and incentives that match your query.
      description: Return a full list of laws and incentives that match your query..
      operationId: v1.output_format.get
      x-api-path-slug: v1-output-format-get
      parameters:
      - in: query
        name: expired
        description: Show only expired, repealed or archived laws and incentives
      - in: query
        name: incentive_type
        description: Search by the incentive type
      - in: query
        name: jurisdiction
        description: Return laws for the given Jurisdiction
      - in: query
        name: keyword
        description: Search laws by keyword in title or text
      - in: query
        name: law_type
        description: Search by the law type
      - in: query
        name: limit
        description: Limit the number of laws returned
      - in: query
        name: local
        description: Show only local examples of laws and incentives
      - in: path
        name: output_format
        description: Response format
      - in: query
        name: poc
        description: Include points of contacts in the return value
      - in: query
        name: recent
        description: Return only recently added or updated laws and incentives
      - in: query
        name: regulation_type
        description: Search by the regulation type
      - in: query
        name: technology
        description: Search by the technology type
      - in: query
        name: user_type
        description: Search by the user type
      responses:
        200:
          description: OK
      tags:
      - Return
      - Full
      - List
      - Of
      - Laws
      - Incentives
      - That
      - Match
      - Your
      - Query
  /v1/category-list.{output_format}:
    get:
      summary: Return the law categories for a given category type.
      description: Return the law categories for a given category type..
      operationId: v1.category_list.output_format.get
      x-api-path-slug: v1categorylist-output-format-get
      parameters:
      - in: path
        name: output_format
        description: Response format
      - in: query
        name: type
        description: Search by the category type
      responses:
        200:
          description: OK
      tags:
      - Return
      - Law
      - Categoriesa
      - Given
      - Category
      - Type
  /v1/pocs.{output_format}:
    get:
      summary: Get the points of contact for a given jurisdiction.
      description: Get the points of contact for a given jurisdiction..
      operationId: v1.pocs.output_format.get
      x-api-path-slug: v1pocs-output-format-get
      parameters:
      - in: query
        name: jurisdiction
        description: Return the points of contact for the given Jurisdiction
      - in: path
        name: output_format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Points
      - Of
      - Contacta
      - Given
      - Jurisdiction
  /v1/{id}.{output_format}:
    get:
      summary: Fetch the details of a specific law given the law's ID.
      description: Fetch the details of a specific law given the law's id..
      operationId: v1.id.output_format.get
      x-api-path-slug: v1id-output-format-get
      parameters:
      - in: path
        name: id
        description: The id of the law that you are searching
      - in: path
        name: output_format
        description: Response format
      - in: query
        name: poc
        description: Include points of contacts in the return value
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Details
      - Of
      - Specific
      - Law
      - Given
      - Laws
      - ID
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---