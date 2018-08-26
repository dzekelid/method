---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
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
    put:
      summary: Update a payment method
      description: Updates the name of the payment method. The name of the payment
        method must be specified.
      operationId: putRestPaymentsMethods
      x-api-path-slug: restpaymentsmethods-put
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
  /rest/payments/methods/plugins/{pluginKey}:
    get:
      summary: Get a payment method
      description: Gets a payment method plugin. The plugin key must be specified.
      operationId: getRestPaymentsMethodsPluginsPluginkey
      x-api-path-slug: restpaymentsmethodspluginspluginkey-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: pluginKey
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Method
  /rest/payments/methods/{methodId}:
    get:
      summary: List payments of a payment method
      description: Lists all payments of the a payment method. The ID of the payment
        method must be specified.
      operationId: getRestPaymentsMethodsMethod
      x-api-path-slug: restpaymentsmethodsmethodid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: path
        name: methodId
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Payment
      - Method
---