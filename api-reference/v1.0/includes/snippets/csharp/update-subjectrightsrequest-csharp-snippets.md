---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SubjectRightsRequest
{
	@odata.type = "#microsoft.graph.subjectRightsRequest",
	InternalDueDateTime = DateTimeOffset.Parse("2021-08-30T00:00:00Z"),
};
await graphClient.Privacy.SubjectRightsRequests["subjectRightsRequest-id"].PatchAsync(requestBody);


```