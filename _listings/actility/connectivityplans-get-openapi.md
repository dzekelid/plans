---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Core API Connectivity plans retrieval
  description: Retrieves a list of connectivity plans existing within authorized scopes.
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /core/v141/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /connectivityPlans:
    get:
      summary: Connectivity plans retrieval
      description: Retrieves a list of connectivity plans existing within authorized
        scopes.
      operationId: retrieves-a-list-of-connectivity-plans-existing-within-authorized-scopes
      x-api-path-slug: connectivityplans-get
      responses:
        200:
          description: OK
      tags:
      - Connectivity
      - Plans
      - Retrieval
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