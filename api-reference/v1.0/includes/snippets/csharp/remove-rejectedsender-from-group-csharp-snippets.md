---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

await graphClient.Groups["group-id"].RejectedSenders.$ref.DeleteAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Id = "https://graph.microsoft.com/v1.0/users/%7Buser-id%7D";
});


```