swagger: "2.0"
x-collection-name: Actility
x-complete: 1
info:
  title: ThingPark DX Maker API
  description: api-providing-features-for-device-makers-such-as-preprovisioning-on-standalone-join-servers-
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /maker/v011/api
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