---
swagger: "2.0"
info:
  title: Paypal Get Funding Plans
  description: Use the GetFundingPlans API operation to determine the funding sources
    that are available for a specified payment, identified by its key, which takes
    into account the preferences and country of the receiver as well as the payment
    amount. You must be both the sender of the payment and the caller of this API
    operation
  version: 1.0.0
host: svcs.sandbox.paypal.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /AdaptivePayments/GetFundingPlans:
    post:
      summary: Get Funding Plans
      description: Use the GetFundingPlans API operation to determine the funding
        sources that are available for a specified payment, identified by its key,
        which takes into account the preferences and country of the receiver as well
        as the payment amount
      operationId: AdaptivePayments.GetFundingPlans.post
      responses:
        200:
          description: OK
      tags:
      - payments
      - plans
definitions: []
x-collection-name: PayPal
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