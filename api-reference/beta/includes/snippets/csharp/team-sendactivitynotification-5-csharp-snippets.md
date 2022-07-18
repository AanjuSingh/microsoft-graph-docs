---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SendActivityNotificationRequestBody
{
	Topic = new TeamworkActivityTopic
	{
		Source = "entityUrl",
		Value = "https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7",
	},
	ActivityType = "pendingFinanceApprovalRequests",
	PreviewText = new ItemBody
	{
		Content = "Internal spending team has a pending finance approval requests",
	},
	Recipient = new TeamworkNotificationRecipient
	{
		@odata.type = "microsoft.graph.channelMembersNotificationRecipient",
		AdditionalData = new()
		{
			{"teamId", "e8bece96-d393-4b9b-b8da-69cedef1a7e7"},
			{"channelId", "19:3d61a2309f094f4a9310b20f1db37520@thread.tacv2"},
		}
	},
	TemplateParameters = new List<KeyValuePair>
	{
		new KeyValuePair
		{
			Name = "pendingRequestCount",
			Value = "5",
		},
	}
};
await graphClient.Teams["team-id"].SendActivityNotification.PostAsync(requestBody);


```