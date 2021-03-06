swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/configuration/timetracking/list:
    get:
      summary: Get all time tracking providers
      description: "Returns all time tracking providers. By default, Jira only has
        one time tracking provider: _JIRA provided time tracking_. However, you can
        install other time tracking providers via apps from the Atlassian Marketplace.
        For more information on time tracking providers, see the documentation for
        the [Time Tracking Provider](https://developer.atlassian.com/cloud/jira/platform/modules/time-tracking-provider/)
        module.  \n  \n**[Permissions](https://developer.atlassian.com/cloud/jira/platform/rest/#permissions)
        required:** Jira administration (that is, member of the _administrators_ [group](https://confluence.atlassian.com/x/24xjL))."
      operationId: com.atlassian.jira.rest.v2.admin.timetracking.TimeTrackingResource.getAvailableTimeTrackingImplement
      x-api-path-slug: api2configurationtimetrackinglist-get
      responses:
        200:
          description: OK
      tags:
      - Time
      - Tracking
      - Providers