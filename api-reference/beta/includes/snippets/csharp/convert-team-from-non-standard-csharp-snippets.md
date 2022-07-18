---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Team
{
	DisplayName = "My Class Team",
	Description = "My Class Team’s Description",
	AdditionalData = new()
	{
		{"template@odata.bind", "https://graph.microsoft.com/beta/teamsTemplates('educationClass')"},
	}
};
var result = await graphClient.Teams.PostAsync(requestBody);


```