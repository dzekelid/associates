---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Assign permission scheme
  description: |-
    Associates a permission scheme with a particular project. See [Managing project permissions](https://confluence.atlassian.com/x/yodKLg) for more information about permission schemes.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg)
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/project/{projectIdOrKey}/role/{id}:
    put:
      summary: Set actors for project role
      description: |-
        Associates actors with the project role for the project, replacing all existing actors.

        If you want to add actors to the project without overwriting the existing list, then use [Add actors to project role](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-project-projectIdOrKey-role-id-post).

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg) or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
      operationId: com.atlassian.jira.rest.v2.issue.project.ProjectRoleResource.setActors_put
      x-api-path-slug: api2projectprojectidorkeyroleid-put
      parameters:
      - in: header
        name: force-account-id
      - in: path
        name: id
        description: The ID of the project role
      - in: path
        name: projectIdOrKey
        description: The project ID or project key (case sensitive)
      responses:
        200:
          description: OK
      tags:
      - Set
      - Actorsproject
      - Role
  /api/2/project/{projectKeyOrId}/permissionscheme:
    put:
      summary: Assign permission scheme
      description: |-
        Associates a permission scheme with a particular project. See [Managing project permissions](https://confluence.atlassian.com/x/yodKLg) for more information about permission schemes.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg)
      operationId: com.atlassian.jira.rest.v2.permission.ProjectPermissionSchemeResource.assignPermissionScheme_put
      x-api-path-slug: api2projectprojectkeyoridpermissionscheme-put
      parameters:
      - in: query
        name: expand
        description: Use [expand](https://developer
      - in: path
        name: projectKeyOrId
        description: The project ID or project key (case sensitive)
      responses:
        200:
          description: OK
      tags:
      - Assign
      - Permission
      - Scheme
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