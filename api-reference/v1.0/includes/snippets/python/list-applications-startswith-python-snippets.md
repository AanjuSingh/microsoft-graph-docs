---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = ApplicationsRequestBuilder.ApplicationsRequestBuilderGetQueryParameters(
		filter = "startswith(displayName,%20'a')",
		count = true,
		top = 1,
		orderby = ["displayName"],
)

request_configuration = ApplicationsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)
headers = {
				'ConsistencyLevel' : "eventual",
}

)


result = await client.applications.get(request_configuration = request_configuration)


```