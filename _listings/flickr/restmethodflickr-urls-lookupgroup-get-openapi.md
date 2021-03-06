---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Urls Lookup Group
  description: Returns a group NSID, given the url to a group's page or photo pool.
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.urls.getGroup:
    get:
      summary: Urls Get Group
      description: Returns the url to a group's page.
      operationId: getRestMethodFlickr.urls.getgroup
      x-api-path-slug: restmethodflickr-urls-getgroup-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: group_id
        description: The NSID of the group to fetch the url for
      responses:
        200:
          description: OK
      tags:
      - Urls
      - GetGroup
  /rest/?method=flickr.urls.getUserPhotos:
    get:
      summary: Urls Get User Photos
      description: Returns the url to a user's photos.
      operationId: getRestMethodFlickr.urls.getuserphotos
      x-api-path-slug: restmethodflickr-urls-getuserphotos-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: user_id
        description: The NSID of the user to fetch the url for
      responses:
        200:
          description: OK
      tags:
      - Urls
      - GetUserPhotos
  /rest/?method=flickr.urls.getUserProfile:
    get:
      summary: Urls Get User Profile
      description: Returns the url to a user's profile.
      operationId: getRestMethodFlickr.urls.getuserprofile
      x-api-path-slug: restmethodflickr-urls-getuserprofile-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: user_id
        description: The NSID of the user to fetch the url for
      responses:
        200:
          description: OK
      tags:
      - Urls
      - GetUserProfile
  /rest/?method=flickr.urls.lookupGallery:
    get:
      summary: Urls Lookup Gallery
      description: Returns gallery info, by url.
      operationId: getRestMethodFlickr.urls.lookupgallery
      x-api-path-slug: restmethodflickr-urls-lookupgallery-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: url
        description: The gallerys URL
      responses:
        200:
          description: OK
      tags:
      - Urls
      - LookupGallery
  /rest/?method=flickr.urls.lookupGroup:
    get:
      summary: Urls Lookup Group
      description: Returns a group NSID, given the url to a group's page or photo
        pool.
      operationId: getRestMethodFlickr.urls.lookupgroup
      x-api-path-slug: restmethodflickr-urls-lookupgroup-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: url
        description: The url to the groups page or photo pool
      responses:
        200:
          description: OK
      tags:
      - Urls
      - LookupGroup
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