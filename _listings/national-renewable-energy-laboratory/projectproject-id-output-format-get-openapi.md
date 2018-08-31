---
swagger: "2.0"
x-collection-name: National Renewable Energy Laboratory
x-complete: 0
info:
  title: High Performance Building Database Get Project Details
  description: This API allows users to request metadata associated with the specific
    Document.
  version: "1.0"
host: developer.nrel.gov
basePath: /api/building-case-studies
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