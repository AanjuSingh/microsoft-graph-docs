---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new DataSource-idRequestBody
{
	AdditionalData = new()
	{
		{"@odata.id", "https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/userSources/c25c3914-f9f7-43ee-9cba-a25377e0cec6"},
	}
};
await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].Searches["ediscoverySearch-id"].CustodianSources["dataSource-id"].PostAsync(requestBody);


```