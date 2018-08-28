---
name: OnSched
x-slug: onsched
description: Build secure and scalable custom apps for Online Booking. Our flexible
  API provides many options for availability and booking. OnSched is an API first
  booking software that allows you to bring your design to life by creating your own
  booking flow. Using our robust API you can customize the interaction between your
  consumers and vendors while we do all the leg work behind the scenes. Want to offer
  online booking to your vendors? Ask about our white labelling solutions and rebrand
  our software as your own.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
x-kinRank: "7"
x-alexaRank: ""
tags: Plans
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/plans/master/_listings/onsched/apis.md
specificationVersion: "0.14"
apis:
- name: OnSched API - Returns a list of customers.
  x-api-slug: consumerv1customersplans-get
  description: "The results are returned in pages. Use the offset and limit parameters
    to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
    the other query parameters to optionally filter the results list."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plans/master/_listings/onsched/consumerv1customersplans-get-openapi.md
- name: OnSched API - Returns a customer object.
  x-api-slug: consumerv1customersplansid-get
  description: "The result returned is a single customer object. An id is required
    to find the customer. Find customer id's using either the GET consumer/v1/customers
    end point,\r\nor the GET consumer/v1/appointments end point. A customer object
    is automatically created with the first booking if it doesn't already exist."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plans/master/_listings/onsched/consumerv1customersplansid-get-openapi.md
- name: OnSched API - Returns a list of customer booking limits.
  x-api-slug: consumerv1customersidplanlimitsserviceidresourceiddatetimetz-get
  description: "The result returned is list of limit rules as defined by the subscribed
    customer plan along with Booking Counts/Minutes\r\nThe results indicate the remaining
    bookings count / minutes. Use the results in your app to determine if the customer
    should continue booking.\r\nYou can enforce Limits in periods: Daily,Weekly,Monthly
    and for maximum total limits. Maximum total limits is based on six months prior
    to\r\nthe DateTimeTz and six months after the DateTimeTz. Daily, Weekly and Monthly
    limits are based on the calculated period relative to the\r\nsubscription plan
    start. Daily,Weekly and Monthly limits can be setup on a per interval basis e.g.
    to biweekly, or daily every 10 days.\r\nSee customer plans setup in the Portal
    for more information.\r\nAll parameters are required. If resourceId is not applicable
    for a non-resource calendar, pass zero.\r\nFormat of the dateTimeTz field is 2018-10-30T10:00-5:00"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plans/master/_listings/onsched/consumerv1customersidplanlimitsserviceidresourceiddatetimetz-get-openapi.md
- name: OnSched API - Returns a list of customer booking limits.
  x-api-slug: consumerv1customersidplanlimitsserviceidresourceiddatetimetz-get
  description: "The result returned is list of limit rules as defined by the subscribed
    customer plan along with Booking Counts/Minutes\r\nThe results indicate the remaining
    bookings count / minutes. Use the results in your app to determine if the customer
    should continue booking.\r\nYou can enforce Limits in periods: Daily,Weekly,Monthly
    and for maximum total limits. Maximum total limits is based on six months prior
    to\r\nthe DateTimeTz and six months after the DateTimeTz. Daily, Weekly and Monthly
    limits are based on the calculated period relative to the\r\nsubscription plan
    start. Daily,Weekly and Monthly limits can be setup on a per interval basis e.g.
    to biweekly, or daily every 10 days.\r\nSee customer plans setup in the Portal
    for more information.\r\nAll parameters are required. If resourceId is not applicable
    for a non-resource calendar, pass zero.\r\nFormat of the dateTimeTz field is 2018-10-30T10:00-5:00"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plans/master/_listings/onsched/consumerv1customersidplanlimitsserviceidresourceiddatetimetz-get-openapi.md
- name: OnSched API - Returns a list of customer booking limits.
  x-api-slug: consumerv1customersidplanlimitsserviceidresourceiddatetimetz-get
  description: "The result returned is list of limit rules as defined by the subscribed
    customer plan along with Booking Counts/Minutes\r\nThe results indicate the remaining
    bookings count / minutes. Use the results in your app to determine if the customer
    should continue booking.\r\nYou can enforce Limits in periods: Daily,Weekly,Monthly
    and for maximum total limits. Maximum total limits is based on six months prior
    to\r\nthe DateTimeTz and six months after the DateTimeTz. Daily, Weekly and Monthly
    limits are based on the calculated period relative to the\r\nsubscription plan
    start. Daily,Weekly and Monthly limits can be setup on a per interval basis e.g.
    to biweekly, or daily every 10 days.\r\nSee customer plans setup in the Portal
    for more information.\r\nAll parameters are required. If resourceId is not applicable
    for a non-resource calendar, pass zero.\r\nFormat of the dateTimeTz field is 2018-10-30T10:00-5:00"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plans/master/_listings/onsched/consumerv1customersidplanlimitsserviceidresourceiddatetimetz-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://onenote.api.gallery.streamdata.io
- type: x-api-stack
  url: http://onsched.stack.network
- type: x-documentation
  url: https://www.onsched.com/api/docs/
- type: x-pricing
  url: https://www.onsched.com/index.html#self-service
- type: x-website
  url: http://www.onsched.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---