---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Groups["group-id"].MemberOf.Group.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Count = true;
	requestConfiguration.QueryParameters.Orderby = new [] { "displayName" };
	requestConfiguration.QueryParameters.Filter = "startswith(displayName,%20'A')";
	requestConfiguration.Headers.Add("ConsistencyLevel", "eventual");
});


```