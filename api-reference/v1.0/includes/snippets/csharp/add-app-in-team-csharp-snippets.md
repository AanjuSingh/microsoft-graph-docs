---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TeamsAppInstallation
{
	AdditionalData = new()
	{
		{"teamsApp@odata.bind", "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"},
	}
};
var result = await graphClient.Teams["team-id"].InstalledApps.PostAsync(requestBody);


```