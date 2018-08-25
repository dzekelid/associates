---
swagger: "2.0"
x-collection-name: AWS Elastic Load Balancing
x-complete: 1
info:
  title: AWS Elastic Load Balancing API
  version: 1.0.0
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
---