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
  /account/info:
    get:
      summary: Retrieves information about the user's account.
      description: Retrieves information about the user's account.
      operationId: retrieves-information-about-the-users-account
      x-api-path-slug: accountinfo-get
      parameters:
      - in: query
        name: locale
        description: Use to specify language settings for user error messages and
          other language specific text
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Account
      - Info