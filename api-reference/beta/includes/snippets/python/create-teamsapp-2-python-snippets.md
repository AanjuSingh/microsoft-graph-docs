---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = TeamsAppsRequestBuilder.TeamsAppsRequestBuilderPostQueryParameters(
		requiresreview = true,
)

request_configuration = TeamsAppsRequestBuilder.TeamsAppsRequestBuilderPostRequestConfiguration(
query_parameters = query_params,
)


await client.appCatalogs.teamsApps.post(request_configuration = request_configuration)


```