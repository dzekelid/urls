---
name: Fire Browse
x-slug: fire-browse
description: A simple and elegant way to explore cancer data. Sitting above one of
  the deepest and most integratively characterized open cancer datasets in the world.
  Backed by a powerful computational infrastructure, application programming interface
  (API), graphical tools and online reports. With over 80K sample aliquots from 11,000+
  cancer patients, spanning 38 unique disease cohorts.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
x-kinRank: "7"
x-alexaRank: "0"
tags: URLs
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/urls/master/_listings/fire-browse/apis.md
specificationVersion: "0.14"
apis:
- name: Fire Browse Beta API - Retrieve links to summary reports from Firehose analysis
    runs.
  x-api-slug: analysesreports-get
  description: This service returns URLs to the analysis result reports for runs of
    the Broad Institute GDAC Firehose analysis pipeline. At least one year of run
    reports are maintained in the database, but the reports from the latest run will
    be returned by default. The set of Nozzle reports returned may be filtered by
    disease cohort, report type and report name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1
  tags: Cancer, API Provider, Data Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/urls/master/_listings/fire-browse/analysesreports-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/urls/master/_listings/fire-browse/analysesreports-get-openapi.md
- name: Fire Browse Beta API - Retrieve standard data archives.
  x-api-slug: archivesstandarddata-get
  description: This service returns the archive URLs for our Firehose standard data
    runs, providing a RESTful interface similar in spirit to the command line firehose_get
    tool. The archives can be filtered based on date, cohort, data type, platform,
    center, data level, and protocol.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1
  tags: Cancer, API Provider, Data Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/urls/master/_listings/fire-browse/archivesstandarddata-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/urls/master/_listings/fire-browse/archivesstandarddata-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://factual.api.gallery.streamdata.io
- type: x-api-stack
  url: http://fire.browse.stack.network
- type: x-website
  url: http://firebrowse.org
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---