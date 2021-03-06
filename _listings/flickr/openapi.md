swagger: "2.0"
x-collection-name: Flickr
x-complete: 1
info:
  title: Flickr
  description: explore-upload-and-organize-photos-on-flickr
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
  /rest/?method=flickr.urls.lookupUser:
    get:
      summary: Urls Lookup User
      description: Returns a user NSID, given the url to a user's photos or profile.
      operationId: getRestMethodFlickr.urls.lookupuser
      x-api-path-slug: restmethodflickr-urls-lookupuser-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: url
        description: The url to the users profile or photos page
      responses:
        200:
          description: OK
      tags:
      - Urls
      - LookupUser