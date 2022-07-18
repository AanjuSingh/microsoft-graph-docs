---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ForwardRequestBody
{
	Comment = "comment-value",
	ToRecipients = new List<Recipient>
	{
		new Recipient
		{
			AdditionalData = new()
			{
			}
		},
	}
};
await graphClient.Groups["group-id"].Threads["conversationThread-id"].Posts["post-id"].Forward.PostAsync(requestBody);


```