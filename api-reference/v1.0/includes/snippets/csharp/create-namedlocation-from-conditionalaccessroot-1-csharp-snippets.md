---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new NamedLocation
{
	@odata.type = "#microsoft.graph.ipNamedLocation",
	DisplayName = "Untrusted IP named location",
	AdditionalData = new()
	{
		{"isTrusted", false},
		{"ipRanges", new List<Object>
		{
		}
	}
};
var result = await graphClient.Identity.ConditionalAccess.NamedLocations.PostAsync(requestBody);


```