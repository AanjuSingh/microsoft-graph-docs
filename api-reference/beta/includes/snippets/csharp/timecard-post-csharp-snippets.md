---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TimeCard
{
	ClockInEvent = new TimeCardEvent
	{
		DateTime = DateTimeOffset.Parse("2019-03-18T00:00:00.000Z"),
		AtApprovedLocation = true,
		Notes = new ItemBody
		{
			Content = "Started late due to traffic in CA 237",
			ContentType = "text",
		},
	},
	Notes = new ItemBody
	{
		Content = "8 To 5 Inventory management",
		ContentType = "text",
	},
	Breaks = new List<TimeCardBreak>
	{
		new TimeCardBreak
		{
			BreakId = "string",
			Notes = new ItemBody
			{
				Content = "Lunch break",
				ContentType = "text",
			},
			Start = new TimeCardEvent
			{
				DateTime = DateTimeOffset.Parse("2019-03-18T02:00:00.000Z"),
				AtApprovedLocation = true,
				Notes = new ItemBody
				{
					Content = "Reduced break to make up for lost time",
					ContentType = "text",
				},
			},
		},
	}
	AdditionalData = new()
	{
		{"onBehalfOfUserId", "a3601044-a1b5-438e-b742-f78d01d68a67"},
	}
};
var result = await graphClient.Teams["team-id"].Schedule.TimeCards.PostAsync(requestBody);


```