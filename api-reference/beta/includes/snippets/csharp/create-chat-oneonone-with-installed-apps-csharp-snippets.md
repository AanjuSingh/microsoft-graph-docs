---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Chat
{
	ChatType = "oneOnOne",
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
				{"user@odata.bind", "https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"},
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
				{"user@odata.bind", "https://graph.microsoft.com/beta/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"},
			}
		},
	}
	InstalledApps = new List<TeamsAppInstallation>
	{
		new TeamsAppInstallation
		{
			AdditionalData = new()
			{
				{"teamsApp@odata.bind", "https://graph.microsoft.com/beta/appCatalogs/teamsApps/05F59CEC-A742-4A50-A62E-202A57E478A4"},
			}
		},
	}
};
var result = await graphClient.Chats.PostAsync(requestBody);


```