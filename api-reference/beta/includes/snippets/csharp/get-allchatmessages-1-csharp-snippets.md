---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Chats["chat-id"].Messages.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Top = 2;
	requestConfiguration.QueryParameters.OrderBy = "createdDateTime%20desc";
});


```