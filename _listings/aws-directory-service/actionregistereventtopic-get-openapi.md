---
swagger: "2.0"
x-collection-name: AWS Directory Service
x-complete: 0
info:
  title: AWS Directory Service API Register Event Topic
  version: 1.0.0
  description: Associates a directory with an SNS topic.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RegisterEventTopic:
    get:
      summary: Register Event Topic
      description: Associates a directory with an SNS topic.
      operationId: registerEventTopic
      x-api-path-slug: actionregistereventtopic-get
      parameters:
      - in: query
        name: DirectoryId
        description: The Directory ID that will publish status messages to the SNS
          topic
        type: string
      - in: query
        name: TopicName
        description: The SNS topic name to which the directory will publish status
          messages
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Topics
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