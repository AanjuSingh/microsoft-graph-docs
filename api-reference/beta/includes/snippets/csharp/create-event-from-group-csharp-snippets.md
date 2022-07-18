---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Event
{
	Subject = "Let's go for lunch",
	Body = new ItemBody
	{
		ContentType = "HTML",
		Content = "Does late morning work for you?",
	},
	Start = new DateTimeTimeZone
	{
		DateTime = "2019-06-15T12:00:00",
		TimeZone = "Pacific Standard Time",
	},
	End = new DateTimeTimeZone
	{
		DateTime = "2019-06-15T14:00:00",
		TimeZone = "Pacific Standard Time",
	},
	Location = new Location
	{
		DisplayName = "Harry's Bar",
	},
	Attendees = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"type", "required"},
			}
		},
	}
};
var result = await graphClient.Groups["group-id"].Events.PostAsync(requestBody);


```