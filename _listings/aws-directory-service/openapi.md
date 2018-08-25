---
swagger: "2.0"
x-collection-name: AWS Directory Service
x-complete: 1
info:
  title: AWS Directory Service API
  version: 1.0.0
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
---