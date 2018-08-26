---
swagger: "2.0"
x-collection-name: Fire Browse
x-complete: 1
info:
  title: Fire Browse Beta API
  description: a-simple-and-elegant-way-to-explore-cancer-data
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
  /Archives/StandardData:
    get:
      summary: Retrieve standard data archives.
      description: This service returns the archive URLs for our Firehose standard
        data runs, providing a RESTful interface similar in spirit to the command
        line firehose_get tool. The archives can be filtered based on date, cohort,
        data type, platform, center, data level, and protocol.
      operationId: getArchivesStandarddata
      x-api-path-slug: archivesstandarddata-get
      parameters:
      - in: query
        name: center
        description: Narrow search to one or more TCGA centers from the scrollable
          list
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: data_type
        description: Narrow search to one or more TCGA data types from the scrollable
          list
      - in: query
        name: date
        description: Select one or more date stamps
      - in: query
        name: format
        description: Format of result
      - in: query
        name: level
        description: Narrow search to one or more TCGA data levels
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: platform
        description: Narrow search to one or more TCGA data generation platforms from
          the scrollable list
      - in: query
        name: protocol
        description: Narrow search to one or more sample characterization protocols
          from the scrollable list
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: tool
        description: Narrow search to include only data/results produced by the selected
          Firehose tool
      responses:
        200:
          description: OK
      tags:
      - Archives
      - StandardData
---