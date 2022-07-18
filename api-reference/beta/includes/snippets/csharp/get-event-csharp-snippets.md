---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Me.Events["event-id"].GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Select = new [] { "subject" , "body" , "bodyPreview" , "organizer" , "attendees" , "start" , "end" , "location" , "hideAttendees" };
	requestConfiguration.Headers.Add("Prefer", "outlook.timezone="Pacific Standard Time"");
});


```