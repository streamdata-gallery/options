---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Describe Orderable Cluster Options
  version: 1.0.0
  description: Returns a list of orderable cluster options.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeOrderableClusterOptions:
    get:
      summary: Describe Orderable Cluster Options
      description: Returns a list of orderable cluster options.
      operationId: describeOrderableClusterOptions
      x-api-path-slug: actiondescribeorderableclusteroptions-get
      parameters:
      - in: query
        name: ClusterVersion
        description: The version filter value
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: NodeType
        description: The node type filter value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Options
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