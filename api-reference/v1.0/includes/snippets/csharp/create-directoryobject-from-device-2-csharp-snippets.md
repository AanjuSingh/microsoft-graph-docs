---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new DirectoryObject-idRequestBody
{
	AdditionalData = new()
	{
		{"@odata.id", "https://graph.microsoft.com/v1.0/directoryObjects/{id}"},
	}
};
await graphClient.Devices["device-id"].RegisteredUsers["directoryObject-id"].PostAsync(requestBody);


```