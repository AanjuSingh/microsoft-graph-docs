---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PlannerAssignedToTaskBoardTaskFormat
{
	OrderHintsByAssignee = new PlannerOrderHintsByAssignee
	{
		AdditionalData = new()
		{
			{"aaa27244-1db4-476a-a5cb-004607466324", "8566473P 957764Jk!"},
		}
	},
};
await graphClient.Planner.Tasks["plannerTask-id"].AssignedToTaskBoardFormat.PatchAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Prefer", "return=representation");
	requestConfiguration.Headers.Add("If-Match", "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="");
});


```