---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Me.Messages.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Select = new [] { "subject" , "body" , "bodyPreview" , "uniqueBody" };
	requestConfiguration.Headers.Add("Prefer", "outlook.body-content-type="text"");
});


```