---
swagger: "2.0"
x-collection-name: AWS API Gateway
x-complete: 0
info:
  title: AWS API Gateway API Method Integration
  version: 1.0.0
  description: Gets the method&#39;s integration responsible for passing the client-submitted
    request to the back end and performing necessary transformations to make the request
    compliant with the back end.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapis/uojnr9hd57/resources/0cjtch/methods/GET/responses/200:
    delete:
      summary: Methodresponse Delete
      description: Deletes method response settings.
      operationId: methodresponseDelete
      x-api-path-slug: restapisuojnr9hd57resources0cjtchmethodsgetresponses200-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Length
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Method
      - Responses
    get:
      summary: Method Responses
      description: Gets a method response associated with a given HTTP status code.
      operationId: methodResponses
      x-api-path-slug: restapisuojnr9hd57resources0cjtchmethodsgetresponses200-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Length
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Method
      - Responses
  /restapis/fugvjdxtri/resources/3kzxbg5sa2/methods/GET:
    patch:
      summary: Method Update
      description: Update the method settings.
      operationId: methodUpdate
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsget-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: '&quot;value&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Cache-Control
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Method
  /restapis/8ekh4oszgl/resources/4oa3abz7jc/methods/GET:
    delete:
      summary: Method Delete
      description: Delete the method resource.
      operationId: methodDelete
      x-api-path-slug: restapis8ekh4oszglresources4oa3abz7jcmethodsget-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Method
  /restapis/uojnr9hd57/resources/0cjtch/methods/GET/integration:
    get:
      summary: Method Integration
      description: Gets the method&#39;s integration responsible for passing the client-submitted
        request to the back end and performing necessary transformations to make the
        request compliant with the back end.
      operationId: methodIntegration
      x-api-path-slug: restapisuojnr9hd57resources0cjtchmethodsgetintegration-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Length
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Method
      - Integration
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