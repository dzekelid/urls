---
swagger: "2.0"
x-collection-name: link.fish
x-complete: 0
info:
  title: link.fish Get social media accounts
  description: |-
    Visits the URL and checks if there are any social media accounts and returns the found ones.

    Will by default return the account identifiers and not the full URL to the profiles. To return URLs instead set the parameter "return_urls" to true.

    The URLs can also be created manually like this:

    | Property        | URL                                    |
    | --------------- | -------------------------------------- |
    | facebookPage    | https://facebook.com/{ID}              |
    | githubUser      | https://github.com/{ID}                |
    | googlePlus      | https://plus.google.com/+{ID}          |
    | instagram       | https://instagram.com/{ID}             |
    | linkedInCompany | https://linkedin.com/company/{ID}      |
    | pinterest       | https://pinterest.com/{ID}             |
    | twitter         | https://twitter.com/{ID}               |
    | youTubeUser     | https://youtube.com/user/{ID}          |

    Properties only get set when a value for it has been found. That means that if no social media account has been found only the property "url" will be set.
  termsOfService: https://link.fish/terms-of-service/
  contact:
    name: link.fish
    url: https://link.fish/api
    email: api@link.fish
  version: "2017-12-01"
host: api.link.fish
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Urls/apps:
    get:
      summary: Get mobile apps
      description: |-
        Visits the URL and checks if there are mobile apps on them and returns the found ones.

        Will by default return the app identifiers and not the full URL to the apps. To return URLs instead set the parameter "return_urls" to true.

        The URLs can also be created manually like this:

        | Property | URL                                                |
        | -------- | -------------------------------------------------- |
        | android  | https://play.google.com/store/apps/details?id={ID} |
        | ios      | https://itunes.apple.com/us/app/app-name/id{ID}    |

        Properties only get set when a value for it has been found. That means that if no app has been found only the property "url" will be set.
      operationId: Urls.apps.get
      x-api-path-slug: urlsapps-get
      parameters:
      - in: query
        name: browser_render
        description: If the page should be fully rendered with a browser to extract
          data
      - in: query
        name: return_urls
        description: Returns app URLs instead of the identifiers
      - in: query
        name: url
        description: The URL of the website to query
      responses:
        200:
          description: OK
      tags:
      - Urls
      - Apps
  /Urls/browser-data:
    get:
      summary: Extract data (browser)
      description: Visits the URL with a full browser and extracts the data. This
        request costs 5 credits.
      operationId: Urls.browser_data.get
      x-api-path-slug: urlsbrowserdata-get
      parameters:
      - in: query
        name: item_format
        description: If the items should be return normal with multiple levels or
          flat with just one level and linked instead
      - in: query
        name: screenshot
        description: If and what kind of screenshot should be returned
      - in: query
        name: screenshot_file_format
        description: The file format of the screenshot
      - in: query
        name: screenshot_width
        description: The widh of the screenshot in pixel
      - in: query
        name: simplify_special_types
        description: Some types like PropertyValue do save key and value in separate
          properties which makes the data harder to process
      - in: query
        name: url
        description: The URL of the website to query
      responses:
        200:
          description: OK
      tags:
      - Urls
      - Browser
      - Data
  /Urls/browser-screenshot:
    get:
      summary: Generate screenshot (browser)
      description: Visits the URL with full browser and creates a screenshot. This
        request costs 5 credits.
      operationId: Urls.browser_screenshot.get
      x-api-path-slug: urlsbrowserscreenshot-get
      parameters:
      - in: query
        name: file_format
        description: The file format of the screenshot
      - in: query
        name: type
        description: What kind of screenshot should be returned
      - in: query
        name: url
        description: The URL of the website to create screenshot of
      - in: query
        name: width
        description: The widh of the screenshot in pixel
      responses:
        200:
          description: OK
      tags:
      - Urls
      - Browser
      - Screenshot
  /Urls/data:
    get:
      summary: Extract data
      description: Visits the URL and extracts the data.
      operationId: Urls.data.get
      x-api-path-slug: urlsdata-get
      parameters:
      - in: query
        name: browser_render
        description: If the page should be fully rendered with a browser to extract
          data
      - in: query
        name: item_format
        description: If the items should be return normal with multiple levels or
          flat with just one level and linked instead
      - in: query
        name: simplify_special_types
        description: Some types like PropertyValue do save key and value in separate
          properties which makes the data harder to process
      - in: query
        name: url
        description: The URL of the website to query
      responses:
        200:
          description: OK
      tags:
      - Urls
      - Data
  /Urls/geo-coordinates:
    get:
      summary: Get geo coordinates
      description: |-
        Visits the URL and checks if there are Geo Coordinates on them and returns the found ones.

        Properties only get set when a value for both latitude and longitude have been found. That means that if no geo coordinates have been found only the property "url" will be set.
      operationId: Urls.geo_coordinates.get
      x-api-path-slug: urlsgeocoordinates-get
      parameters:
      - in: query
        name: browser_render
        description: If the page should be fully rendered with a browser to extract
          data
      - in: query
        name: url
        description: The URL of the website to query
      responses:
        200:
          description: OK
      tags:
      - Urls
      - Geo
      - Coordinates
  /Urls/social-media:
    get:
      summary: Get social media accounts
      description: |-
        Visits the URL and checks if there are any social media accounts and returns the found ones.

        Will by default return the account identifiers and not the full URL to the profiles. To return URLs instead set the parameter "return_urls" to true.

        The URLs can also be created manually like this:

        | Property        | URL                                    |
        | --------------- | -------------------------------------- |
        | facebookPage    | https://facebook.com/{ID}              |
        | githubUser      | https://github.com/{ID}                |
        | googlePlus      | https://plus.google.com/+{ID}          |
        | instagram       | https://instagram.com/{ID}             |
        | linkedInCompany | https://linkedin.com/company/{ID}      |
        | pinterest       | https://pinterest.com/{ID}             |
        | twitter         | https://twitter.com/{ID}               |
        | youTubeUser     | https://youtube.com/user/{ID}          |

        Properties only get set when a value for it has been found. That means that if no social media account has been found only the property "url" will be set.
      operationId: Urls.social_media.get
      x-api-path-slug: urlssocialmedia-get
      parameters:
      - in: query
        name: browser_render
        description: If the page should be fully rendered with a browser to extract
          data
      - in: query
        name: return_urls
        description: Returns profile URLs instead of the profile names/ids
      - in: query
        name: url
        description: The URL of the website to query
      responses:
        200:
          description: OK
      tags:
      - Urls
      - Social
      - Media
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