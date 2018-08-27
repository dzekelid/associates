---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToAssist Remote Support Associate Ticket
  description: "Associates a ticket for a particular partner with a current session.\n\n
    \ Request Parameters:                  \n                    \n    field      data
    type      description    \n    sessionId      string      The unique ID of the
    session to associate with the new partner object.    \n    userToken      string
    \     The token identifying and authenticating the user in the partner system
    that this object is being created on behalf of this user.    \n    partnerObject
    \     string      The partner object to associate with the session."
  version: 1.0.0
host: api.getgo.com
basePath: /G2A/rest/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    put:
      summary: Associate Ticket
      description: "Associates a ticket for a particular partner with a current session.\n\n
        \ Request Parameters:                  \n                    \n    field      data
        type      description    \n    sessionId      string      The unique ID of
        the session to associate with the new partner object.    \n    userToken      string
        \     The token identifying and authenticating the user in the partner system
        that this object is being created on behalf of this user.    \n    partnerObject
        \     string      The partner object to associate with the session."
      operationId: UnnammedEndpointPut
      x-api-path-slug: put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Associate
      - Ticket
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