---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Chat
{
	ChatType = "group",
	Topic = "Group chat title",
	Members = new List<ConversationMember>
	{
		new ConversationMember
		{
			@odata.type = "#microsoft.graph.aadUserConversationMember",
			Roles = new List<String>
			{
				"owner",
			}
			AdditionalData = new()
			{
				{"user@odata.bind", "https://graph.microsoft.com/beta/users('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')"},
			}
		},
		new ConversationMember
		{
			@odata.type = "#microsoft.graph.aadUserConversationMember",
			Roles = new List<String>
			{
				"owner",
			}
			AdditionalData = new()
			{
				{"user@odata.bind", "https://graph.microsoft.com/beta/users('82fe7758-5bb3-4f0d-a43f-e555fd399c6f')"},
			}
		},
		new ConversationMember
		{
			@odata.type = "#microsoft.graph.aadUserConversationMember",
			Roles = new List<String>
			{
				"guest",
			}
			AdditionalData = new()
			{
				{"user@odata.bind", "https://graph.microsoft.com/beta/users('8ba98gf6-7fc2-4eb2-c7f2-aef9f21fd98g')"},
			}
		},
	}
};
var result = await graphClient.Chats.PostAsync(requestBody);


```