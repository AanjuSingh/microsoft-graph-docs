---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Me.Events["event-id"].Instances.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.StartDateTime = "2019-04-08T09:00:00.0000000";
	requestConfiguration.QueryParameters.EndDateTime = "2019-04-30T09:00:00.0000000";
	requestConfiguration.QueryParameters.Select = new [] { "subject" , "bodyPreview" , "seriesMasterId" , "type" , "recurrence" , "start" , "end" };
});


```