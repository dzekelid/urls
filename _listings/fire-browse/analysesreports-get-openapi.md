---
swagger: "2.0"
x-collection-name: Fire Browse
x-complete: 0
info:
  title: Fire Browse Beta API Retrieve links to summary reports from Firehose analysis
    runs.
  description: This service returns URLs to the analysis result reports for runs of
    the Broad Institute GDAC Firehose analysis pipeline. At least one year of run
    reports are maintained in the database, but the reports from the latest run will
    be returned by default. The set of Nozzle reports returned may be filtered by
    disease cohort, report type and report name.
  version: 1.1.35 (2016-09-27 10:12:23 6a47e74011281b2aa
host: firebrowse.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Analyses/Reports:
    get:
      summary: Retrieve links to summary reports from Firehose analysis runs.
      description: This service returns URLs to the analysis result reports for runs
        of the Broad Institute GDAC Firehose analysis pipeline. At least one year
        of run reports are maintained in the database, but the reports from the latest
        run will be returned by default. The set of Nozzle reports returned may be
        filtered by disease cohort, report type and report name.
      operationId: getAnalysesReports
      x-api-path-slug: analysesreports-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: date
        description: Select one or more date stamps
      - in: query
        name: format
        description: Format of result
      - in: query
        name: name
        description: Narrow search to one or more report names
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: type
        description: Narrow search to one or more report types
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Reports
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