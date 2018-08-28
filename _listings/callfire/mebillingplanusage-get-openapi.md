---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Find plan usage
  description: Searches for the data of a billing plan usage for the user. Returns
    the data of a billing plan usage for the current month
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/billing/plan-usage:
    get:
      summary: Find plan usage
      description: Searches for the data of a billing plan usage for the user. Returns
        the data of a billing plan usage for the current month
      operationId: getBillingPlanUsage
      x-api-path-slug: mebillingplanusage-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Billing
      - Plan-usage
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