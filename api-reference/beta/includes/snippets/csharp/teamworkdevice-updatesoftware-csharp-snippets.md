---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UpdateSoftwareRequestBody
{
	SoftwareType = "teamsClient",
	SoftwareVersion = "1.0.96.22",
};
await graphClient.Teamwork.Devices["teamworkDevice-id"].UpdateSoftware.PostAsync(requestBody);


```