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
		Value = "https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}",
	},
	ActivityType = "reservationUpdated",
	PreviewText = new ItemBody
	{
		Content = "You have moved up the queue",
	},
	Recipient = new TeamworkNotificationRecipient
	{
		@odata.type = "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
		AdditionalData = new()
		{
			{"userId", "jacob@contoso.com"},
		}
	},
	TemplateParameters = new List<KeyValuePair>
	{
		new KeyValuePair
		{
			Name = "reservationId",
			Value = "TREEE433",
		},
		new KeyValuePair
		{
			Name = "currentSlot",
			Value = "23",
		},
	}
};
await graphClient.Teams["team-id"].SendActivityNotification.PostAsync(requestBody);


```