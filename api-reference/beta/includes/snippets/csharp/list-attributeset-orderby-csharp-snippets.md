---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Directory.AttributeSets.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.OrderBy = "id";
});


```