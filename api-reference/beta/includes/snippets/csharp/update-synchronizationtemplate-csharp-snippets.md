---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Applications.Item.Synchronization.Templates.Item.Template
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"id" , "Slack"
		},
		{
			"applicationId" , "{id}"
		},
		{
			"factoryTag" , "CustomSCIM"
		},
	},
};
await graphClient.Applications["{application-id}"].Synchronization.Templates["{synchronizationTemplate-id}"].PutAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Authorization", "Bearer <token>");
});


```