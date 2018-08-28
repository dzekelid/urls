---
swagger: "2.0"
x-collection-name: Botify
x-complete: 0
info:
  title: Botify Parameters Analyses Username Project Slug Analysis Slug Urls Datamodel
  description: Parameters analyses username project slug analysis slug urls datamodel.
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
  /analyses/{username}/{project_slug}/{analysis_slug}/features/ganalytics/orphan_urls/{medium}/{source}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Ganalytics
        Orphan Urls Medium Source
      description: 'Legacy    List of Orphan URLs. URLs which generated visits from
        the selected source according to Google Analytics data, but were not crawled
        with by the Botify crawler (either because no links to them were found on
        the website, or because the crawler was not allowed to follow these links
        according to the project settings).   For a search engine (medium: origanic;
        sources: all, aol, ask, baidu, bing, google, naver, yahoo, yandex) or a social
        network (medium: social; sources: all, facebook, google+, linkedin, pinterest,
        reddit, tumblr, twitter)'
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesGanalyticsOrphanUrlsMediumSource
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturesganalyticsorphan-urlsmediumsource-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
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
      - Features
      - Ganalytics
      - Orphan
      - Urls
      - Medium
      - Source
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Ganalytics
        Orphan Urls Medium Source
      description: Parameters analyses username project slug analysis slug features
        ganalytics orphan urls medium source.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesGanalyticsOrphanUrlsMediumSource
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturesganalyticsorphan-urlsmediumsource-parameters
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
      - Features
      - Ganalytics
      - Orphan
      - Urls
      - Medium
      - Source
  /analyses/{username}/{project_slug}/{analysis_slug}/features/visits/orphan_urls/{medium}/{source}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Visits Orphan
        Urls Medium Source
      description: 'List of Orphan URLs. URLs which generated visits from the selected
        source according to Google Analytics data, but were not crawled with by the
        Botify crawler (either because no links to them were found on the website,
        or because the crawler was not allowed to follow these links according to
        the project settings).   For a search engine (medium: origanic; sources: all,
        aol, ask, baidu, bing, google, naver, yahoo, yandex) or a social network (medium:
        social; sources: all, facebook, google+, linkedin, pinterest, reddit, tumblr,
        twitter)'
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesVisitsOrphanUrlsMediumSource
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturesvisitsorphan-urlsmediumsource-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
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
      - Features
      - Visits
      - Orphan
      - Urls
      - Medium
      - Source
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Visits
        Orphan Urls Medium Source
      description: Parameters analyses username project slug analysis slug features
        visits orphan urls medium source.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesVisitsOrphanUrlsMediumSource
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturesvisitsorphan-urlsmediumsource-parameters
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
      - Features
      - Visits
      - Orphan
      - Urls
      - Medium
      - Source
  /analyses/{username}/{project_slug}/{analysis_slug}/urls:
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Urls
      description: Parameters analyses username project slug analysis slug urls.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugUrls
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurls-parameters
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
      - Urls
    post:
      summary: Post Analyses Username Project Slug Analysis Slug Urls
      description: Post analyses username project slug analysis slug urls.
      operationId: postAnalysesUsernameProjectSlugAnalysisSlugUrls
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurls-post
      parameters:
      - in: query
        name: area
        description: Analysis context
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      - in: body
        name: UrlsQuery
        description: Urls query
        schema:
          $ref: '#/definitions/holder'
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
      - Urls
  /analyses/{username}/{project_slug}/{analysis_slug}/urls/aggs:
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Urls Aggs
      description: Parameters analyses username project slug analysis slug urls aggs.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugUrlsAggs
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsaggs-parameters
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
      - Urls
      - Aggs
    post:
      summary: Post Analyses Username Project Slug Analysis Slug Urls Aggs
      description: Post analyses username project slug analysis slug urls aggs.
      operationId: postAnalysesUsernameProjectSlugAnalysisSlugUrlsAggs
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsaggs-post
      parameters:
      - in: query
        name: area
        description: Analysis context
      - in: body
        name: UrlsAggsQueries
        description: UrlsAggs queries
        schema:
          $ref: '#/definitions/holder'
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
      - Urls
      - Aggs
  /analyses/{username}/{project_slug}/{analysis_slug}/urls/datamodel:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Urls Datamodel
      description: Get analyses username project slug analysis slug urls datamodel.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugUrlsDatamodel
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsdatamodel-get
      parameters:
      - in: query
        name: area
        description: Analysis context
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
      - Urls
      - Datamodel
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Urls Datamodel
      description: Parameters analyses username project slug analysis slug urls datamodel.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugUrlsDatamodel
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsdatamodel-parameters
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
      - Urls
      - Datamodel
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