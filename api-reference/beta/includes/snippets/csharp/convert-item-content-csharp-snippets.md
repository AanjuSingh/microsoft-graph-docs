---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

await graphClient.Drive.Items["driveItem-id"].Content.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Format = "%7Bformat%7D";
});


```