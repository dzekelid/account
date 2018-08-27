---
name: Azure Data Lake Analytics
x-slug: azure-data-lake-analytics
description: The Data Lake analytics service is a new distributed analytics service
  built on Apache YARN that dynamically scales so you can focus on your business goals,
  not on distributed infrastructure. Instead of deploying, configuring and tuning
  hardware, you write queries to transform your data and extract valuable insights.
  The analytics service can handle jobs of any scale instantly by simply setting the
  dial for how much power you need. You only pay for your job when it is running making
  it cost-effective. The analytics service supports Azure Active Directory letting
  you simply manage access and roles, integrated with your on-premises identity system.
  It also includes U-SQL, a language that unifies the benefits of SQL with the expressive
  power of user code. U-SQL&rsquo;s scalable distributed runtime enables you to efficiently
  analyze data in the store and across SQL Servers in Azure, Azure SQL Database and
  Azure SQL Data Warehouse.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Account
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/azure-data-lake-analytics/apis.md
specificationVersion: "0.14"
apis:
- name: DataLakeAnalyticsJobManagementClient - Account Update
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountname-patch
  description: Updates the Data Lake Analytics account object specified by the accountName
    with the contents of the account object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: :////
  tags: Analysis, Microsoft, Data, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/azure-data-lake-analytics/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountname-patch-openapi.md
- name: DataLakeAnalyticsJobManagementClient - Account Create
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountname-put
  description: Creates the specified Data Lake Analytics account. This supplies the
    user with computation services for Data Lake Analytics workloads
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: :////
  tags: Analysis, Microsoft, Data, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/azure-data-lake-analytics/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountname-put-openapi.md
- name: DataLakeAnalyticsJobManagementClient - Account Delete
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountname-delete
  description: Begins the delete delete process for the Data Lake Analytics account
    object specified by the account name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: :////
  tags: Analysis, Microsoft, Data, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/azure-data-lake-analytics/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountname-delete-openapi.md
- name: DataLakeAnalyticsJobManagementClient - Account Get
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountname-get
  description: Gets details of the specified Data Lake Analytics account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: :////
  tags: Analysis, Microsoft, Data, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/azure-data-lake-analytics/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountname-get-openapi.md
- name: DataLakeAnalyticsJobManagementClient - Account List
  x-api-slug: subscriptionssubscriptionidprovidersmicrosoft-datalakeanalyticsaccounts-get
  description: Gets the first page of Data Lake Analytics accounts, if any, within
    the current subscription. This includes a link to the next page, if any.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: :////
  tags: Analysis, Microsoft, Data, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/azure-data-lake-analytics/subscriptionssubscriptionidprovidersmicrosoft-datalakeanalyticsaccounts-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://azure.container.service.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.data.lake.analytics.stack.network
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/data-lake-analytics/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/data-lake-analytics/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/data-lake-analytics/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/data-lake-analytics/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---