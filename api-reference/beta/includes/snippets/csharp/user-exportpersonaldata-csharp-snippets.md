---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new StorageLocationRequestBody
{
	StorageLocation = "storageLocation-value",
};
await graphClient.Users["user-id"].ExportPersonalData.PostAsync(requestBody);


```