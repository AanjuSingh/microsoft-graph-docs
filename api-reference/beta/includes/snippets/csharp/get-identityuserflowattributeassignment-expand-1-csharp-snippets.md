---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Identity.B2cUserFlows["b2cIdentityUserFlow-id"].UserAttributeAssignments.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Expand = new [] { "userAttribute" };
});


```