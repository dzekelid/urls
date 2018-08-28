swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox Notify Appendix API v1
  description: the-dropbox-notify--is-a-part-of-dropbox-core-ap-with-a-separate-endpoint-for-notification-call-
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api-notify.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /save_url/{root}/{path}:
    post:
      summary: Save a file from the specified URL into Dropbox.
      description: |-
        Save a file from the specified URL into Dropbox.

        If the given path already exists, the file will be renamed to avoid the conflict (e.g. `myfile (1).txt`).
      operationId: save-a-file-from-the-specified-url-into-dropboxif-the-given-path-already-exists-the-file-will-be-ren
      x-api-path-slug: save-urlrootpath-post
      parameters:
      - in: path
        name: path
        description: The path in Dropbox where the file will be saved
      - in: path
        name: root
        description: 'Root folder: `auto` - automatically determines the appropriate
          root folder using your apps permissionlevel (recommended); `sandbox` - the
          codename for app folder level; `dropbox` - full dropbox access'
      - in: formData
        name: url
        description: The URL to be fetched
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - URL
      - Root
      - Path