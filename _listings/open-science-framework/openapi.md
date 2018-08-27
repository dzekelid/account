swagger: "2.0"
x-collection-name: Open Science Framework
x-complete: 1
info:
  title: Open Science Framework
  description: osf-provides-free-and-open-source-project-management-support-for-researchers-across-the-entire-research-lifecycle--as-a-collaboration-tool-osf-helps-researchers-work-on-projects-privately-with-a-limited-number-of-collaborators-and-make-parts-of-their-projects-public-or-make-all-the-project-publicly-accessible-for-broader-dissemination--as-a-workflow-system-osf-enables-connections-to-the-many-services-researchers-already-use-to-streamline-their-process-and-increase-efficiency--as-a-flexible-repository-it-can-store-and-archive-research-data-protocols-and-materials--
  contact:
    name: OSF
    url: https://osf.io/support
    email: support@osf.io
  version: "2.0"
host: test-api.osf.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/addons/{provider}/accounts/{account_id}/:
    get:
      summary: Retrieve an addon account
      description: |-
        Retrieves the details of an addon account

        #### Permissions

        Addon accounts are visible only to the user that authorized the account.

        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested addon account, if the request was successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: Users_addon_accounts_read
      x-api-path-slug: usersuser-idaddonsprovideraccountsaccount-id-get
      parameters:
      - in: path
        name: account_id
        description: The unique identifier of the addon account
      - in: path
        name: provider
        description: The unique identifier of the addon provider
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Addons
      - Provider
      - Accounts
      - Account