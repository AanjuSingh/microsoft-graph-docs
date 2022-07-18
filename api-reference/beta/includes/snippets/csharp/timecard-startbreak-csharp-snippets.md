---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new StartBreakRequestBody
{
	Notes = new ItemBody
	{
		ContentType = "text",
		Content = "start break smaple notes",
	},
	AdditionalData = new()
	{
		{"atAprovedLocation", true},
	}
};
var result = await graphClient.Teams["team-id"].Schedule.TimeCards["timeCard-id"].StartBreak.PostAsync(requestBody);


```