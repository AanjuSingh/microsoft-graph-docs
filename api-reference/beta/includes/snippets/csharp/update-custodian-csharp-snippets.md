---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Custodian
{
	ApplyHoldToSources = "false",
};
await graphClient.Compliance.Ediscovery.Cases["case-id"].Custodians["custodian-id"].PatchAsync(requestBody);


```