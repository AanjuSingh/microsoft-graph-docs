---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UnifiedGroupSource
{
	IncludedSources = "mailbox",
	AdditionalData = new()
	{
		{"group@odata.bind", "https://graph.microsoft.com/v1.0/groups/93f90172-fe05-43ea-83cf-ff785a40d610"},
	}
};
var result = await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].Custodians["ediscoveryCustodian-id"].UnifiedGroupSources.PostAsync(requestBody);


```