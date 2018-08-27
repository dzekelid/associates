---
swagger: "2.0"
x-collection-name: AWS Elastic Load Balancing
x-complete: 0
info:
  title: AWS Elastic Load Balancing API Set Security Groups
  version: 1.0.0
  description: Associates the specified security groups with the specified load balancer.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SetSecurityGroups:
    get:
      summary: Set Security Groups
      description: Associates the specified security groups with the specified load
        balancer.
      operationId: setSecurityGroups
      x-api-path-slug: actionsetsecuritygroups-get
      parameters:
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      - in: query
        name: SecurityGroups.member.N
        description: The IDs of the security groups
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Groups
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