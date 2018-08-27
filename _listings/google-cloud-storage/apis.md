---
name: Google Cloud Storage
x-slug: google-cloud-storage
description: Google Cloud Storage is unified object storage for developers and enterprises,
  from live data serving to data analytics/ML to data archiving. Google Cloud Storage
  allows world-wide storage and retrieval of any amount of data at any time. You can
  use Google Cloud Storage for a range of scenarios including serving website content,
  storing data for archival and disaster recovery, or distributing large data objects
  to users via direct download.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Account
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/google-cloud-storage/apis.md
specificationVersion: "0.14"
apis:
- name: Google Cloud Storage - Get Service Account
  x-api-slug: v1getgoogleserviceaccount-get
  description: Returns the Google service account that is used by Storage Transfer
    Service to access buckets in the project where transfers run or in other projects.
    Each Google service account is associated with one Google Developers Console project.
    Users should add this service account to the Google Cloud Storage bucket ACLs
    to grant access to Storage Transfer Service. This service account is created and
    owned by Storage Transfer Service and can only be used by Storage Transfer Service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/google-cloud-storage/v1getgoogleserviceaccount-get-openapi.md
- name: Google Cloud Storage - Get Account
  x-api-slug: v1googleserviceaccountsprojectid-get
  description: Returns the Google service account that is used by Storage Transfer
    Service to access buckets in the project where transfers run or in other projects.
    Each Google service account is associated with one Google Developers Console project.
    Users should add this service account to the Google Cloud Storage bucket ACLs
    to grant access to Storage Transfer Service. This service account is created and
    owned by Storage Transfer Service and can only be used by Storage Transfer Service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/google-cloud-storage/v1googleserviceaccountsprojectid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.cloud.sql.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.cloud.storage.stack.network
- type: x-authentication
  url: https://cloud.google.com/storage/docs/authentication
- type: x-best-practices
  url: https://cloud.google.com/storage/docs/best-practices
- type: x-change-log
  url: https://cloud.google.com/storage/release-notes
- type: x-code
  url: https://cloud.google.com/storage/docs/reference/libraries
- type: x-concepts
  url: https://cloud.google.com/storage/docs/concepts
- type: x-dmca-policy
  url: https://cloud.google.com/storage/docs/dmca
- type: x-faq
  url: https://cloud.google.com/storage/docs/faq
- type: x-getting-started
  url: https://cloud.google.com/storage/docs/quickstarts
- type: x-guides
  url: https://cloud.google.com/storage/docs/how-to
- type: x-pricing
  url: https://cloud.google.com/storage/pricing
- type: x-service-level-agreements
  url: https://cloud.google.com/storage/sla
- type: x-support
  url: https://cloud.google.com/storage/docs/resources-support
- type: x-tutorials
  url: https://cloud.google.com/storage/docs/tutorials
- type: x-website
  url: https://cloud.google.com/storage/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---