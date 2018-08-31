---
swagger: "2.0"
x-collection-name: National Renewable Energy Laboratory
x-complete: 0
info:
  title: Transportation Laws and Incentives Return the law categories for a given
    category type.
  description: Return the law categories for a given category type..
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
  /project.{output_format}:
    get:
      summary: Get Projects
      description: Get Projects
      operationId: getProject
      x-api-path-slug: project-output-format-get
      parameters:
      - in: query
        name: city
        description: City
      - in: path
        name: output_format
        description: Response Format
      - in: query
        name: page
        description: Page Number
      - in: query
        name: portal
        description: Portal ID
      - in: query
        name: province
        description: 'State or Province (ex: CO, AZ)'
      - in: query
        name: region
        description: Climate Region
      - in: query
        name: search
        description: Search Text
      responses:
        200:
          description: OK
      tags:
      - Projects
  /project/{project_id}.{output_format}:
    get:
      summary: Get Project Details
      description: This API allows users to request metadata associated with the specific
        Document.
      operationId: document
      x-api-path-slug: projectproject-id-output-format-get
      parameters:
      - in: path
        name: output_format
        description: Response Format
      - in: path
        name: project_id
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
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