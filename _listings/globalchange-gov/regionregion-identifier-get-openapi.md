---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 0
info:
  title: Global Change Information System API Get a representation of a region.
  description: Get JSON which represents the structure of a region.
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /region:
    get:
      summary: List regions.
      description: List the regions, 20 per page.
      operationId: list-the-regions-20-per-page
      x-api-path-slug: region-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the regions
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Regions
  /region/{region_identifier}:
    get:
      summary: Get a representation of a region.
      description: Get JSON which represents the structure of a region.
      operationId: get-json-which-represents-the-structure-of-a-region
      x-api-path-slug: regionregion-identifier-get
      parameters:
      - in: path
        name: region_identifier
        description: region_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Region
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