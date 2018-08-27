swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /enterprises/{enterpriseId}/serviceAccount:
    get:
      summary: Return Service Account
      description: |-
        Returns a service account and credentials. The service account can be bound to the enterprise by calling setAccount. The service account is unique to this enterprise and EMM, and will be deleted if the enterprise is unbound. The credentials contain private key data and are not stored server-side.

        This method can only be called after calling Enterprises.Enroll or Enterprises.CompleteSignup, and before Enterprises.SetAccount; at other times it will return an error.

        Subsequent calls after the first will generate a new, unique set of credentials, and invalidate the previously generated credentials.

        Once the service account is bound to the enterprise, it can be managed using the serviceAccountKeys resource.
      operationId: androidenterprise.enterprises.getServiceAccount
      x-api-path-slug: enterprisesenterpriseidserviceaccount-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: query
        name: keyType
        description: The type of credential to return with the service account
      responses:
        200:
          description: OK
      tags:
      - Account