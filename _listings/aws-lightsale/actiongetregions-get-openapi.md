---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 0
info:
  title: Amazon Lightsale API Get Regions
  version: 1.0.0
  description: Returns a list of all valid regions for Amazon Lightsail.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetRegions:
    get:
      summary: Get Regions
      description: Returns a list of all valid regions for Amazon Lightsail.
      operationId: getRegions
      x-api-path-slug: actiongetregions-get
      parameters:
      - in: query
        name: includeAvailabilityZones
        description: A Boolean value indicating whether to also include Availability
          Zones in your get      regions request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Regions
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