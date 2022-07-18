---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Contacts.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "startswith(displayName,'A')";
	requestConfiguration.QueryParameters.Count = true;
	requestConfiguration.QueryParameters.Top = 1;
	requestConfiguration.QueryParameters.Orderby = new [] { "displayName" };
	requestConfiguration.Headers.Add("ConsistencyLevel", "eventual");
});


```