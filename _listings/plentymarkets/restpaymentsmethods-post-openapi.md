---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Create a payment method
  description: Creates a payment method. The plugin key, the payment key and the name
    of the payment method must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/payments/methodNames/{paymentMethodId}:
    get:
      summary: List all payment method names for a payment method id
      description: List all payment method names for a payment method id. The payment
        method id must be specified.
      operationId: getRestPaymentsMethodnamesPaymentmethod
      x-api-path-slug: restpaymentsmethodnamespaymentmethodid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: paymentMethodId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Payment
      - Method
      - Namesa
      - Payment
      - Method
      - Id
  /rest/payments/methodNames/{paymentMethodId}/{lang}:
    get:
      summary: Gets a payment method name by id and lang
      description: Gets a payment method name by id and lang. The ID and the requested
        lang of the payment method must be specified.
      operationId: getRestPaymentsMethodnamesPaymentmethodLang
      x-api-path-slug: restpaymentsmethodnamespaymentmethodidlang-get
      parameters:
      - in: path
        name: lang
      - in: path
        name: paymentMethodId
      responses:
        200:
          description: OK
      tags:
      - S
      - Payment
      - Method
      - Name
      - By
      - Id
      - Lang
  /rest/payments/methods:
    post:
      summary: Create a payment method
      description: Creates a payment method. The plugin key, the payment key and the
        name of the payment method must be specified.
      operationId: postRestPaymentsMethods
      x-api-path-slug: restpaymentsmethods-post
      parameters:
      - in: body
        name: /rest/payments/methods
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Method
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