---
swagger: "2.0"
x-collection-name: Botify
x-complete: 0
info:
  title: Botify Parameters Analyses Username Project Slug Analysis Slug Crawl Statistics
    Urls List Type
  description: Parameters analyses username project slug analysis slug crawl statistics
    urls list type.
  version: 1.0.0
host: api.botify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /analyses/{username}/{project_slug}/{analysis_slug}/crawl_statistics/urls/{list_type}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Crawl Statistics Urls
        List Type
      description: Return a list of 1000 latest URLs crawled (all crawled URLs or
        only URLS with HTTP errors)
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugCrawlStatisticsUrlsListType
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statisticsurlslist-type-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
      - Urls
      - List
      - Type
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Crawl Statistics
        Urls List Type
      description: Parameters analyses username project slug analysis slug crawl statistics
        urls list type.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugCrawlStatisticsUrlsListType
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statisticsurlslist-type-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
      - Urls
      - List
      - Type
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