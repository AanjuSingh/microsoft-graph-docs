---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Me.Profile.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Expand = new [] { "names($select=first,last)" , "skills($select=displayName)" };
});


```